---
title:  "Instalando e configurando kubernetes localmente com o minikube no Mac OSX"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
header:
  image: https://github.com/vinicius3w/vinicius3w.github.io/blob/master/images/header-by-jesus-kiteque-224069.jpg?raw=true
  caption: "Photo credit: @ikukevk on [**Unsplash**](https://unsplash.com/photos/w7ZyuGYNpRQ)"
categories: 
  - DevOps
tags:
  - Container
  - Kubernetes
  - Minikube
  - Site Reliability Engineering
  - Docker
  - Helm
  - Container Registry
---

O [Minikube](https://kubernetes.io/docs/setup/minikube/) é a ferramenta ideal para configurar uma instância/cluster [kubernetes](https://kubernetes.io/) (chamaremos de k8s a partir de agora) localmente para testar e experimentar suas implantações.

Neste artigo vamos tentar ajudá-los a colocá-lo em funcionamento na sua máquina local (Mac OSX), registrar algumas dicas sobre onde e como as coisas deves ser feitas e também tentar torná-lo capaz de usar o Helm (eu suponho que quando você usa o k8s quer aprender e usar o Helm, etcd, istio etc).

> Este artigo tem o objetivo de ser um guia de referência para um ambiente k8s local.

# Instalação do Minikube

O Minikube trabalha com máquinas virtuais e, para isso, pode usar várias opções dependendo de sua preferência e sistema operacional. Minha preferência neste caso é o [VirtualBox](https://www.virtualbox.org/wiki/Downloads) da Oracle.

Você pode usar o **brew** para instalar tudo:

```bash
$ brew cask install virtualbox minikube
```

Nesse caso, você pode obter algum tipo de erro de instalação inconclusivo relacionado à instalação do VirtualBox, especialmente no Mojave e provavelmente depois (hehehe).

O que quer que seja dito, provavelmente é um novo recurso de segurança do MacOS X que está no seu caminho.

Vá para **Preferências do Sistema> Segurança e Privacidade** e na tela **Geral**, você verá uma (ou algumas) mensagens sobre algum software que precisa de aprovação para instalar. Você deve revisar cuidadosamente a lista se houver mais de uma e permitir a instalação do software necessário - neste caso, o **software da Oracle**.

Depois disso, você pode executar novamente o comando acima e, quando estiver pronto, você deve estar pronto para as próximas etapas.

# Executando e acessando o cluster

Começar não poderia ser tão fácil quanto

```bash
$ minikube start
```

Para otimizar os recursos da sua máquina local, sugiro que sempre interrompa o minikube quando não precisar mais dele ... Com o VirtualBox sempre em execução, ele pode drenar a bateria do laptop (se for o caso) rapidamente:

```bash
$ minikube stop
```

O dashboard do Kubernetes também está disponível (enquanto o minikube está em execução):

```bash
$ minikube dashboard
```

Eu suponho que você já tenha o [**kubectl**](https://kubernetes.io/docs/tasks/tools/install-kubectl/) instalado localmente e que já o esteja usando para alguns clusters remotos, de modo que você tenha vários contextos. Neste caso, você precisa listar os contextos e mudar para o minikube (nos seguintes comandos, assumindo o nome padrão que é, “minikube”):

```bash
$ kubectl config get-contexts
$ kubectl config use-context minikube
```

Agora que você está no contexto do seu cluster k8s local que roda no minikube, podemos fazer todas as operações do k8s nele.

# Ingress controller

Para executar suas implantações que têm Ingress (e eu suponho que a maioria delas terá), você precisará do add-on:

```bash
$ minikube addons enable ingress
```

Certifique-se de configurar a entrada com base em seus hosts locais. Basicamente, significa que o que você definir como host em suas regras do Ingress precisa ser configurado em seu arquivo `/etc/hosts`

```
[minikube ip] your.host
```

Onde você lê "[minikube ip]" deve substituir pelo ip atual do minikube. Ele também funciona com vários hosts locais separados por espaço após o ip do minikube.

Aqui está o atalho para fazer isso no bash:

```bash
$ echo "$(minikube ip) local.host" | sudo tee -a /etc/hosts
```

# Container registry — i.e. Docker registry

> A realidade do uso real de um *container registry* no ambiente local é difícil, por isso vamos adotar uma opção fácil, rápida e corriqueira que torna bastante simples implantar seu trabalho local em seu k8s local, mas priva você da experiência realmente importante de usar um *container registry*.

## Container registry local

Obtenha o contexto do docker local para apontar para o contexto do minikube:

```bash
$ eval $(minikube docker-env)
```

> Para reverter: ```$ eval $(docker-machine env -u)```

**No contexto do minikube, para iniciar o registro do docker local:**

```bash
$ docker run -d -p 5000:5000 --restart=always --name registry registry:2
```

Então, agora você tem o registro local para enviar itens (contanto que sua janela de encaixe esteja no contexto do minikube).

**Agora você pode fazer:**

```bash
$ docker build . -t <your_tag>
$ docker tag <your_tag> localhost:5000/<your_tag>:<version>
```

Nesse ponto, você pode usar **localhost:5000/<your_tag>:** como imagem em sua implantação e é isso.

##Usando o repositório de contêiner remoto

Para usar o repositório de contêiner remoto localmente, você precisa fornecer uma maneira de autenticar, que é através dos [secrets](https://kubernetes.io/docs/concepts/configuration/secret/) do k8s.

Para o gerenciamento de segredos locais para registros ECR, GCR e Docker, eu recomendo usar o addon minikube chamado de [registry-creds](https://github.com/upmc-enterprises/registry-creds)(credenciais de registro). Eu não o considero seguro o suficiente para ser usado em qualquer lugar, mas em ambiente local tudo bem.

```bash
$ minikube addons configure registry-creds
$ minikube addons enable registry-creds
```

> **Nota sobre a configuração do ECR**: Certifique-se de que, se você estiver configurando-o para o AWS ECR e não tiver o papel que deseja usar (normalmente não tem e é opcional), defina-o com algo aleatório como "changeme" ou smt... Ele requer valor, se você simplesmente pressionar enter (já que é opcional) a implantação do pod de creds falhará e tornará sua vida miserável (hahahaha).

In case of AWS ECR, that will let you pull from your repo directly setting url as container image and adding pull secret named awsecr-cred:
No caso do AWS ECR, isso permitirá que você faça o pull do repo definindo diretamente a URL como imagem do contêiner e adicionando o pull secret chamado awsecr-cred:

```
imagePullSecrets:
      - name: awsecr-cred
```

> Eu tenho que observar aqui que executar isso localmente funcionou de forma bastante caótica para mim e cada sessão foi uma nova experiência e um novo truque para fazer com que funcionasse... **Não é um caminho feliz**.

# Helm

Helm é o gerenciador de pacotes para o k8s e é frequentemente usado para gerenciamento de configurações entre implantações. Com alta da popularidade da ferramenta e o constante aumento da sua adoção, é interessante terminar este guia com a nota sobre a adição do Helm ao seu ambiente k8s local.

É bem fácil neste momento, basta usar o minikube:

```bash
$ brew install kubernetes-helm
$ helm init
```

> Essa deve ser uma informação obsoleta muito em breve, mas atualmente o Helm usa um backend chamado Tiller e isso é o que é instalado/implantado durante a execução do helm init.
> 
> Você deve verificar a implantação do Helm com: ```$ kubectl describe deploy tiller-deploy — namespace=kube-system```

Leitura muito importante: <https://docs.helm.sh/using_helm/>

Agora você tem um ambiente local k8s completo capaz de aceitar todas as suas implantações de teste antes de decidir colocá-las na nuvem (ou em um servidor "*raw iron*" em algum lugar).
