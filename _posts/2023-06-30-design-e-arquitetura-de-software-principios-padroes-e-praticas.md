---
title:  "Design e arquitetura de software: princípios, padrões e práticas"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
header:
  image: https://github.com/vinicius3w/vinicius3w.github.io/blob/master/images/header-by-jesus-kiteque-224069.jpg?raw=true
  caption: "Photo credit: @ikukevk on [**Unsplash**](https://unsplash.com/photos/w7ZyuGYNpRQ)"
categories: 
  - Architecture
tags:
  - software engineering
  - platform engineering
  - Software Design
  - Software Architecture
  - Design Principles
  - Architectural Patterns
  - Service Oriented Architecture (SOA)
  - Microservices
  - Modularity
  - Scalability
  - Maintainability
  - Design Patterns
---

O design e a arquitetura de software representam a realização dos anseios e expectativas dos clientes no desenvolvimento de software, moldando a estrutura, o comportamento e os atributos de um sistema. Ele fornece um plano para o desenvolvimento de sistemas que atendem a requisitos, expectativas, restrições e regras de negócios específicas. Envolve a **tomada de decisões estratégicas** que afetam significativamente o desempenho, a capacidade de manutenção, continuidade do negócio e o sucesso geral do sistema. Este artigo visa fornecer uma compreensão abrangente dos princípios de design de software, padrões de arquitetura modernos, Arquitetura Orientada a Serviços (SOA) e microsserviços em uma abordagem didática e minimamente viável para ser o ponto de partida deste entendimento. Ao explorar esses tópicos, espero fornecer uma compreensão abrangente do assunto, minimamente completa, factível, viável e desejável e, em especial, com pequenos exemplos práticos.

## Disclaimer

Este artigo tem por objetivo estimular um debate entre os alunos da disciplina [Engenharia de Software](https://bit.ly/vcg-es) do curso de [Bacharelado em Sistemas de Informação](https://portal.cin.ufpe.br/graduacao/sistemas-de-informacao/) do [Centro de Informática](https://portal.cin.ufpe.br/) da [UFPE](https://www.ufpe.br/). Ele fornece uma visão abrangente de Design e Arquitetura de Software, mas há muitos outros aspectos a serem explorados. Por exemplo, como diferentes estilos de arquitetura afetam o desempenho do sistema? Como os princípios de design podem ser aplicados na prática? Quais são os trade-offs entre diferentes estilos arquitetônicos? Essas são apenas algumas perguntas que podem servir de ponto de partida para uma discussão rica e envolvente.

## Princípios de design e sua importância

Os princípios de design são conceitos ou diretrizes fundamentais que os desenvolvedores de software seguem para criar sistemas de alta qualidade, sustentáveis e escaláveis. Eles servem como base para o design e arquitetura de software, orientando os desenvolvedores na **tomada de decisões de design** que aprimoram os [atributos de qualidade](https://pt.wikipedia.org/wiki/ISO/IEC_9126) do sistema, como capacidade de manutenção, escalabilidade e desempenho. Esses princípios incluem conceitos como modularidade, encapsulamento, alta coesão, baixo acoplamento e ocultação de informações. Eles visam melhorar a legibilidade, reutilização e confiabilidade do software.

Um dos conjuntos mais populares de princípios de design é [SOLID](https://bit.ly/3XucLW0), um acrônimo que significa Responsabilidade Única (**S**ingle Responsibility), Aberto-Fechado (**O**pen-Closed), Substituição de Liskov (**L**iskov Substitution), Segregação de Interface (**I**nterface Segregation) e Inversão de Dependência (**D**ependency Inversion). Esses princípios orientam o design e a programação orientados a objetos, promovendo um código fácil de entender, manter e expandir.

- **Princípio de Responsabilidade Única (Single Responsibility Principle - SRP)**: Este princípio afirma que uma classe deve ter apenas um motivo para mudar. Ele encoraja os desenvolvedores a separar as responsabilidades em diferentes classes, promovendo alta coesão e baixo acoplamento.

- **Princípio Aberto-Fechado (Open-Closed Principle - OCP)**: De acordo com este princípio, as entidades de software (classes, módulos, funções, etc.) devem ser abertas para extensão, mas fechadas para modificação. Isso significa que você deve ser capaz de adicionar novas funcionalidades sem alterar o código existente.

- **Princípio da Substituição de Liskov (Liskov Substitution Principle - LSP)**: Este princípio afirma que se um programa estiver usando uma classe base, ele deve ser capaz de usar qualquer uma de suas subclasses sem que o programa saiba disso. Isso garante que uma subclasse possa substituir sua superclasse sem afetar a correção do programa.

- **Princípio de Segregação de Interface (Interface Segregation Principle - ISP)**: Este princípio sugere que os clientes não devem ser forçados a depender de interfaces que não usam. Ele promove o uso de várias interfaces específicas em vez de uma interface de uso geral.

- **Princípio de Inversão de Dependência (Dependency Inversion Principle - DIP)**: Este princípio afirma que módulos de alto nível não devem depender de módulos de baixo nível. Ambos devem depender de abstrações. Isso incentiva o desacoplamento dos módulos de software, tornando o sistema mais flexível e adaptável a mudanças.

Esses princípios, quando aplicados corretamente, podem melhorar significativamente a qualidade do design e da arquitetura do software. Eles ajudam na criação de sistemas fáceis de manter, entender e estender, reduzindo assim o custo e o esforço de desenvolvimento de software a longo prazo.

Os princípios de design não são apenas conceitos teóricos; eles têm implicações práticas que podem afetar significativamente a qualidade de um sistema de software. Por exemplo, aderir ao Princípio de Responsabilidade Única pode levar a um sistema mais fácil de manter e entender. Quando cada classe em um sistema tem uma única responsabilidade, fica mais fácil identificar onde uma mudança é necessária quando um requisito muda. Isso reduz o risco de introdução de bugs no sistema.

Da mesma forma, o Princípio Aberto-Fechado promove flexibilidade em um sistema. Ao projetar entidades de software abertas para extensão, mas fechadas para modificação, podemos adicionar novos recursos ou alterar o comportamento existente sem modificar o código existente. Isso reduz o risco de interromper a funcionalidade existente e torna o sistema mais adaptável às mudanças nos requisitos.

Na próxima seção, exploraremos os padrões arquitetônicos modernos e seu papel no design e na arquitetura de software.

## Padrões Arquitetônicos Modernos

Os padrões arquitetônicos fornecem uma solução reutilizável para problemas comuns que ocorrem na arquitetura de software. Eles representam uma visão de alto nível do sistema e fornecem uma maneira de organizar o código de maneira a promover a reutilização, manutenção e escalabilidade. Aqui estão alguns padrões arquitetônicos modernos:

- **Arquitetura em camadas**: Também conhecida como arquitetura N-tier, esse padrão organiza o sistema em camadas, cada uma fornecendo serviços para a camada acima dela. Uma arquitetura em camadas típica pode incluir uma camada de apresentação, camada de lógica de negócios e camada de acesso a dados. Esse padrão é benéfico porque separa as preocupações, tornando o sistema mais fácil de entender, manter e atualizar.
- **Model-View-Controller (MVC)**: O MVC separa a representação de dados (modelo), interface do usuário (visão) e lógica de interação do usuário (controlador). Esse padrão melhora a modularidade, permitindo o desenvolvimento e a modificação independentes de cada componente. O MVC é amplamente utilizado em aplicativos web e desktop.
- **Arquitetura Hexagonal**: Também conhecido como Portas e Adaptadores, este padrão permite que uma aplicação seja igualmente conduzida por usuários, programas, testes automatizados ou scripts em lote, e seja desenvolvida e testada isoladamente de seus eventuais dispositivos de tempo de execução e bancos de dados. O objetivo é criar componentes de aplicativos fracamente acoplados que possam ser facilmente conectados ao seu ambiente de software por meio de portas e adaptadores.
- **Event-Driven Architecture**: Este padrão é projetado em torno da produção, detecção e reação a eventos. Um evento é uma mudança de estado que aciona a execução de determinadas tarefas. Essa arquitetura é particularmente útil em sistemas de tempo real e sistemas assíncronos nos quais você deseja desacoplar o produtor de eventos do consumidor de eventos. Falaremos em detalhes a seguir.

Em resumo, os padrões arquitetônicos fornecem soluções de alto nível para problemas arquitetônicos. Eles fornecem uma maneira de comunicar sobre a estrutura de alto nível de um sistema e compartilhar conhecimento sobre problemas comuns e suas soluções. Por exemplo, o padrão de arquitetura em camadas é um padrão comum que organiza um sistema em camadas, cada uma com uma função e responsabilidade específicas. Essa separação de preocupações torna o sistema mais fácil de entender e manter. Também promove a reutilização, pois as camadas podem ser compartilhadas em diferentes partes de um sistema ou mesmo em diferentes sistemas.

A arquitetura orientada a eventos, por outro lado, é um padrão adequado para sistemas com comportamento assíncrono. Em uma arquitetura orientada a eventos, o fluxo do programa é determinado por eventos como ações do usuário, saídas de sensores ou mensagens de outros programas. Isso pode levar a um sistema mais responsivo e capaz de lidar com altas cargas.

### Arquiteturas Orientadas em Eventos (Event-Driven Architectures)

[Arquiteturas Orientadas em Eventos (Event-Driven Architectures)](https://www.redhat.com/pt-br/topics/integration/what-is-event-driven-architecture) são um paradigma arquitetural que se concentra no fluxo de eventos como o principal mecanismo de comunicação e coordenação entre componentes de um sistema de software. Nesse modelo, os eventos são as principais entidades de troca de informações e desencadeiam ações nos componentes interessados. Vamos explorar os principais aspectos das Arquiteturas Orientadas em Eventos:

- **Eventos**: Eventos representam mudanças de estado ou ocorrências significativas dentro de um sistema. Essas mudanças podem ser desencadeadas por ações de usuários, integrações com sistemas externos, atualizações de dados, entre outros. Os eventos carregam informações relevantes que são consumidas pelos componentes interessados.
- **Produtores e Consumidores**: Na arquitetura orientada em eventos, os produtores são responsáveis por gerar e publicar eventos quando ocorrem eventos significativos. Por outro lado, os consumidores são os componentes interessados em receber e reagir aos eventos. Os consumidores podem se inscrever para receber eventos específicos e processá-los de acordo com a lógica de negócios.
- **Filas de Eventos e Padrões de Mensageria**: Para garantir a entrega e a escalabilidade na troca de eventos, é comum utilizar filas de eventos e padrões de mensageria. As filas de eventos armazenam os eventos publicados até que os consumidores estejam prontos para processá-los. Os padrões de mensageria definem as formas de comunicação assíncrona entre produtores e consumidores, permitindo uma comunicação robusta e assíncrona.
- **Decoupling (Desacoplamento)**: Uma vantagem fundamental das arquiteturas orientadas em eventos é o desacoplamento entre os componentes. Os produtores e consumidores não precisam conhecer uns aos outros diretamente. Em vez disso, eles se comunicam por meio da troca de eventos. Isso permite que os componentes evoluam independentemente, facilitando a manutenção, a escalabilidade e a substituição de componentes.
- **Escalabilidade e Resiliência**: Arquiteturas orientadas em eventos são altamente escaláveis e resilientes. A comunicação assíncrona por meio de eventos permite que os componentes sejam distribuídos e dimensionados de forma independente. Além disso, caso ocorram falhas em um componente, os eventos perdidos podem ser recuperados ou tratados posteriormente.
- **Fluxo de Eventos e Modelagem de Domínio**: A adoção de arquiteturas orientadas em eventos facilita a modelagem de domínio, uma vez que os eventos refletem as mudanças de estado importantes no sistema. Através da análise dos eventos e de seus fluxos, é possível entender o comportamento do sistema e modelar as regras de negócio de forma mais precisa.

As Arquiteturas Orientadas em Eventos oferecem uma abordagem flexível e escalável para o design de sistemas de software. Ao adotar esse paradigma, os engenheiros podem construir sistemas que reagem de forma eficiente a eventos e mudanças de estado, promovendo a flexibilidade, a escalabilidade e a manutenção simplificada. As arquiteturas orientadas em eventos são especialmente adequadas para cenários em que a comunicação assíncrona e a coordenação entre componentes são essenciais.

### Service Oriented Architecture (SOA)

Arquitetura Orientada a Serviços ([Service Oriented Architecture - SOA](https://ibm.co/3prYGM2)) é um [architectural pattern](https://en.wikipedia.org/wiki/Architectural_pattern) (padrão arquitetural) - não confundir com [design pattern](https://bit.ly/3JHDjgH) (padrão de projeto) - que divide um sistema em pequenas unidades chamadas **serviços**. Cada serviço é uma unidade discreta de funcionalidade que pode ser acessada remotamente e acionada e atualizada independentemente, semelhante a como um objeto de software, na programação orientada a objetos, pode ser criado, operado e destruído independentemente.

SOA é conhecido por seus benefícios em **ambientes de grande escala**. Promove a reutilização, pois os serviços podem ser usados por vários aplicativos. Também melhora a escalabilidade, pois os serviços podem ser dimensionados individualmente com base na demanda. Além disso, como os serviços são fracamente acoplados, fazendo com que as alterações em um serviço não afetam os outros, o que simplifica a manutenção e as atualizações.

Aspectos-chave do SOA incluem:

- **Composição de Serviços**: O SOA permite a composição de serviços para construir sistemas complexos. Os serviços podem ser combinados para criar novas funcionalidades, aproveitando os princípios de baixo acoplamento e separação de preocupações. Isso promove flexibilidade e reutilização.
- **Descoberta e Registro de Serviços**: Mecanismos de descoberta de serviços, como registros de serviço, permitem que os serviços localizem e se comuniquem dinamicamente entre si. Isso desacopla os serviços de suas localizações físicas, permitindo escalabilidade e tolerância a falhas.

No entanto, a implementação de SOA não é isenta de desafios. Requer um design cuidadoso para definir os serviços e suas interações e também requer medidas de segurança robustas, pois os serviços geralmente são acessíveis por meio de uma rede.

### Arquitetura Baseada em Microservices (Microservices-Based Architecture - MBA)

A arquitetura [Microservices](https://go.aws/42ZFSS8) é um padrão de projeto que estrutura uma aplicação como uma **coleção de serviços fracamente acoplados**. Em uma arquitetura de microsserviços, os serviços são refinados e **os protocolos são leves**. O benefício de decompor uma aplicação em diferentes serviços "menores" é que ele melhora a modularidade e torna a aplicação mais fácil de entender, desenvolver e testar. Essa abordagem arquitetônica também paraleliza o desenvolvimento, permitindo que pequenas equipes autônomas desenvolvam, implantem e dimensionem seus respectivos serviços de forma independente.

Os [microsserviços](https://red.ht/3XF4Wgb) oferecem vários benefícios, incluindo flexibilidade nas opções de tecnologia, implantação independente e escalabilidade. No entanto, eles também introduzem complexidade em termos de coordenação ([orquestração](https://bit.ly/3JFt2Sl), [coreografia](https://bit.ly/3PIt67L)) de serviço, consistência de dados e operações de sistema distribuído.

Aspectos-chave dos microservices incluem:

- **Governança Descentralizada**: Os microservices adotam uma governança descentralizada, permitindo que equipes individuais tenham autonomia sobre seus respectivos serviços. Isso possibilita um desenvolvimento e implantação rápidos dos serviços, promovendo agilidade e inovação.
- **Escalabilidade e Isolamento de Falhas**: Os microservices podem ser dimensionados individualmente com base na demanda, melhorando a escalabilidade geral do sistema. Além disso, falhas em um microservice não afetam o sistema inteiro, já que eles são isolados, garantindo tolerância a falhas e resiliência do sistema.

Na próxima seção, forneceremos exemplos práticos ilustrando esses conceitos.

## Exemplos Práticos

Para entender melhor esses conceitos, vamos considerar alguns exemplos práticos.

### Exemplo de Princípios de Design

Considere um sistema para gerenciar uma biblioteca. Neste sistema, podemos ter uma classe `Livro`. De acordo com o Princípio de **Responsabilidade Única (SRP)**, esta classe deve ter apenas uma responsabilidade. Por exemplo, pode ser responsável por manter o controle das informações do livro (título, autor, ISBN, etc.). Se também atribuíssemos a ela a responsabilidade de administrar os empréstimos de livros, estaríamos violando o SRP. Em vez disso, devemos ter uma classe `Empréstimo` separada para lidar com empréstimos de livros.

### Exemplo de SOA e Microsserviços

Em uma arquitetura orientada a serviços, considere um sistema de reservas de viagens. Poderia ter serviços separados para voos, hotéis e aluguel de carros. Cada um desses serviços pode ser usado e atualizado de forma independente, promovendo a reutilização e a manutenção.

Em uma arquitetura de microsserviços, considere uma plataforma de streaming de vídeo como a Netflix. Ele pode ter microsserviços para autenticação do usuário, recomendações de vídeo, streaming e muito mais. Cada um desses microsserviços pode ser desenvolvido, implantado e dimensionado de forma independente, proporcionando flexibilidade e resiliência.

## Conclusão

O **Design e a Arquitetura de Software** são essenciais para o desenvolvimento de sistemas de software modernos, garantindo sua robustez, escalabilidade e facilidade de manutenção. Ao aderir aos princípios de design e adotar padrões arquiteturais modernos, como o SOA e microservices, os engenheiros podem criar software que atenda às necessidades em constante evolução de usuários e empresas. À medida que o campo de desenvolvimento de software continua a avançar, compreender esses conceitos e princípios torna-se cada vez mais crucial para construir sistemas de software de alta qualidade e adaptáveis. Embora esses conceitos venham com seu próprio conjunto de desafios, os benefícios que eles oferecem em termos de reutilização, escalabilidade e manutenção os tornam parte integrante da [Engenharia de Software moderna](https://bit.ly/engsoft4-0).

Isso conclui nossa exploração de Design e Arquitetura de Software. Incentivamos você a se aprofundar nesses tópicos e continuar aprendendo sobre o fascinante campo do desenvolvimento de software.

## Referências

Vamos começar com o primeiro tópico: "Princípios de design e padrões arquitetônicos modernos". Aqui estão as quatro primeiras referências relevantes sobre o tema, com base na contagem de citações:

1. [Reflections on the REST architectural style and "principled design of the modern web architecture" (impact paper award)](https://dx.doi.org/10.1145/3106237.3121282) by R. Fielding, R. Taylor, Justin R. Erenkrantz, M. Gorlick, E. J. Whitehead, Rohit Khare, P. Oreizy. This paper discusses the history, evolution, and shortcomings of REST, as well as several related architectural styles that it inspired. [Full Text](http://dl.acm.org/ft_gateway.cfm?id=3121282&type=pdf)
2. [Landscape of Architecture and Design Patterns for IoT Systems](https://dx.doi.org/10.1109/JIOT.2020.3003528) by H. Washizaki, Shinpei Ogata, A. Hazeyama, T. Okubo, E. Fernández, Nobukazu Yoshioka. This paper presents a systematic literature review of IoT architecture and design patterns. [Full Text](https://ieeexplore.ieee.org/ielx7/6488907/9219268/09120234.pdf)
3. [A Standard Driven Software Architecture for Fully Autonomous Vehicles](https://dx.doi.org/10.1109/ICSA-C.2018.00040) by A. Serban, E. Poll, Joost Visser. This paper proposes a prescriptive approach to designing a functional software architecture for fully autonomous vehicles. [Full Text](https://repository.ubn.ru.nl/bitstream/handle/2066/195379/3/195379pub.pdf)
4. [Software engineering for Responsible AI: An empirical study and operationalised patterns](https://dx.doi.org/10.1109/ICSE-SEIP55303.2022.9793864) by Q. Lu, Liming Zhu, Xiwei Xu, J. Whittle, David M. Douglas, C. Sanderson. This paper presents an empirical study involving interviews with 21 scientists and engineers to understand the practitioners' views on AI ethics principles and their implementation. [Full Text](http://arxiv.org/pdf/2111.09478)

Aqui estão as quatro primeiras referências relevantes sobre o tema "Arquitetura Orientada a Serviços (SOA) e microsserviços" com base na contagem de citações:

1. [Applications Based on Service-Oriented Architecture (SOA) in the Field of Home Healthcare](https://dx.doi.org/10.3390/s17081703) by K. Ávila, P. Sanmartín, D. Jabba, M. Jimeno. This article reviews applications developed in the health industry that implement a service-oriented (SOA) design in architecture. [Full Text](https://www.mdpi.com/1424-8220/17/8/1703/pdf?version=1500973883)
2. [RESTful API Automated Test Case Generation](https://dx.doi.org/10.1109/QRS.2017.11) by A. Arcuri. This paper proposes a fully automated white-box testing approach for RESTful APIs, where test cases are automatically generated using an evolutionary algorithm. [Full Text](http://arxiv.org/pdf/1901.01538)
3. [From The Business Motivation Model (BMM) To Service Oriented Architecture (SOA)](https://dx.doi.org/10.5381/jot.2008.7.8.c6) by Birol Berkem. This article provides insight about how to link your business vision, goals, strategies, tactics, and business rules according to BMM, then bridging the resulting business specifications toward components of a Service Oriented Architecture (SOA). [Full Text](http://www.jot.fm/issues/issue_2008_11/column6.pdf)
4. [The Role of Internet of Services (IoS) on Industry 4.0 Through the Service Oriented Architecture (SOA)](https://dx.doi.org/10.1007/978-3-319-99707-0_3) by Jacqueline Zonichenn Reis, R. F. Gonçalves. This paper discusses the role of the Internet of Services and Service Oriented Architecture in the context of Industry 4.0. [Full Text](https://hal.inria.fr/hal-02177890/file/472851_1_En_3_Chapter.pdf)

Acrescento alguns ótimos links complementares

1. [Software Architecture Guide](https://www.martinfowler.com/architecture/) by Martin Fowler.
2. [5 essential patterns of software architecture](https://www.redhat.com/architect/5-essential-patterns-software-architecture). Software is essential. What are the main architectural patterns used to create the software we all rely on daily? -- December 16, 2020 by Red Hat.
3. [14 software architecture design patterns to know](https://www.redhat.com/architect/14-software-architecture-patterns). Architectural patterns increase your productivity: These reusable schemes address common software design challenges. -- March 16, 2022 by Red Hat
4. [10 Software Architecture Patterns You Must Know About](https://www.simform.com/blog/software-architecture-patterns/). Software architecture patterns hold a lot of importance as they can be used to solve various problems. Choose the type of software architecture patterns in this blog. -- July 4, 2020 by SIMFORM
5. [What is Service-Oriented Architecture (SOA)?](https://bit.ly/3rbqG7j), by NGINX
6. [Introduction to Microservices](https://bit.ly/44nLg3b), by NGINX
7. [What Are Microservices?](https://bit.ly/434z99r), by NGINX
