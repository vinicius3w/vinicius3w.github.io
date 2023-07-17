---
title: "Desenvolvimento de Software Dirigido a Dados: Uma Visão Geral Educacional"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
header:
  image: https://github.com/vinicius3w/vinicius3w.github.io/blob/master/images/header-by-jesus-kiteque-224069.jpg?raw=true
  caption: "Photo credit: @ikukevk on [**Unsplash**](https://unsplash.com/photos/w7ZyuGYNpRQ)"
categories: 
  - Architecture
tags:
  - software engineering
  - Software Design
  - Software Architecture
  - Software Development
  - Data-Driven Software Development
  - Relational Databases
  - Non-Relational Databases
  - Object-Relational Mapping (ORM)
  - Data Access Frameworks
  - Software Development Methodologies
  - Data-Driven Decision Making
  - Software Development Tools
  - Data-Driven Design
  - Data-driven Culture
  - Data-Driven Strategy
---

Data-Driven Software Development (DDSD) é uma abordagem moderna para o desenvolvimento de software que enfatiza o uso de dados para orientar os processos de tomada de decisão.  Essa abordagem é baseada no princípio de que os dados, quando coletados, analisados ​​e interpretados adequadamente, podem fornecer informações valiosas que podem aumentar significativamente a eficiência e a eficácia dos processos de desenvolvimento de software.  Envolve o uso de indicadores-chave de desempenho (KPIs) ou objetivos e resultados-chave (OKRs) para fornecer resultados claros, objetivos e mensuráveis.  Essa abordagem é fundamental na construção de produtos lucrativos, encontrando maneiras de reduzir custos e melhorar a eficiência.

## Bancos de dados relacionais e não relacionais

 No contexto do DDSD, os dados são normalmente armazenados em bancos de dados, que podem ser relacionais ou não relacionais.

 Bancos de dados relacionais, ou bancos de dados SQL, como MySQL, Oracle e SQL Server, são baseados no modelo relacional - armazenar dados em formato tabular - que organiza os dados em tabelas com linhas e colunas.  As colunas contêm atributos de dados e as linhas possuem valores de dados.  Eles são escaláveis ​​verticalmente, o que significa que podem lidar com cargas crescentes adicionando mais recursos a um único servidor.  Esses bancos de dados são ideais para aplicativos que exigem consultas complexas, integridade transacional e forte consistência.

 Por outro lado, os bancos de dados não relacionais, às vezes chamados de bancos de dados NoSQL (Not Only SQL), como MongoDB, Cassandra e CouchDB, são projetados para escalabilidade e alto desempenho, pois não usam tabelas, campos, e modelo de dados estruturados de colunas.  Em vez disso, eles armazenam dados em um formato que seja melhor para o tipo de dados que estão manipulando.  Pode ser uma estrutura hierárquica, um gráfico ou uma estrutura orientada a documentos.  Os bancos de dados não relacionais são escalonáveis ​​horizontalmente, o que significa que eles lidam com mais tráfego adicionando mais servidores ao banco de dados.  Eles são ideais para aplicativos que exigem flexibilidade, escalabilidade e capacidade de lidar com grandes volumes de dados e tipos de dados complexos.

## Mapeamento objeto-relacional (ORM) e estruturas de acesso a dados

Object-Relational Mapping (ORM) é uma técnica de programação que cria uma "ponte" entre programas orientados a objetos e, na maioria dos casos, bancos de dados relacionais.  ORM simplifica as interações do banco de dados, permitindo que os desenvolvedores usem conceitos familiares de Programação Orientada a Objetos (OOP).  Ele usa descritores de metadados para criar uma camada entre a linguagem de programação e um banco de dados relacional, ajudando os programadores a trabalhar com bancos de dados usando sua linguagem de programação preferida.  As estruturas ORM, como Hibernate, Entity Framework e Sequelize, abstraem o sistema de banco de dados subjacente, permitindo que os desenvolvedores interajam com o banco de dados usando a linguagem de programação do aplicativo, em vez de SQL.

Estruturas de acesso a dados, como Spring Data e MyBatis, fornecem uma abordagem mais flexível para acesso a dados, permitindo que os desenvolvedores escrevam consultas SQL personalizadas quando necessário, ao mesmo tempo em que fornecem uma API de alto nível para tarefas comuns de acesso a dados.

Frameworks como Hibernate, Java Persistence API (JPA) e Java Data Objects (JDO) suportam ORM.  Por exemplo, no ecossistema .NET, Entity Framework é um ORM popular que simplifica o mapeamento entre objetos em software para tabelas e colunas em um banco de dados relacional.

## Benefícios do desenvolvimento de software dirigido a dados

 O DDSD oferece inúmeros benefícios que podem aumentar significativamente a eficiência e a eficácia dos processos de desenvolvimento de software.  Aqui estão alguns dos principais benefícios:

 1. **Visibilidade e responsabilidade:** uma abordagem robusta de desenvolvimento dirigido por dados fornece referências para maior visibilidade dos esforços de desenvolvimento atuais.  Assim, as equipes de desenvolvimento podem visualizar facilmente o impacto de seu trabalho, pois ele está vinculado ao sucesso das métricas de negócios gerais da empresa.  Isso deixa as equipes com pontos de dados claros e concisos para medir o sucesso individual e coletivo.

 2. **Time-to-Market acelerado:** O DDSD ajuda a reduzir o tempo envolvido em um projeto e acelera o time-to-market de uma versão de software, que é um componente vital das vantagens competitivas de qualquer organização.

 3. **Ambiente de solução de problemas:** O DDSD brota de um ambiente proficiente, proativo, ágil e de solução de problemas que permite que as unidades de desenvolvimento corrijam rapidamente contratempos de curto e longo prazo.

 4. **Melhoria contínua e tomada de decisão mais rápida:** O DDSD é um facilitador de melhoria contínua e tomada de decisão mais rápida.  Com a ajuda dos dados, as equipes de desenvolvimento obtêm acesso a insights valiosos e acionáveis ​​que podem ajudar efetivamente a reduzir o tempo envolvido em um projeto, solucionar desafios rotineiros, simplificar a melhoria contínua e muito mais.

 5. **Pensamento geral:** o desenvolvimento dirigido por dados também pode ajudar as organizações a explorar padrões comparativos e pesquisas de propensão de resultados exclusivos nos níveis da organização e do setor.  Isso é o que gostamos de chamar de pensamento "big picture", que ajuda as organizações a se manterem à frente da curva.

 No entanto, é importante observar que o DDSD não vem sem seus desafios. Muitas vezes, as organizações lutam para alinhar KPIs e OKRs individuais e organizacionais, falhando em medir e rastrear com precisão as contribuições individuais e coletivas. Outro desafio dessa abordagem é o volume real do trabalho, que pode levar a esforços substanciais, atrasos desnecessários ou retrabalho durante o desenvolvimento e a implantação. Apesar desses desafios, os benefícios do DDSD geralmente superam as desvantagens, tornando-o uma abordagem valiosa para o desenvolvimento de software moderno.

### Principais desafios na tomada de decisão baseada em dados

1. **Qualidade dos dados**: o primeiro desafio em um projeto baseado em dados é a descoberta de dados.  A qualidade dos conjuntos de dados é crucial e fundamental. A solução para esse desafio é seguir o ciclo de qualidade dos dados para melhorar e garantir a alta qualidade dos dados.

2. **Integração de dados**: A integração de dados é o processo de combinar dados de diferentes fontes e armazená-los juntos para obter uma visão unificada. Os problemas de integração de dados provavelmente são causados ​​por dados inconsistentes dentro de uma organização. A solução para esse problema é usar plataformas de integração de dados que possam automatizar e orquestrar transformações, criar frameworks extensíveis, otimizar o desempenho de consultas automaticamente, etc.

3. **Dados sujos**: Dados sujos são dados que contêm informações imprecisas. É praticamente impossível removê-lo completamente de um conjunto de dados. Dados sujos podem ser imprecisos, incorretos, duplicados, inconsistentes, incompletos ou violar regras de negócios. A solução para esse desafio é limpar, validar, substituir e excluir dados brutos e não estruturados com a ajuda de especialistas em gerenciamento de dados ou ferramentas de limpeza de dados.

4. **Incerteza dos dados**: A incerteza pode ocorrer por vários motivos, incluindo erros de medição, erros de processamento, etc. Ao usar dados do mundo real, erros e incertezas devem ser esperados. A solução para esse desafio é usar poderosas ferramentas de software de análise e quantificação de incertezas que podem simplificar a simulação, o teste e a análise de sistemas complexos.

5. **Transformação de dados**: Transformar dados de múltiplas fontes que normalmente são incompatíveis entre si é um desafio. Os dados precisam ser limpos e normalizados antes que possam ser usados ​​juntos. Para obter insights significativos dos dados, a transformação de dados é essencial.

Agora, vamos encontrar algumas informações sobre as tendências futuras na tomada de decisão baseada em dados.

## Tendências Futuras em Desenvolvimento de Software Dirigido a Dados

 1. **Aumento em 5G e novas tecnologias (AI, ML, AR, VR):** O poder da tecnologia 5G será a maior mudança tecnológica com poder de download mais rápido que é até 100 vezes mais rápido que 4G.  Com recursos atualizados de qualidade, como rede remota mais rápida, taxas de latência mais baixas e acessibilidade de largura de banda mais fácil, o 5G funciona bem com ofertas de alta demanda de dados. Essas ofertas incluem streaming de vídeo 4K, realidade aumentada como virtual e realidade aumentada que estão abrindo uma nova dimensão para o crescimento dos negócios. Os desenvolvedores de software estão adotando as tecnologias 5G para desenvolver aplicativos poderosos com novas funcionalidades em todos os espaços de negócios. A tecnologia será uma enorme melhoria na segurança que afastará todos os obstáculos presentes no 4G.

 2. **Expansão da Internet das Coisas (IoT):** Dispositivos e aplicativos inteligentes construídos usando IoT tornaram-se uma tendência popular no desenvolvimento de aplicações industriais, desde manufatura, processamento de alimentos até divisões de energia e saúde e medicina. Esses dispositivos permitem que as empresas tomem decisões baseadas em dados. Ao conectar tudo por meio de sensores e atuadores, a IoT está tornando nosso mundo mais inteligente. As empresas estão ansiosas para gastar mais em produtos habilitados para IoT para prosperar no futuro. Estendendo a jornada além dos dispositivos inteligentes, as empresas estão se movendo rapidamente em direção aos aplicativos. Seu objetivo é se tornar mais eficiente e fornecer recursos avançados com a integração da IoT. Na situação atual do COVID, o setor de saúde está prestes a mudar, oferecendo melhores serviços na forma de telemedicina, imagens conectadas, monitoramento de pacientes internados, dispositivos vestíveis, etc.

 3. **Produtos e aplicativos digitais:** eles se tornaram uma parte inseparável de qualquer negócio. Com mais e mais dados produzidos a cada dia, as empresas estão se voltando para software dirigido a dados. Isso marca melhorias significativas nas operações e funcionalidades de negócios. Os desenvolvedores de software estão sempre atualizados com a tecnologia mais recente e aproveitando os benefícios das atualizações. Isso significa que 2023 promete oportunidades incomparáveis. Quer uma empresa esteja desenvolvendo um produto corporativo ou lançando uma nova ideia na forma de um aplicativo móvel, essas tendências certamente os ajudariam a obter uma vantagem competitiva.

 Essas tendências indicam que o futuro do DDSD é promissor e cheio de oportunidades. O surgimento de novas tecnologias e a expansão da IoT estão abrindo caminho para processos de desenvolvimento de software mais avançados e eficientes. A integração dessas tecnologias nas operações de negócios não apenas melhora as funcionalidades, mas também fornece uma vantagem competitiva para os negócios.

## Conclusão

 O DDSD é uma abordagem poderosa que aproveita os dados para orientar a tomada de decisões e melhorar a qualidade do software. Compreender os princípios do DDSD, as diferenças entre bancos de dados relacionais e não relacionais e o papel do ORM no acesso a dados é crucial para qualquer desenvolvedor de software ou cientista de dados. Aproveitando essas ferramentas e técnicas, as organizações podem criar produtos de software mais eficientes, eficazes e lucrativos.

## Leituras Adicionais

Para os interessados ​​em se aprofundar no tópico de DDSD, aqui estão alguns recursos recomendados:

### Blog Posts

1. [Data-driven Software: Towards the Future of Programming in Data Science - Databricks](https://www.databricks.com/blog/2021/05/04/data-driven-software-towards-the-future-of-programming-in-data-science.html)
2. [Data-Driven Software Development: How To Make Strategic Dev Decisions - CloudZero](https://www.cloudzero.com/blog/data-driven-development)
3. [Data-driven development: what it is and how to do it right - DEVTALENTS](https://devtalents.com/data-driven-software-development/)
4. [What Is Data-Driven Development | Its Benefits - WayPath](https://waypathconsulting.com/data-driven-development-and-its-benefits/)
5. [Seven Industry Trends in Data-Driven Software Development](https://www.data-mania.com/blog/seven-industry-trends-in-data-driven-software-development/)

### Tutoriais Online

1. [An ultimate guide to Data-driven development and its use in web development - iFour Technolab](https://www.ifourtechnolab.com/blog/an-ultimate-guide-to-data-driven-development-and-its-use-in-web-development)
2. [Data-driven Software: Towards the Future of Programming in Data Science - Databricks](https://www.databricks.com/blog/2021/05/04/data-driven-software-towards-the-future-of-programming-in-data-science.html)
3. [Introduction - Defining Data-Driven Software Development - O'Reilly](https://www.oreilly.com/library/view/defining-data-driven-software/9781492049272/ch01.html)
4. [Build Your Own Interactive Data-Driven Web App: A Step-by-Step Guide - Medium](https://medium.com/@PedroLinsMMC/build-your-own-interactive-data-driven-web-app-a-step-by-step-guide-2485c7b2a9bd)
5. [Data-Driven Development for Stream Processing - Medium](https://medium.com/codex/data-driven-development-for-stream-processing-e4aeb6eaf4a3)

### Vídeos no YouTube

1. [Next-Gen, data-driven application development](https://youtube.com/watch?v=CqZYSpngFPo)
2. [Introduction to Data-Driven R&D](https://youtube.com/watch?v=cpvfA-jQLjE)
3. [Data-Driven Development in the Automotive Field](https://youtube.com/watch?v=SExQZna9x90)
4. ["Machine Programming & the Future of Data-Driven Software Development" by Justin Gottschlich](https://youtube.com/watch?v=ehpoAb6AFto)
5. [Data-Driven Agile: Embedding Data Quality in Software Development](https://youtube.com/watch?v=KzFGjxCxwtU)

### Artigos

1. [Undulate: A framework for data-driven software engineering enabling soft computing](https://www.sciencedirect.com/science/article/pii/S0950584922001549)
2. [Data-Driven Scientific Programming and Intelligent Application - Hindawi](https://www.hindawi.com/journals/sp/si/785759/)
3. [(PDF) Data-Driven Decisions and Actions in Today's Software Development - ResearchGate](https://www.researchgate.net/publication/325748524_Data-Driven_Decisions_and_Actions_in_Today's_Software_Development)
4. [Data Science and Analytics: An Overview from Data-Driven Smart Computing, Decision-Making and Applications Perspective - PMC - NCBI](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8274472/)
5. [Towards data-driven software engineering skills assessment](https://www.emerald.com/insight/content/doi/10.1108/IJCS-07-2018-0014/full/html)

### Livros

1. [Running Lean: Iterate from Plan A to a Plan That Works by Ash Maurya](https://www.amazon.com/Running-Lean-Iterate-Plan-Works/dp/1449305172)
2. [Defining Data-Driven Software Development - O'Reilly](https://www.oreilly.com/library/view/defining-data-driven-software/9781492049272/)
3. [Data-Oriented Programming: Reduce software complexity - Yehonathan Sharvit](https://www.amazon.com/Data-Oriented-Programming-Unlearning-Yehonathan-Sharvit/dp/1617298573)
4. [Data-oriented design: software engineering for limited resources and short schedules](https://www.amazon.com/Data-oriented-design-engineering-resources-schedules/dp/1916478700)
5. [Evidence-based Software Engineering: based on the publicly available data](http://knosof.co.uk/ESEUR/)

---

## Instruções passo a passo para desenvolver um aplicativo dirigido a dados simples usando Python e JavaScript

**Etapa 1: Definir o escopo e os requisitos do aplicativo**

- Definir claramente o objetivo e o escopo do aplicativo.
- Identificar os requisitos e funcionalidades específicas que a aplicação deverá ter.
- Determinar o público-alvo e as personas dos usuários.

**Etapa 2: projetar a arquitetura do aplicativo**

- Decidir sobre a arquitetura geral do aplicativo, considerando fatores como escalabilidade, desempenho e capacidade de manutenção.
- Escolha um padrão de arquitetura adequado, como Model-View-Controller (MVC) ou Microservices.
- Definir o fluxo de dados e as relações entre os diferentes componentes da aplicação.

**Etapa 3: configurar o ambiente de desenvolvimento**

- Instale ambientes de desenvolvimento Python e JavaScript em sua máquina.
- Configure um sistema de controle de versão como o Git para rastrear alterações em sua base de código.
- Crie um novo diretório de projeto e inicialize-o como um repositório Git.

**Etapa 4: escolha uma estrutura de back-end**

- Pesquise e selecione uma estrutura da web Python adequada, como Django, Flask ou Pyramid.
- Instale o framework escolhido e quaisquer dependências necessárias.
- Crie um novo projeto Django ou aplicativo Flask usando a interface de linha de comando do framework.

**Etapa 5: Crie o banco de dados**

- Decida a tecnologia de banco de dados a ser usada, como SQLite, MySQL ou PostgreSQL.
- Configure o banco de dados e defina as configurações de conexão em sua estrutura de back-end.
- Crie as tabelas ou modelos de banco de dados necessários com base nos requisitos de seu aplicativo.

**Etapa 6: implemente a lógica de back-end**

- Defina as rotas ou endpoints de URL para lidar com diferentes solicitações HTTP.
- Escreva a lógica de back-end para lidar com essas solicitações, incluindo recuperação, manipulação e armazenamento de dados.
- Implementar quaisquer mecanismos de autenticação ou autorização necessários.

*Etapa 7: Escolha um Frontend Framework**

- Pesquise e selecione uma estrutura de front-end JavaScript adequada, como React, Angular ou Vue.js.
- Instale o framework escolhido e quaisquer dependências necessárias.
- Configure o ambiente de desenvolvimento front-end usando ferramentas como npm ou yarn.

**Etapa 8: Projete a interface do usuário**

- Crie wireframes ou maquetes para visualizar a interface do usuário do seu aplicativo.
- Implemente o design da interface do usuário usando HTML, CSS e a estrutura de front-end escolhida.
- Garanta capacidade de resposta e acessibilidade da interface do usuário em diferentes dispositivos e navegadores.

**Etapa 9: Integre o back-end e o front-end**

- Conecte os componentes de front-end e back-end fazendo chamadas de API do front-end para o back-end.
- Implemente os endpoints necessários no back-end para lidar com essas solicitações de API.
- Teste a integração enviando solicitações do frontend e verificando as respostas.

**Etapa 10: Implemente a Visualização e Interação de Dados**

- Escolha bibliotecas ou estruturas adequadas para visualização de dados, como D3.js ou Chart.js.
- Integre as ferramentas de visualização de dados selecionadas em seu aplicativo front-end.
- Implemente recursos interativos como filtragem, classificação e pesquisa de dados.

**Etapa 11: Teste e depure o aplicativo**

- Escreva testes de unidade e testes de integração para garantir a exatidão do seu código.
- Use ferramentas e técnicas de depuração para identificar e corrigir quaisquer problemas ou erros.
- Realize testes completos em diferentes cenários e casos extremos.

**Etapa 12: implantar o aplicativo**

- Escolha uma plataforma de hospedagem ou servidor para implantar seu aplicativo, como Heroku, AWS ou DigitalOcean.
- Defina as configurações necessárias e implante seu código de back-end e front-end.
- Monitore o desempenho do aplicativo e resolva quaisquer problemas que possam surgir.

**Etapa 13: Documentar e manter a base de código**

- Escrever documentação para o aplicativo, incluindo instruções de instalação, diretrizes de uso e documentação da API.
- Mantenha uma base de código limpa e organizada seguindo as melhores práticas e padrões de codificação.
- Atualize regularmente as dependências e bibliotecas para garantir segurança e compatibilidade.
