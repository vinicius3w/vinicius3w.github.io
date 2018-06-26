---
title:  "O que é arquitetura Serverless (sem servidor)?"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
header:
  image: https://github.com/vinicius3w/vinicius3w.github.io/blob/master/images/header-by-jesus-kiteque-224069.jpg?raw=true
  caption: "Photo credit: @ikukevk on [**Unsplash**](https://unsplash.com/photos/w7ZyuGYNpRQ)"
categories: 
  - Development
tags:
  - Serverless
  - Engenharia de Software
  - Desenvolvimento
  - boas práticas
  - Function as a Service
  - Function
  - Lambda
---

Sem servidor ou *Serverless*, a mais nova _buzzword_ do momento (tá, nem tão nova assim dependendo de quão *early adopter* você é) vem ganhando muita atenção dos profissionais e estudantes no mundo (indústria e academia) de Tecnologia da Informação. Em parte devido à forma como os fornecedores/provedores de nuvem, como a [AWS](https://aws.amazon.com/pt/serverless/) e [Microsoft Azure](https://azure.microsoft.com/en-us/services/functions/), majoritariamente, fizeram o _hype_ da arquitetura, de conferências a _meetups_, a posts de blogs e artigos em quase todos os lugares. Além disso, novos projetos pipocam o tempo todo (nota: vale à pena conferir o [Fn](https://github.com/fnproject/fn)). Mas serverless não é apenas sobre o _hype_, ele promete também a possibilidade de implementações de negócios do "jeito ideal" e que, em um primeiro momento, soa bastante agradável para os ouvidos e, provavelmente, lança uma luz sobre os custos e o orçamento também.

O lema no universo Serverless é

> _“Focus on your **application**, not the **infrastructure**”_

Temos que reconhecer, é um lema reconfortante, principalmente sabendo que muitas das nossas horas do dia são dedicadas a implementar, manter, depurar e monitorar a nossa infraestrutura. Com toda essa carga na infraestrutura fora do nosso caminho, de fato poderíamos nos concentrar nos tão sonhados **objetivos de negócios** (ou _business drivers_) que nossas aplicações devem atender. Neste contexto, muitos esforços poderiam ser direcionados para onde os resultados são realmente mais importantes, e valiosos. Claro, soa como mais uma [bala de prata](http://www.cs.nott.ac.uk/~pszcah/G51ISS/Documents/NoSilverBullet.html), mas se você pensar bem, é asism que as coisas deveriam ser desde o princípio né? Pelo menos para aqueles que não podem gastar tanto esforço (tempo e dinheiro) presos nas ais diversas complexidades de infraestrutura (principalmente nos dias de hoje, com [as mais modernas complexidades](https://cloudplatform.googleblog.com/2018/06/Time-to-Hello-World-VMs-vs-containers-vs-PaaS-vs-FaaS.html)).

## E então, o que é Serverless?

Serverless é um modelo de execução de computação em nuvem no qual o provedor de nuvem gerencia **dinamicamente** a **alocação** e o **provisionamento** de servidores para atender a uma computação (execução, função). Uma aplicação Serverless é executada em [contêineres](https://www.docker.com/what-container) _stateless_ (sem estado) que são disparados por evento (_event-triggered_), **efêmeros** (podem durar por uma chamada) e totalmente gerenciados pelo provedor de nuvem. O preço é baseado no número de execuções, e não na capacidade de computação pré-adquirida. 

> Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of **third-party services**, **client-side logic** and cloud-hosted remote procedure calls (**Functions as a Service**).

A maioria dos provedores de nuvem investiram pesado em serverless. Com essa promoção maciça e a oferta realista, podemos seguramente assumir que serverless será um dos serviços em nuvem mais usados nos próximos anos. Aqui estão alguns dos serviços em nuvem atualmente disponíveis:

* [AWS Lambda](https://aws.amazon.com/lambda/)
* [Google Cloud Functions](https://cloud.google.com/functions/)
* [Azure Functions](https://azure.microsoft.com/en-us/services/functions/)
* [IBM OpenWhisk](https://www.ibm.com/cloud-computing/bluemix/openwhisk)
* [Alibaba Function Compute](https://www.alibabacloud.com/product/function-compute)
* [Iron Functions](http://open.iron.io/)
* [Auth0 Webtask](https://webtask.io/)
* [Oracle Fn Project](https://fnproject.io/)
* [Kubeless](https://kubeless.io/)

## Arquitetura Tradicional vs Serverless

[![]({{ BASE_PATH }}/images/2018-06-26-o-que-eh-arquitetura-serverless/1_x_v5NRC3TTMt1MaYl1gMUg.png)](https://www.gocd.org/2017/06/26/serverless-architecture-continuous-delivery/)
Fonte: <https://www.gocd.org/2017/06/26/serverless-architecture-continuous-delivery/>

Durante anos, as aplicações eram executadas em servidores que sempre necessitavam de correções, atualizações além de uma dedicação contínua (madrugadas à fio) para mantê-los em operação. Desta forma, **TODA** responsabilidade do funcionamento deles estava em **você**. Serverless tende a ser diferente dessa situação, onde você não precisa mais se preocupar com os servidores subjacentes. Eles já não são mais gerenciados por você e com o gerenciamento fora do quadro, a responsabilidade recai sobre os fornecedores de nuvem. Mas, independentemente dos recursos interessantes do Serverless, em alguns casos, a arquitetura tradicional o supera.

### Preço

Uma das principais vantagens de usar Serverless é o **custo reduzido**. O modelo de custo do Serverless é baseado em **execução**: você é cobrado pelo número de execuções. Você recebe um certo número de **segundos de uso** que varia de acordo com a **quantidade de memória necessária**. Da mesma forma, o preço por MS (milissegundos) varia com a quantidade de memória necessária. Obviamente, funções de execução mais curtas são mais adaptáveis a esse modelo, com um pico de tempo de execução de 300 segundos para a maioria dos fornecedores de nuvem.

O vencedor aqui é a arquitetura Serverless.

### Networking

A desvantagem é que as funções Serverless são acessadas apenas como **APIs privadas**. Para acessá-los, você deve configurar um **gateway de API**. Isso não afeta seu preço ou processo, mas significa que você não pode acessá-los diretamente por meio do IP habitual.

O vencedor aqui é a arquitetura tradicional.

### Dependências de terceiros

A maioria, se não todos os projetos, têm dependências externas. Eles dependem de bibliotecas que não estão embutidas na linguagem ou framework que você usa. Desenvolvedores costumam usar bibliotecas com funcionalidades que incluem criptografia, processamento de imagens, etc., e essas bibliotecas podem ser muito pesadas. Sem acesso no nível do sistema, a solução é empacotar essas dependências na própria aplicação.

> Reinventar a roda **nem sempre** é uma boa ideia.

O vencedor aqui é baseado no contexto. Para aplicações simples com **poucas dependências**, o Serverless é o vencedor; para qualquer coisa **mais complexa**, a arquitetura tradicional é a vencedora.

### Ambientes

Configurar ambientes diferentes para Serverless é tão fácil quanto configurar um ambiente único. Como se trata de pagamento por execução, temos aqui uma grande melhoria em relação aos servidores tradicionais, já que desta forma não há mais a necessidade de configurar máquinas de desenvolvimento, teste e produção, por exemplo. 

O vencedor aqui é a arquitetura Serverless.

### Timeout

Com a computação Serverless, há um limite de timeout de **300 segundos**. Funções muito complexas ou de **longa duração** não são boas para Serverless, mas ter um timeout rígido impossibilita a realização de determinadas tarefas. Um limite rígido nesse tempo torna o Serverless inutilizável para aplicações que possuem tempos de execução variáveis e para determinados serviços que requerem informações de uma fonte externa.

O vencedor claro aqui é a arquitetura tradicional.

### Escala

O processo de escalonamento para Serverless é automático e contínuo, mas há falta de controle ou total ausência de controle. Embora o dimensionamento automático seja ótimo, é difícil não conseguir resolver e atenuar erros relacionados a novas instâncias Serverless.

Temos um empate técnico entre a arquitetura Serverless e a tradicional.

## Functions as a Service (FaaS)

O FaaS é uma implementação de arquiteturas Serverless onde os desevnolvedores podem implantar uma função individual ou uma parte da lógica de negócios. Eles começam em milissegundos (~ 100 ms para o [AWS Lambda](https://aws.amazon.com/lambda/)) e processam solicitações individuais em um intervalo de tempo - no geral - de 300 segundos - imposto pela maioria dos fornecedores de nuvem.

### Princípios do FaaS

* Gerenciamento completo de servidores
* Cobrança baseada em invocação
* Orientado a eventos e instantaneamente escalonável

### Propriedades chave do FaaS

* **Funções lógicas independentes do lado do servidor:** Os FaaS são semelhantes às funções que você está acostumado a escrever em linguagens de programação. Unidades de lógica **pequenas**, separadas, que recebem argumentos de entrada, operam na entrada e retornam o resultado.
* **Sem estado:** Com o Serverless, **tudo é sem estado**, você não pode salvar um arquivo no disco em uma execução da sua função e esperar que ela esteja lá na próxima. Quaisquer duas invocações da mesma função podem ser executadas em contêineres completamente diferentes sob o teto.
* **Efêmero:** FaaS são projetados para iniciar rapidamente, fazer seu trabalho e depois desligar novamente. Eles não permanecem sem uso. Contanto que a tarefa seja executada, os contêineres subjacentes são descartados.
* **Disparados por evento:** Embora as funções possam ser chamadas diretamente, elas geralmente são acionadas por eventos de outros serviços de nuvem, como solicitações HTTP, novas entradas de banco de dados ou notificações de mensagens de entrada. FaaS são frequentemente usados e considerados como a cola entre serviços em um ambiente de nuvem.
* **Escalonável por padrão:** Com as funções _stateless_, vários contêineres podem ser inicializados, permitindo que tantas funções sejam executadas (em paralelo, se necessário), conforme necessário, para atender continuamente a todas as solicitações recebidas.
* **Totalmente gerenciado por um fornecedor de nuvem:** O [AWS Lambda](https://aws.amazon.com/lambda/), [Azure Functions](https://azure.microsoft.com/en-us/services/functions/), [IBM OpenWhisk](https://www.ibm.com/cloud-computing/bluemix/openwhisk) e o [Google Cloud Functions](https://cloud.google.com/functions/) são as soluções FaaS mais conhecidas disponíveis atualmente. Cada oferta suporta tipicamente uma variedade de linguagens e tempos de execução, i.e. Node.js, Python, .NET Core, Java.

## Aplicação Serverless (um exemplo da AWS)

Uma solução Serverless consiste em um servidor Web, funções Lambda (FaaS), serviço de token de segurança (STS), autenticação do usuário e banco de dados.

[![]({{ BASE_PATH }}/images/2018-06-26-o-que-eh-arquitetura-serverless/1_TIrjN7EjLUVJmJ6YvHR7Dg.png)](http://blog.tonyfendall.com/2015/12/serverless-architectures-using-aws-lambda/)
Fonte: <http://blog.tonyfendall.com/2015/12/serverless-architectures-using-aws-lambda/>

* **Aplicação Cliente** - A UI da sua aplicação é renderizada no lado do cliente em algum framework frontend javascript, que nos permite usar um servidor web simples e estático.
* _Servidor Web_ - O Amazon S3 fornece um servidor Web robusto e simples. Todos os arquivos HTML, CSS e JS estáticos para nossa aplicação podem ser fornecidos a partir do S3.
* **Funções Lambda (FaaS)** - São os principais facilitadores na arquitetura Serverless. Os serviços da aplicação para efetuar login e acessar dados serão criados como funções Lambda. Estas funções irão ler e escrever a partir do seu banco de dados e fornecer respostas JSON.
* **Security Token Service (STS)** - Gera credenciais temporárias da AWS (chave de API e chave secreta) para os usuários da aplicação. Essas credenciais temporárias são usadas pela aplicação cliente para chamar a API da AWS (e, portanto, chamar o Lambda).
* **Autenticação do usuário** - O AWS Cognito é um serviço de identidade integrado ao AWS Lambda. Com o Amazon Cognito, você pode adicionar facilmente a inscrição do usuário e o login em suas aplicações Web e móveis. Ele também tem as opções para autenticar usuários através de provedores de identidade social como Facebook, Twitter ou Amazon, com soluções de identidade SAML ou usando seu próprio sistema de identidade.
* **Banco de dados** - O AWS DynamoDB fornece um banco de dados NoSQL totalmente gerenciado. O DynamoDB não é essencial para uma aplicação Serverless, mas é usado como um exemplo aqui.

## Benefícios da arquitetura Serverless

### Da perspectiva de negócios

* O custo gerado por uma aplicação Serverless é baseado no número de execuções da função, medido em milissegundos em vez de horas.
* Agilidade do processo: Unidades implantáveis menores resultam em entrega mais rápida de recursos ao mercado, aumentando a capacidade de adaptação à mudança.
* O custo de contratação de engenheiros de infraestrutura de backend cai.
* Custos operacionais reduzidos.

### Da perspectiva do desenvolvedor

* Responsabilidade reduzida, sem infraestrutura de backend a ser gerida.
* Zero administração do sistema.
* Gerenciamento operacional mais fácil.
* Promove a adoção de Nanoservices, Microservices, Princípios SOA.
* Configuração mais rápida.
* Escalável, não precisa se preocupar com o número de solicitações simultâneas.
* Monitorando fora da caixa.
* Promove a inovação.

### Da perspectiva do usuário

* Se as empresas estão usando essa vantagem competitiva para enviar recursos mais rapidamente, os clientes estão recebendo novos recursos mais rapidamente do que antes.
* É possível que os usuários possam fornecer mais facilmente seu próprio backend de armazenamento (ou seja, Dropbox, Google Drive).
* É mais provável que esses tipos de aplicações ofereçam armazenamento em cache no lado do cliente, o que proporciona uma melhor experiência offline.

## Desvantagens da arquitetura Serverless

### Da perspectiva de negócios

* Controle total reduzido.
* O temido bloqueio de fornecedor (_vendor lock-in_) exige mais confiança para um provedor terceirizado.
* Exposição adicional ao risco requer mais confiança para um provedor terceirizado.
* Risco de segurança.
* Risco de Recuperação de Desastres.
* Todos esses inconvenientes podem ser mitigados com alternativas de código aberto, mas à custa dos benefícios de custo mencionados anteriormente.

### Da perspectiva do desenvolvedor

* A tecnologia imatura resulta em fragmentação de componentes, melhores práticas não são claras.
* Complexidade arquitetônica.
* A disciplina necessária contra a expansão de funções.
* A multilocação (_multi-tenancy_) significa que é tecnicamente possível que as funções vizinhas possam sobrecarregar os recursos do sistema nos bastidores.
* Testar localmente se torna complicado.
* Restrições significativas no estado local.
* A duração da execução é limitada.
* Falta de ferramentas operacionais.

### Da perspectiva do usuário

* A menos que seja arquitetado corretamente, uma aplicação pode fornecer uma experiência ruim ao usuário como resultado do aumento da latência da solicitação.

## Serverless Frameworks

Plataformas Serverless precisam de infraestruturas onde possam ser executadas. Estruturas independentes de provedores fornecem uma maneira independente de plataforma para definir e implantar código Serverless em várias plataformas de nuvem ou serviços comerciais.

* [Serverless Framework](https://serverless.com/) (Javascript, Python, Golang)
* [Apex](http://apex.run/) (Javascript)
* [ClaudiaJS](https://claudiajs.com/) (Javascript)
* [Sparta](https://gosparta.io/) (Golang)
* [Gordon](https://github.com/jorgebastida/gordon) (Javascript)
* [Zappa](https://www.zappa.io/) (Python)
* [Up](https://github.com/apex/up) (Javascript, Python, Golang, Crystal)

## Resumo

A arquitetura Serverless é certamente muito interessante, mas ainda possui uma série de limitações. Vale ressaltar que a validade e o sucesso das arquiteturas de software dependem muito mais dos requisitos do negócio e do que das tecnologias. Da mesma forma, Serverless pode se destacar quando usado em local/contexto adequado.

Aqui estão alguns links para você começar sua jornada sem Serverless.

* [Serverless Examples](https://github.com/serverless/examples) – A collection of boilerplates and examples of serverless architectures built with the Serverless Framework and AWS Lambda.
* [Awesome Serverless](https://github.com/anaibol/awesome-serverless) - A curated list of awesome services, solutions and resources for serverless / nobackend applications.

Este post foi baseado nos seguintes artigos: ["The Benefits of Serverless Computing and its Impact on DevOps"](https://hackernoon.com/the-benefits-of-serverless-computing-and-its-impact-on-devops-e75d82c47ac4), ["Comparing PubNub Functions vs. AWS Lambda Functions"](https://www.pubnub.com/blog/comparing-pubnub-functions-vs-aws-lambda-functions/), ["Time to “Hello, World”: VMs vs. containers vs. PaaS vs. FaaS"](https://cloudplatform.googleblog.com/2018/06/Time-to-Hello-World-VMs-vs-containers-vs-PaaS-vs-FaaS.html) e ["What is Serverless Architecture? What are its Pros and Cons?"](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9).