---
title:  "Ensinando Engenharia de Software na Prática, Parte II"
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
  - saas
  - soa
  - swebok
  - software testing
---

Depois de alguns meses entretido com outros desafios, minhas atenções voltaram para a construção da nova abordagem de abordar _Educação em Engenharia de Software_ ou_ Como formar Capital Humano **EFICIENTE** em Produção de Software._

No primeiro post da série, tratei do que eu considero como [A biblioteca do Desenvolvedor de Software dos dias de hoje](https://viniciusgarcia.com/2014/02/14/a-biblioteca-do-desenvolvedor-de-software-dos-dias-de-hoje/). Diversos temas (ou verticais) foram destacados com algumas sugestões de bons (ótimos?) livros que abordam estes problemas de maneira didática, prática e objetiva.

No segundo post da série, comecei a tratar do desafio [Ensinando Engenharia de Software na Prática, Parte I](https://viniciusgarcia.com/2014/02/19/ensinando-engenharia-de-software-na-pratica-parte-i/). Nele fiz uma contextualização das experiências e desafios que vivi tentando ensinar/vivenciar a engenharia de software na academia, ou melhor, tentando levar o **estado da arte para o estado da prática**. Adicionalmente, as bases desta nova abordagem que estou desenhando para a formação de capital humano em engenharia de software começaram a ser estabelecidas.

Depois destas discussões o desafio foi conseguir estruturar um ciclo de vida do conhecimento a ser apresentado e evoluído dentro de um período de um semestre letivo, que na prática são uns 4 meses. Estes meses frequentemente sofrem interrupções na sua continuidade devidos a feriados, catástrofes naturais (aqui em Recife temos sérios problemas com chuvas), Copa do Mundo (como neste ano) e por aí vai. Mas até que nada disso compromete, efetivamente, a continuidade e sobrevivência do curso em si.

Isso tudo passa, inicialmente, pela (re)definição da ementa do curso. Segundo a [Wikipedia](http://pt.wikipedia.org/wiki/Ementa), **Ementa** é

> (do latim ementum, “pensamento”, “ideia”, de e e mens, “juízo”, “razão”, “mente”) é um termo aplicado de modo geral, para indicar uma espécie de apontamento ou anotação tomada para lembrança, a fim de que, por aí, se produza depois o documento escrito, para que se faça e se execute o ato nela lembrado. Por exemplo, é a decisão resumida das matérias e suas cargas horárias dadas numa faculdade.

> Uma ementa universitária, em geral, apresenta muito sucintamente as idéias gerais que serão abordadas ao longo da disciplina, como forma de um fichamento (frases soltas, de forma bem sintética). A apresentação mais detalhada dos assuntos que serão estudados, ponto a ponto, é dada no programa de curso.

A ementa atual do curso (até 2014.1) é a que se segue:

> Engenharia de Software não é só desenvolvimento de software. Ou seja, não é somente a atividade de programar e conhecer linguagens e ferramentas de apoio à programação. Existem uma série de processos envolvidos que colaboram na “construção” de um produto de software, desde a especificação do projeto, seu planejamento de execução, desenvolvimento, testes, manutenção e evolução. Portanto, Engenharia de Software claramente não se trata apenas de programação, uma atividade que pode ser desenvolvida de forma independente de outras pessoas, mas sim de um conjunto de atividades, tarefas e mais ainda, papéis que requerem trabalho em equipe (social) e capacidade de comunicação (socialização). Neste curso, vamos estudar princípios da Engenharia de Software, seus objetivos, atividades, papéis, recursos, como planejar um projeto, descobrir requisitos, abstrair uma proposta de construção de um produto de software e apresentar uma solução que será construída de forma iterativa, bem como a continuidade da vida útil deste produto.

Analisando-a friamente, ela é até bem mais adequada do que _**MUITAS**_ ementas encontradas por aí… o que não é surpresa, dado o caráter diferencial da forma como a disciplina é vivenciada. Entretanto, conforme já foi discutido até então, uma **_reengenharia_** no curso se mostrou necessária e, consequentemente, a ementa foi revista. A nova ementa é

> Hoje a Engenharia de Software não é só desenvolvimento de software ou de um **Software as a Service** (**SaaS**). Ou seja, não é somente a atividade de programar e conhecer linguagens e ferramentas de apoio à programação. Existem uma série de processos envolvidos que colaboram na “construção” de um produto de software, desde a especificação do projeto, seu planejamento de execução, desenvolvimento, testes, manutenção e evolução porque um software ou SaaS não tem vida curta. Portanto, Engenharia de Software claramente não se trata apenas de programação, uma atividade que pode ser desenvolvida de forma independente de outras pessoas, mas sim de um conjunto de atividades, tarefas e mais ainda, papéis que requerem trabalho em equipe (social) e capacidade de comunicação (socialização).  
Neste curso, vamos estudar princípios da Engenharia de Software através de técnicas ágeis altamente produtivas para desenvolver sistemas de informação na forma de SaaS. Espera-se que os alunos se deparem e compreendam os novos desafios e oportunidades de SaaS versus software empacotados por meio da aplicação de técnicas de desenvolvimento fundamentais para a concepção, análise, projeto, implementação, teste e implantação de um sistema de informação SaaS simples.

É importante ressaltar que esta é uma das **poucas** disciplinas do curso de SI que possibilita ao aluno **um contato mais próximo e prático** com as disciplinas relacionadas ao **desenvolvimento de software propriamente dito**, uma clara carência não só deste curso mas uma necessidade real do mercado de TI nacional e com muitas posições de trabalho em aberto o que demonstra uma clara carência de capital humano especializado.

É sabido que uma imersão **prática** em Engenharia de Software em um curso semestral (em torno de 15 semanas) com _Exercícios Escolares _intercalados, necessidades de aulas práticas de monitoria, revisões e um significativo projeto em times com data limite para conclusão é uma meta bastante ambiciosa.

Neste contexto, espera-se que os estudantes, para cursar esta disciplina com sucesso, estejam confortáveis com _pelo menos uma linguagem de programação Orientada a Objetos_ e com os _conceitos básicos da Orientação a Objetos_ (classes, herança, polimorfismo, sobrecarga, entre outros) e _conceitos básicos de abstração e estrutura de dados_ (abstração de dados, abstrações de procedimentos / funções de alta ordem, recursão, tipos abstratos de dados, entre outros).

Antes desta disciplina, é importante ressaltar que os alunos de SI do CIn cursam “_IF966 INTRODUÇÃO AOS SISTEMAS DE INFORMAÇÃO_” (pré-requisito) que introduz os alunos aos principais conceitos e fundamentos dos Sistemas de Informação e da Tecnologia da Informação e Comunicação; “_IF968 PROGRAMAÇÃO 1_” (pré-requisito) que aborda os conceitos básicos de algoritmos, estruturas de dados dinâmicas, técnicas de construção de algoritmos e alguns breves conceitos de complexidade de algoritmos, usualmente em Java mas com experiências feitas utilizando Python (são duas turmas, onde a turma com os “reprovados” trabalham com Python como uma experiência em verificar qual o impacto de já iniciar com Java e suas complexidades atrapalha na absorção do conteúdo); e, “_IF969 ALGORITMOS E ESTRUTURA DE DADOS_” (obrigatória do curso) utilizando Java que conforme o nome diz, trata dos algoritmos e estruturas de dados. A IF968 e a IF969 são as únicas disciplinas do curso que tratam de algoritmos e programação e juntamente com a IF977 formam a trilha de disciplinas obrigatórias para trabalhar o desenvolvimento de software propriamente dito.

Existem ainda disciplina (co)relacionadas como:

- “IF976 – BANCO DE DADOS”
- “IF979 – PLANEJAMENTO E GERENCIAMENTO DE PROJETOS”
- “IF978 – GESTÃO DE PROCESSOS DE NEGÓCIO”

No próximo post tratarei do projeto propriamente dito do curso, ou seja, o programa da disciplina. Quais os principais temas, como eles serão tratados, o ciclo de vida do conhecimento dentro do framework do curso e o que eu imagino enfrentar de desafios e os riscos envolvidos!

Espero não demorar tanto para o próximo post, mesmo porque o semestre atual está no fim e a disciplina tem que ficar pronta logo!
