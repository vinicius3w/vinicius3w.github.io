---
title:  "Ensinando Engenharia de Software na Prática, Parte V"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
header:
  image: https://github.com/vinicius3w/vinicius3w.github.io/blob/master/images/header-by-jesus-kiteque-224069.jpg?raw=true
  caption: "Photo credit: @ikukevk on [**Unsplash**](https://unsplash.com/photos/w7ZyuGYNpRQ)"
categories: 
  - Education
tags:
  - software engineering
  - cloud computing
  - teaching
  - platform engineering
  - digital engineering
  - software product engineering
  - software architecture
  - software testing
  - software quality
  - software engineer
  - devops
  - site reliability engineering
  - sre
---

No [terceiro artigo da série, mas primeiro dessa temporada](https://viniciusgarcia.me/education/ensinando-engenharia-de-software-na-pratica-parte-iii/) eu comecei a discussão acerca da necessidade de evolução da [disciplina de Engenharia de Software sob a minha responsabilidade](https://bit.ly/vcg-es), no [curso de Sistemas de Informação](https://portal.cin.ufpe.br/graduacao/sistemas-de-informacao/) do [Centro de Informática de UFPE](https://www.cin.ufpe.br/). A seguir, no [quarto artigo da série, e segundo dessa temporada](https://viniciusgarcia.me/education/ensinando-engenharia-de-software-na-pratica-parte-iv/) eu evoluí as discussões acerca da **Educação em Engenharia de Software** em especial a complexidade e dificuldade que é lidar com uma disciplina de 60 horas que em algumas instituições já se transformou em curso de graduação. 

E, para além disso, temos um assunto da disciplina que também pode ser candidata a um curso de graduação (tá, posso estar exagerando, mas 60 horas é tempos de menos para lidar com Arquitetura de Software) e, portanto, vale a pena entender a relação entre a [Engenharia de Produtos de Software](https://bit.ly/3K2Q1aV) versus [Arquitetura de Software](https://bit.ly/3cT8VwN).

Além destas duas áreas dentro da engenharia de software também temos a engenharia de plataforma. Em resumo, a [Engenharia de Plataforma](https://www.gartner.com/en/articles/what-is-platform-engineering) é uma área da engenharia de software que se concentra no design, desenvolvimento e manutenção de plataformas, que são definidas como a base ou infraestrutura subjacente de um sistema de software. A engenharia de plataforma é importante porque as plataformas são a base sobre a qual os sistemas de software são construídos, e é crucial que essas plataformas sejam bem projetadas, desenvolvidas e mantidas. 

Neste artigo, exploraremos mais a fundo o surgimento da engenharia de plataforma, discutindo seus principais conceitos, técnicas e ferramentas, e como ela está transformando a maneira como as empresas criam e entregam seus produtos e serviços digitais.

## O surgimento da Engenharia de Plataforma

A [Engenharia de Plataforma](https://bit.ly/3YGR3gS) é uma área emergente dentro da ciência da computação que está ganhando cada vez mais destaque nos últimos anos. Trata-se de um conjunto de técnicas, metodologias e ferramentas utilizadas para criar, gerenciar e evoluir plataformas digitais, que são sistemas complexos e escaláveis que suportam a integração de diversos aplicativos e serviços. Essas plataformas são projetadas para serem flexíveis e modulares, permitindo que novos recursos possam ser adicionados ou removidos de forma ágil e eficiente.

Embora a engenharia de plataforma seja uma área relativamente nova, suas raízes remontam às primeiras arquiteturas de software distribuídas, desenvolvidas na década de 1970. Foi somente no início dos anos 2000, no entanto, que a engenharia de plataforma começou a ganhar maior atenção da indústria e da academia, à medida que as empresas começaram a adotar abordagens baseadas em plataformas para criar e entregar seus produtos e serviços.

As plataformas digitais se tornaram uma parte integral do mundo moderno, com exemplos que vão desde os sistemas operacionais em nossos computadores até as redes sociais e aplicativos móveis que usamos em nosso dia a dia. As plataformas são essenciais para a criação de ecossistemas digitais em larga escala, permitindo que uma ampla variedade de desenvolvedores e provedores de serviços possam interagir e colaborar para criar valor para os usuários.

Um dos principais fatores que contribuíram para o surgimento da engenharia de plataforma é a proliferação da computação em nuvem (ou cloud computing, em inglês). Com o crescimento das plataformas de computação em nuvem, como [Amazon Web Services (AWS)](https://aws.amazon.com/) e [Microsoft Azure](https://azure.microsoft.com/), surgiram novas ferramentas e tecnologias para construir, implantar e gerenciar aplicativos de software na nuvem. A computação em nuvem permite que empresas e organizações hospedem seus aplicativos em infraestruturas remotas, oferecendo maior escalabilidade, flexibilidade e disponibilidade, além de reduzir custos de infraestrutura. Isso exigiu a criação de novas plataformas e ferramentas para gerenciar aplicativos em ambientes de nuvem, o que, por sua vez, impulsionou o desenvolvimento da engenharia de plataforma.

Além disso, a adoção em larga escala de microsserviços e tecnologias de contêinerização, como o Docker, facilitou a criação e a implantação de sistemas de software distribuídos. Isso aumentou a necessidade de arquiteturas de plataforma robustas e escaláveis para apoiar esses sistemas. E, finalmente, o crescimento do desenvolvimento do software ágil levou a uma mudança para a construção e implantação de software em incrementos menores e mais frequentes. Isso aumentou a importância de ter uma plataforma flexível e escalável para construir e implantar esses incrementos.

No entanto, apesar dessa explosão de conhecimentos, a criação e gerenciamento de plataformas digitais pode ser uma tarefa complexa e desafiadora, envolvendo questões de arquitetura, segurança, desempenho, escalabilidade e governança. É aí que entra a engenharia de plataforma, fornecendo uma estrutura sistemática para lidar com esses desafios e garantir que as plataformas possam evoluir de forma sustentável ao longo do tempo.

### Conceitos, técnicas e ferramentas

A [Engenharia de Plataforma](https://bit.ly/3IlAFNt) é baseada em uma série de conceitos fundamentais que ajudam a orientar o processo de criação e gestão de plataformas digitais. Entre os principais conceitos, destacam-se:

- [Arquitetura de plataforma](https://bit.ly/3HUydvU): a arquitetura de uma plataforma digital é a estrutura que define como os diversos componentes da plataforma interagem entre si. Ela deve ser projetada para suportar a integração de diferentes aplicativos e serviços, e para garantir a escalabilidade e a flexibilidade da plataforma.
- [Ecossistema de plataforma](https://bit.ly/3InLUEY): o ecossistema de uma plataforma digital é o conjunto de desenvolvedores, provedores de serviços e usuários que interagem com a plataforma. A engenharia de plataforma deve levar em conta a dinâmica do ecossistema para garantir que a plataforma possa evoluir de forma sustentável e atender às necessidades de seus usuários.
- [APIs (_application programming interface_)](https://ibm.co/3YuRg79): APIs são as interfaces que permitem que diferentes aplicativos e serviços se comuniquem com a plataforma. A engenharia de plataforma deve projetar APIs que sejam fáceis de usar e escaláveis, garantindo a interoperabilidade entre diferentes sistemas.

Por sua vez, a engenharia de plataforma utiliza uma série de técnicas para criar, gerenciar e evoluir plataformas digitais. Algumas das principais técnicas incluem:

- [DevOps](https://bit.ly/vcg-devops): DevOps é uma abordagem de desenvolvimento de software que enfatiza a colaboração e a integração contínua entre as equipes de desenvolvimento e operações. Na engenharia de plataforma, o DevOps é utilizado para automatizar a implantação e a gestão da plataforma, reduzindo o tempo de inatividade e aumentando a eficiência operacional.
- [Microsserviços](https://bit.ly/vcg-microservices): microsserviços são uma abordagem de arquitetura de software que consiste em dividir uma aplicação em serviços independentes e autônomos, cada um com sua própria interface e funcionalidade. Na engenharia de plataforma, os microsserviços são utilizados para aumentar a flexibilidade e a escalabilidade da plataforma, permitindo que diferentes serviços sejam adicionados ou removidos conforme necessário.
- [Containers](https://bit.ly/3xntPR7): containers são ambientes isolados que permitem a execução de aplicativos em diferentes plataformas. Na engenharia de plataforma, os containers são utilizados para criar ambientes de desenvolvimento e produção padronizados e replicáveis, facilitando a implantação e a gestão da plataforma.

E, para habilitar os conceitos e as técnicas, a engenharia de plataforma faz uso de uma ampla variedade de ferramentas para dar suporte ao desenvolvimento, implantação e gestão de plataformas digitais. Algumas das principais ferramentas incluem:

- [GitLab](https://about.gitlab.com/): GitLab é uma plataforma de gerenciamento de código de código aberto que ajuda a gerenciar o ciclo de vida do código-fonte de um aplicativo. Com o GitLab, é possível hospedar um repositório de código-fonte, controlar o acesso e a colaboração de desenvolvedores, automatizar a compilação e os testes de código, entre outros. Ele oferece recursos avançados de integração contínua e entrega contínua (CI/CD), permitindo que os desenvolvedores implantem e atualizem aplicativos de forma rápida e segura.
- [Docker](https://www.docker.com/): Docker é uma plataforma de virtualização de containers de código aberto que ajuda a criar ambientes padronizados e replicáveis para o desenvolvimento, implantação e gestão de aplicativos. Com o Docker, é possível empacotar um aplicativo e suas dependências em um container, garantindo que ele possa ser executado em qualquer ambiente de infraestrutura. Ele oferece recursos avançados de gerenciamento de containers, incluindo controle de versão, distribuição, segurança e rede.
- [Kubernetes](https://kubernetes.io/): Kubernetes é uma plataforma de orquestração de containers de código aberto que ajuda a gerenciar a implantação e o escalonamento de aplicativos em ambientes de containers. Com o Kubernetes, é possível automatizar o processo de implantação e gestão de containers, garantindo que os aplicativos estejam sempre disponíveis e escaláveis. Ele oferece recursos avançados de gerenciamento de carga, balanceamento de carga, recuperação de falhas, atualização e monitoramento de aplicativos, entre outros.
- [Apache Kafka](https://kafka.apache.org/): Apache Kafka é uma plataforma de streaming de código aberto que ajuda a integrar diferentes serviços e aplicativos em uma plataforma digital, permitindo que eles troquem dados em tempo real. Com o Kafka, é possível criar pipelines de dados para transportar eventos entre diferentes serviços e aplicativos de forma confiável e escalável. Ele oferece recursos avançados de armazenamento e gerenciamento de fluxos de dados, incluindo garantias de entrega, particionamento, replicação e persistência de dados.
- [Grafana](https://grafana.com/): Grafana é uma plataforma de visualização de dados de código aberto que ajuda a monitorar o desempenho e a saúde da plataforma, fornecendo informações valiosas para os desenvolvedores e administradores da plataforma. Com o Grafana, é possível criar painéis e gráficos personalizados que mostram as métricas de desempenho, uso de recursos e atividade de usuários da plataforma. Ele oferece recursos avançados de consulta, filtragem e alerta, permitindo que os usuários personalizem a visualização e o monitoramento da plataforma de acordo com suas necessidades.

## Por que a engenharia da plataforma é importante?

A [Engenharia da Plataforma](https://bit.ly/3I3FcTv) desempenha um papel crítico na possibilidade de organizações de criar, implantar e gerenciar aplicativos de software em escala. Ajuda a garantir que esses aplicativos sejam confiáveis, eficientes e fáceis de manter. Aqui estão algumas razões específicas pelas quais a engenharia da plataforma é importante:

A engenharia da plataforma é importante porque permite que as organizações construam e implantem [plataformas digitais](https://www.credencys.com/blog/what-is-a-digital-platform/) de maneira rápida e eficiente, fornecendo uma base bem projetada e bem gerenciada, tendo uma [estratégia](https://opensenselabs.com/blog/articles/digital-platform-strategy) para reduzir o tempo e o esforço necessários para construir e implantar estes serviços.

Além disso, pela composição de metodologias e ferramentas de apoio, ajuda a garantir a confiabilidade e o desempenho das plataformas de software possam lidar com altos níveis de tráfego e uso sem ter um tempo de inatividade ou problemas de desempenho. Essa infraestrutura permite também que as organizações mantenham e atualizem facilmente seus artefatos de software. E, claro, ao implementar medidas robustas de segurança e conformidade, os engenheiros de plataformas ajudam as organizações a proteger suas plataformas de software e atender aos requisitos regulatórios que por ventura se apliquem.

### Princípios e práticas de engenharia de plataforma

Os princípios e práticas de engenharia de plataformas envolvem o design, o desenvolvimento e a manutenção de plataformas, que são definidas como a base ou infraestrutura subjacente para um sistema de software. Alguns princípios e práticas específicos de engenharia de plataforma incluem:

- **Design de arquiteturas de plataforma escaláveis e confiáveis**: os engenheiros de plataforma projetam e criam arquiteturas de plataforma capazes de lidar com altos níveis de tráfego e uso sem ter um tempo de inatividade ou problemas de desempenho.
- **Desenvolvimento e manutenção de componentes e serviços da plataforma**: os engenheiros de plataforma desenvolvem e mantêm os vários componentes e serviços que compõem a plataforma, como bancos de dados, filas de mensagens e APIs.
- **Interoperabilidade sistemas de plataformas com outras tecnologias**: os engenheiros de plataforma integram a plataforma a outras tecnologias, como plataformas de computação em nuvem e microsserviços, para permitir a construção e a implantação de aplicativos de software.
- **Garantir que as plataformas sejam fáceis de manter e atualizar**: os engenheiros de plataformas projetam plataformas fáceis de manter e atualizar, a fim de minimizar a interrupção e o tempo de inatividade ao fazer alterações na plataforma.
- **Implementando sistemas robustos de monitoramento e observabilidade**: os engenheiros de plataforma implementam sistemas de monitoramento e observabilidade para rastrear o desempenho e o uso da plataforma e identificar, resolver e antecipar problemas.
- **Implementando medidas de segurança e conformidade**: os engenheiros de plataforma implementam medidas de segurança e conformidade para proteger a plataforma e garantir que ela atenda aos requisitos regulatórios.

### Papel dos engenheiros de plataforma no processo de desenvolvimento de software

Os engenheiros da plataforma são responsáveis por garantir que uma plataforma digital seja confiável, com desempenho e sustentável, e que atenda às necessidades dos usuários, aplicações e serviços que se baseia, consomem recursos e/ou usam ela. Eles trabalham em estreita colaboração com desenvolvedores de software, gerentes de produto e outras profissionais e stakeholders para identificar e abordar desafios técnicos e para melhorar continuamente a plataforma para atender aos requisitos de negócios e técnicos em evolução.

Adicionalmente, desempenham um papel fundamental no processo de desenvolvimento de software, trabalhando para criar e manter as plataformas e sistemas subjacentes que suportam a execução das aplicações e serviços conectados às plataformas digitais. Em vez de se concentrarem apenas em escrever código para uma única aplicação, os engenheiros de plataforma se concentram em projetar, desenvolver e manter plataformas digitais compartilhadas que podem ser usadas por várias aplicações, serviços e usuários.

Além disso, os engenheiros de plataforma são responsáveis por monitorar e gerenciar o desempenho das plataformas digitais, aplicando práticas de monitoramento, análise e otimização para garantir a continuidade da execução de tudo o que compõe a plataforma digital. Eles também são responsáveis por manter as plataformas atualizadas, corrigindo falhas de segurança e implementando melhorias de desempenho, garantindo que os aplicativos sejam executados de maneira confiável e eficiente.

## E o que vem depois?

Incluir o estudo da Engenharia de Plataforma em um curso de Ciência da Computação, Engenharia da Computação, Sistemas de Informação ou correlatos é importante não apenas para atender às demandas do mercado de trabalho atual, mas também para preparar os alunos para enfrentar os desafios do futuro. A **transformação digital** está impulsionando uma crescente demanda por profissionais com conhecimento em engenharia de plataforma, uma vez que cada vez mais empresas estão migrando seus serviços para a nuvem. Isso exige uma nova abordagem para o desenvolvimento de software, com novas tecnologias, arquiteturas e metodologias.

Além disso, a Engenharia de Plataforma é uma área **interdisciplinar**, que abrange aspectos da Engenharia de Software, Redes, Sistemas Distribuídos, Segurança e Gerenciamento de Infraestrutura. Compreender a Engenharia de Plataforma pode ajudar os alunos a compreender melhor a **complexidade e a interconexão** dessas áreas, o que pode ser valioso em muitos outros contextos da Tecnologia da Informação e Comunicação.

Outro aspecto a ser considerado é o fato de que as plataformas de software são cada vez mais importantes para empresas de todos os setores, desde as de tecnologia até as de varejo, finanças e saúde. Isso significa que profissionais com habilidades em Engenharia de Plataforma têm uma ampla gama de oportunidades de carreira e podem contribuir para o sucesso de empresas em muitos setores diferentes.

Em resumo, incluir o estudo da Engenharia de Plataforma em uma disciplina de [Engenharia de Software](https://bit.ly/vcg-es) é importante para preparar os alunos para as demandas do mercado de trabalho atual, para enfrentar os desafios do futuro e para desenvolver habilidades interdisciplinares e valiosas para muitas outras áreas e mercados de tecnologia.
