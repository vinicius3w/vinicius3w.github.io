---
title:  "Ensinando Engenharia de Software na Prática, Parte IV"
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

No [artigo anterior](https://viniciusgarcia.me/education/ensinando-engenharia-de-software-na-pratica-parte-iii/) eu comecei a discussão acerca da necessidade de evolução da [disciplina de Engenharia de Software sob a minha responsabilidade](https://bit.ly/vcg-es), no [curso de Sistemas de Informação](https://portal.cin.ufpe.br/graduacao/sistemas-de-informacao/) do [Centro de Informática de UFPE](https://www.cin.ufpe.br/).

Este disciplina é focada no ensino de engenharia de software **na prática**. O objetivo é atacar os desafios do ensino da engenharia de software no meio acadêmico e como habilitar efetivamente os desenvolvedores de software para um mundo globalizado e em constante evolucão e necessitado de [software cada vez mais complexos e de larga escala](https://doi.org/10.1145/2209249.2209268).

## Educação em Engenharia de Software

Lembrando que a educação em engenharia de software é um campo de estudo que se concentra na preparação de profissionais para carreiras nas indústrias de desenvolvimento, gerenciamento e manutenção de software. Inclui cursos em informática, programação e matemática, bem como disciplinas mais especializadas como projeto de software, metodologias de desenvolvimento e testes.

Essa **educação em engenharia de software** pode assumir muitas formas, incluindo programas tradicionais de graduação, programas de ensino on-line e a distância, e cursos e certificações mais especializados. Estes programas podem variar em termos de seu foco (_conforme até falei um pouco também no artigo passado_), com alguns fornecendo uma educação mais geral em princípios e práticas de engenharia de software, enquanto outros permitem que os estudantes se especializem em uma área específica, como o desenvolvimento de aplicativos móveis, sistemas de informação ou cibersegurança.

Muitos destes programas de educação em engenharia de software também incluem estágios ou treinamentos práticos como parte do currículo (às vezes vinculados a programas/projetos/cursos de extensão atrelados a própia matriz curricular - _estamos trabalhando nisso lá no CIn, inclusive_), o que pode proporcionar aos estudantes uma **valiosa experiência no mundo real** e ajudá-los a construir suas redes profissionais desenvolvendo habilidades e capacidades que provavelmente não teriam como trabalhar em uma jornada apenas dentro de uma sala  de aula, em ambiente controlado (como num tubo de ensaio).

O campo da educação em engenharia de software está em constante evolução, e novas tecnologias e técnicas estão sendo desenvolvidas o tempo todo. Como resultado, é importante que os profissionais da área se mantenham atualizados com os últimos desenvolvimentos e melhores práticas, a fim de evoluir suas habilidades e permanecer competitivos no mercado de trabalho. Mas, conforme também já discutido, além das evoluções em metodologias e estratégias para se ensinar e aprender a engenharia de software, temos a própria **evolução da engenharia de software** (seus métodos, processos e ferramentas - para dizer o mínimo), que é o foco destas _"mal traçadas linhas"_.

Vou então tentar começar a destrinchar algumas dessas novas percepções sobre a engenharia de software e suas, _"veja bem"_, ramificações (me segurei para não dizer especializações).

## Engenharia de Produtos de Software versus Arquitetura de Software

[Engenharia de produto de software](https://erngui.com/misc/design-factory.html#:~:text=Managing%20The%20Design%20Factory%201%20let%20your%20decisions,what%20needs%20controlling%29%204%20design%20is%20information%20generation) (do inglês _Software product engineering_ ou SPE) é o processo de criação de um **produto de software**, desde a concepção inicial da idéia até o lançamento final do produto. Envolve a **aplicação de princípios e práticas de engenharia** para a **criação de software**, a fim de produzir produtos de software de **alta qualidade, confiáveis e de fácil manutenção**.

A SPE envolve uma série de atividades, incluindo coleta e análise de requisitos, projeto e implementação, teste e depuração, e implantação e manutenção. Ela envolve o uso de várias ferramentas e técnicas, tais como sistemas de controle de versão, ferramentas de depuração e estruturas de teste, para apoiar o processo de desenvolvimento de software. Também envolve colaboração e comunicação com membros da equipe e stakeholders em geral, a fim de garantir que o produto de software atenda às necessidades de seus usuários.

A SPE é um campo importante dentro da engenharia de software que ajuda as organizações a **desenvolver produtos de software de alta qualidade**. Em resumo, podemos destacar que algumas das principais características da SPE incluem:

- **O uso de princípios e práticas de engenharia de software** para garantir a qualidade e a confiabilidade do produto de software.
- Envolve a **coleta e análise de requisitos** e concentra-se em atender as necessidades dos usuários e stakeholders do produto de software.
- Envolve o **uso de várias ferramentas e técnicas**, tais como sistemas de controle de versão, ferramentas de depuração e estruturas de teste, para apoiar o processo de desenvolvimento de software.
- Envolve **colaboração e comunicação** com membros da equipe e partes interessadas, a fim de garantir que o produto de software atenda às necessidades de seus usuários.
- Frequentemente envolve um **processo de desenvolvimento iterativo**, no qual o produto é **desenvolvido e testado em etapas incrementais**, com **feedback e ajustes** feitos em cada etapa.
- Envolve **esforços contínuos para melhorar** o produto de software, por exemplo, através da implementação de novos recursos e da resolução de problemas.

Por sua vez, a [arquitetura de software](https://en.wikipedia.org/wiki/Software_architecture) (do inglês _Software Architecture_ ou SA) é a estrutura de alto nível de um sistema de software, que define o projeto geral e a organização desse sistema. Ela inclui os componentes do sistema, suas relações e interações, restrições e os princípios e diretrizes que regem seu projeto e evolução.

A SA está preocupada com o panorama geral de um sistema de software, e como ele é **organizado e estruturado** para atender às necessidades de seus usuários dentro dos níveis de qualidade estabelecidos e priorizados.

A SA é um fator importante no desenvolvimento de um sistema de software, pois tem um impacto significativo na capacidade de manutenção, escalabilidade e outros importantes atributos de qualidade do sistema. É frequentemente definida no início do processo de desenvolvimento do software e serve como um plano para o resto do desenvolvimento e deve ser constantemente [re]avaliada e evoluída.

Há vários princípios-chave que são importantes em uma SA. [**Modularidade**](https://en.wikipedia.org/wiki/Modularity) refere-se à idéia de dividir um sistema de software em componentes menores, auto-contidos, cada um com uma interface bem definida. Isto facilita a compreensão, manutenção e evolução do sistema. A [**separação das preocupações**](https://en.wikipedia.org/wiki/Separation_of_concerns) refere-se à idéia de dividir o sistema em componentes, cada um responsável por um aspecto específico do sistema. Isto ajuda a tornar o sistema mais fácil de entender e modificar. [**Reutilização**](https://en.wikipedia.org/wiki/Reusability) refere-se à capacidade de reutilizar componentes em diferentes contextos, o que pode ajudar a reduzir o tempo e os custos de desenvolvimento. [**Escalabilidade**](https://en.wikipedia.org/wiki/Scalability) refere-se à capacidade do sistema de lidar com o aumento do tráfego e do uso sem ter problemas de desempenho.

Além disso, ela também frequentemente faz uso de [**padrões de projeto**](https://en.wikipedia.org/wiki/Design_Patterns), que são soluções reutilizáveis para problemas comuns de projeto. Pode ser baseado em um estilo arquitetônico particular, como uma arquitetura [cliente-servidor](https://en.wikipedia.org/wiki/Client%E2%80%93server_model) ou uma arquitetura baseada em [microsserviços](https://en.wikipedia.org/wiki/Microservices), que define a estrutura geral do sistema. Deve considerar uma variedade de atributos de qualidade, tais como desempenho, segurança e usabilidade, a fim de garantir que o sistema atenda às necessidades de seus usuários. E envolve fazer concessões entre diferentes escolhas de projeto, tais como entre flexibilidade e desempenho ou entre complexidade e simplicidade.

Há também uma série de questões que são comumente encontradas na SA. Manter um **equilíbrio entre objetivos de curto e longo prazo é importante**, assim como assegurar que a arquitetura esteja alinhada com os **objetivos comerciais**. O gerenciamento do [débito técnico](https://en.wikipedia.org/wiki/Technical_debt) também é crucial, pois pode levar a problemas com a manutenção e escalabilidade do sistema se não for gerenciado cuidadosamente. E lidar com a mudança de requisitos é um desafio comum, pois as necessidades do sistema e de seus usuários podem mudar com o tempo.

### Diferenças

Uma diferença fundamental entre os dois campos pode ser vista sob três perspectivas: escopo, foco e atividades. 

Escopo: A SPE é um campo amplo que abrange todo o processo de criação de um produto de software, desde a concepção inicial da idéia até o lançamento final do produto. Envolve a aplicação de princípios e práticas de engenharia à criação de software, a fim de produzir produtos de software de alta qualidade, confiáveis e de fácil manutenção. A SA, por outro lado, é um campo mais especializado que se preocupa com a estrutura e organização de alto nível de um sistema de software. Ela inclui os componentes do sistema, suas relações e interações, e os princípios e diretrizes que regem seu projeto e evolução.

Foco: A SPE está focada em atender as necessidades dos usuários e partes interessadas do produto de software. Envolve a coleta e análise dos requisitos, projetando e implementando o produto, testando-o e depurando-o, e implantando-o e mantendo-o. O objetivo da SPE é produzir um produto de software que atenda às necessidades de seus usuários e partes interessadas. A SA, por outro lado, está focada em definir o projeto e a organização geral do sistema. Ela envolve a definição dos componentes e relações do sistema, assim como os princípios e diretrizes que regem seu projeto e evolução. O objetivo da SA é criar um sistema que seja bem organizado, escalável e de fácil manutenção.

Atividades: A engenharia de produtos de software envolve uma ampla gama de atividades, incluindo coleta e análise de requisitos, projeto e implementação, testes e depuração, e implantação e manutenção. Envolve trabalhar com uma equipe de desenvolvedores para criar o produto de software e colaborar com as partes interessadas para garantir que o produto atenda às necessidades de seus usuários. A arquitetura de software envolve a definição dos componentes e relações do sistema, assim como os princípios e diretrizes que regem seu projeto e evolução. 

### Similaridades

Tanto a SE quanto a SA envolvem o uso de princípios e práticas de engenharia a fim de garantir a qualidade e a confiabilidade do sistema. Isto pode incluir o uso das melhores práticas como testes, depuração e revisão de código para garantir que o sistema seja de alta qualidade.

Ambos os campos envolvem o uso de várias ferramentas e técnicas para apoiar o processo de desenvolvimento. Isto pode incluir sistemas de controle de versão, ferramentas de depuração, estruturas de teste e outras ferramentas que são usadas para gerenciar e apoiar o processo de desenvolvimento.

E, finalmente, ambos os campos envolvem colaboração e comunicação com membros da equipe e stakeholders, a fim de garantir que as necessidades dos usuários sejam atendidas. Isto pode envolver trabalhar com outros desenvolvedores para projetar e implementar o sistema, e se comunicar com os stakeholders para garantir que suas necessidades estejam sendo atendidas.

## E agora, onde estamos e para onde vamos?

Engenharia de Software é uma área de estudo que se concentra no design, desenvolvimento e manutenção de sistemas de software. Engenharia de Produto de Software é uma área relacionada que se concentra no gerenciamento do ciclo de vida de um produto de software, desde a concepção até o lançamento. Arquitetura de Software, por sua vez, é uma área mais especializada que se concentra na estrutura e organização de um sistema de software. Todas essas áreas são importantes para o desenvolvimento de software de qualidade e confiável.

Além destas duas áreas dentro da engenharia de software também temos a engenharia de plataforma. Em resumo, a [engenharia de plataforma](https://en.wikipedia.org/wiki/Product-family_engineering) é uma área da engenharia de software que se concentra no design, desenvolvimento e manutenção de plataformas, que são definidas como a base ou infraestrutura subjacente de um sistema de software. A engenharia de plataforma é importante porque as plataformas são a base sobre a qual os sistemas de software são construídos, e é crucial que essas plataformas sejam bem projetadas, desenvolvidas e mantidas. 

No próximo artigo, vou buscar explorar em mais detalhes o que é essa tal engenharia de plataforma, quais são os principais desafios e práticas envolvidas e como os engenheiros de plataforma atuam no processo de desenvolvimento de software.