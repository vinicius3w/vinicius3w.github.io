---
title:  "As dores que nos levam aos Estilos Arquiteturais"
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
  - software architecture
  - software quality
  - software engineer
  - architectural styles
  - layered architecture
  - client-server architecture
  - microservices
  - service-oriented architecture
  - event-driven architecture
---

Li um dia desses um tweet sobre o fato de que as dores do mundo real no ciclo de desenvolvimento que levam a criação de estilos arquiteturais. O tweet se perdeu na nova estrutura de timeline do Twitter (Pra você) mas ele me inspirou a falar um pouco sobre isso.

## Tudo começa pelo entendimento de "quem é o estilo arquitetural na fila do pão dos arquitetos"

A arquitetura de software é uma disciplina fundamental no desenvolvimento de sistemas e plataformas de soft1ware, responsável por definir a estrutura global do sistema/plataforma e as principais decisões de design que moldam suas características. Um dos principais desafios enfrentados pelos arquitetos de software é escolher o estilo arquitetural mais adequado para o sistema em questão, uma vez que diferentes estilos podem ter implicações significativas em termos de desempenho, segurança, escalabilidade e outras propriedades importantes.

## Como assim estilos arquiteturais?

Os estilos arquiteturais de software são conjuntos de princípios e padrões que orientam a organização e interação dos componentes de um sistema ou plataforma, bem como as decisões de design tomadas pelos arquitetos. Esses estilos surgiram como uma resposta a dores específicas enfrentadas pelos desenvolvedores de software, e foram estabelecidos no mercado como uma forma de lidar com essas dores de uma maneira mais eficiente e consistente.

Desde o início da minha carreira como engenheiro de software (ou designer de plataformas), sempre acreditei que a arquitetura é uma parte fundamental do processo de design de uma solução digital.

Cada estilo arquitetural tem suas próprias vantagens e desvantagens, e a escolha do estilo mais adequado para um determinado sistema/plataforma depende de vários fatores, como os requisitos de negócios, as limitações técnicas, a complexidade do sistema/plataforma e a experiência dos desenvolvedores. Além disso, é importante destacar que muitos sistemas/plataformas de software podem incorporar mais de um estilo arquitetural, dependendo das necessidades específicas de cada componente, módulo ou serviço.

## A jornada histórica dos estilos clássicos ao longo do tempo

Historicamente falando, os estilos arquiteturais de software têm evoluído ao longo do tempo, em resposta às mudanças nas demandas e tecnologias da indústria de software. O primeiro estilo arquitetural significativo foi a arquitetura em camadas (mais informações [aqui](https://bit.ly/3nU1twl) e [aqui](https://amzn.to/3nZ3eIR)), que surgiu na década de 1970, como uma forma de separar a lógica de negócios de um sistema da lógica de apresentação. Essa abordagem ajudou a reduzir a complexidade e aumentar a modularidade dos sistemas, além de melhorar a [manutenção](https://bit.ly/403eUrg) e a [reutilização de código](https://bit.ly/400gt9x). No entanto, a arquitetura em camadas pode levar a um acoplamento excessivo entre as camadas e pode não ser adequada para sistemas com requisitos de desempenho muito altos.

Outro estilo arquitetural importante que surgiu na década de 1970 foi a arquitetura cliente-servidor (mais informações [aqui](https://bit.ly/3zMuGfw) e [aqui](https://amzn.to/3Mq14fw)), que dividia o sistema em duas partes principais: o cliente, que interagia com o usuário final, e o servidor, que fornecia os serviços e recursos necessários para o sistema funcionar. Essa abordagem foi motivada pela necessidade de lidar com a crescente complexidade dos sistemas de software e a necessidade de distribuição e compartilhamento de recursos. Essa abordagem pode ser eficaz em sistemas distribuídos e escaláveis, mas pode ser mais complexa de implementar e gerenciar do que outros estilos arquiteturais.

Mais recentemente, a [arquitetura orientada a serviços](https://amzn.to/41gS0O2) e a arquitetura baseada em microsserviços (mais informações [aqui](https://bit.ly/41iqPmf) e [aqui](https://amzn.to/3Ul8oel)) surgiram como resposta a dores específicas, como a dificuldade de integrar sistemas heterogêneos e a complexidade de se coordenar equipes grandes em projetos complexos, respectivamente. A arquitetura orientada a serviços enfatiza a modularidade e a reutilização de componentes de software, bem como a interoperabilidade entre diferentes sistemas, enquanto a [arquitetura baseada em microsserviços](hyyps://bit.ly/vcg-microservices) enfatiza a divisão do sistema em serviços menores e independentes, cada um executando em seu próprio processo, o que ajuda a melhorar a escalabilidade e a flexibilidade do sistema. Isso tudo pode tornar o sistema mais flexível e adaptável a mudanças, mas também pode aumentar a complexidade e o tempo de resposta do sistema.

O que está no "hype" atualmente é a arquitetura baseada ou dirigida a eventos (do inglês, _Event-Driven Architecture_ - EDA). A arquitetura baseada em eventos é um estilo arquitetural em que a comunicação entre os componentes do sistema/plataforma é baseada na troca de eventos assíncronos. Em um sistema/plataforma EDA, um evento é uma notificação assíncrona de que algo aconteceu em algum lugar do sistema/plataforma. O sistema/plataforma pode ser composto por diversos componentes, como serviços, aplicativos, bancos de dados, dispositivos IoT, entre outros, que podem gerar e/ou consumir eventos.

A principal vantagem da arquitetura baseada em eventos é que ela permite que o sistema/plataforma seja altamente distribuído e escalável, sem depender de uma arquitetura centralizada de troca de mensagens. Isso significa que os componentes do sistema/plataforma podem se comunicar diretamente uns com os outros através da troca de eventos, sem depender de um intermediário ou de um ponto de coordenação centralizado.

Além disso, a arquitetura baseada em eventos é muito útil em cenários em que os eventos são importantes para o negócio, como em sistemas de processamento de pagamentos, sistemas de logística, sistemas de monitoramento e controle de produção, entre outros. Isso porque a troca de eventos permite que o sistema reaja de forma rápida e eficiente às mudanças de estado e às ações dos usuários ou de outros sistemas.

No entanto, a implementação de uma arquitetura baseada em eventos pode ser complexa, especialmente em sistemas/plataforma que envolvem muitos componentes e eventos diferentes. É importante projetar cuidadosamente o sistema/plataforma, definir padrões de eventos e implementar mecanismos de tratamento de erros para garantir a integridade do sistema.

Para aprender mais sobre a arquitetura baseada em eventos, eu recomendo a leitura do livro ["Building Event-Driven Microservices" de Adam Bellemare](https://bit.ly/3GxkR97), que fornece uma introdução detalhada sobre a arquitetura baseada em eventos e sua implementação em sistemas/plataforma de microsserviços.

## Fica, vai ter bolo!

Os estilos arquiteturais são uma área fascinante e dinâmica da indústria de software, que constantemente evolui e se adapta para atender às demandas cada vez mais complexas e desafiadoras da tecnologia moderna. Ao explorar os diferentes estilos arquiteturais, você descobrirá como eles surgiram a partir de dores específicas enfrentadas pelos desenvolvedores e arquitetos de software, e como eles oferecem vantagens e desvantagens únicas em diferentes cenários.

Ao mergulhar em cada estilo arquitetural, você terá a oportunidade de aprimorar suas habilidades de tomada de decisão, aprendendo a escolher o estilo mais adequado para um determinado sistema/plataforma com base nos requisitos de negócios, nas limitações técnicas, na complexidade do sistema/plataforma e na experiência dos desenvolvedores.

Aprender sobre os estilos arquiteturais de software é uma jornada emocionante e desafiadora, mas que traz inúmeros benefícios para sua carreira como desenvolvedor ou arquiteto de software. Então não perca tempo e comece agora mesmo a explorar as diferentes possibilidades que os estilos arquiteturais têm a oferecer!
