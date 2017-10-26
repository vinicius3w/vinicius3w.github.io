---
title:  "Ensinando Engenharia de Software na Prática, Parte I"
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
  - swebok
  - soa
  - software testing
---
Dando continuidade no tema de _Educação em Engenharia de Software_ ou_ Como formar Capital Humano **EFICIENTE** em Produção de Software_, vem o segundo post da série. O primeiro você pode conferir aqui: [A biblioteca do Desenvolvedor de Software dos dias de hoje](https://viniciusgarcia.com/2014/02/14/a-biblioteca-do-desenvolvedor-de-software-dos-dias-de-hoje/).

Eu sou professor de Engenharia de Software há alguns anos… especificamente no [Centro de Informática](http://www.cin.ufpe.br/) da [UFPE](http://www.ufpe.br/), desde o primeiro semestre de 2012.

A primeira experiência pode ser vista neste [link](https://viniciusgarcia.com/courses/if977/). Aqui a ideia já veio de experiências prévias em disciplinas na UPE, no Mestrado Profissional do [CESAR.EDU](http://www.cesar.edu.br/newsite/) e de apoio a disciplinas da pós-graduação do CIn, em especial:

- IN0953 – Engenharia de Software, junto com o prof. Silvio Meira
- IN1163 – Tópicos Avançados em Desenvolvimento de Software de Código Aberto, conduzida com o pessoal do [RiSE](https://wordpress.dcc.ufba.br/riselabs/)

A experiência nestas disciplinas foi plenamente prática, com um esforço na implantação de técnicas baseadas em PBL ([_Problem-Based Learning_](http://en.wikipedia.org/wiki/Problem-based_learning)). Na primeira experiência de ES no curso de Sistemas de Informação, a intenção foi a mesma, com foco na resolução de problemas ao invés de _um monte_ de slides com teorias, puramente.

Todos os tópicos teóricos do curso giravam em torno da execução de um projeto em equipe que devia ser desenvolvido em iterações (quatro para ser mais exato).

Para começar, era feito uma imersão nos conceitos básicos e fundamentais da Engenharia de Software, mais especificamente no que é Software, o que é Engenharia, como se dá a Engenharia de algo tão complexo e diferente que é o Software e tudo o que cerca esse processo produtivo. Uma das perguntas que faço sempre aos alunos é: _como eu defino o preço do meu software?_

Em seguida, uma discussão acerca das Fábricas de Software, desde as clássicas até os modelos mais “diversos” existentes hoje… como se dão, o que são, por que são… qual o princípio e necessidade de existir uma comunidade ao redor desse ciclo de desenvolvimento, onde entra o software livre… Claro, a leitura e discussão do clássico [The Cathedral and the Bazaar](http://catb.org/~esr/writings/cathedral-bazaar/cathedral-bazaar/) é obrigatória!

A definição do projeto, contra a minha real vontade, sempre ficou a cargo dos alunos. Como era difícil conseguir projetos reais ou mais próximos do mundo real (por uma série de questões, mas a principal é falta de tempo do professor – entidade única envolvida na disciplina, uma vez que os monitores são apoio e normalmente são alunos que acabaram de cursar a disciplina) a abordagem era estimular a descoberta de oportunidades de negócios, aproveitando todo o caráter inovador e empreendedor que o CIn tem em seu DNA.

Tivemos excelentes resultados e resultados nem tão significativos… mas acredito que no final o saldo é positivo. A partir da segunda rodada da disciplina, ou seja, de 2012.2 resolvemos promover duas integrações, digamos assim.

A primeira foi **horizontal** e teve por objetivo tratar o currículo de Engenharia de Software que acreditamos ser o ideal no CIn. Então por uma iniciativa dos professores de ES dos três cursos de graduação do centro (Ciência da Computação, Engenharia da Computação e Sistemas de Informação) tentamos encontrar o que seria o _core_ de ES e compartilhamos tudo referente a este núcleo. A metodologia, critérios, artefatos e _templates_, políticas e métodos de avaliações, enfim, buscamos montar um framework para somente acrescentarmos o que seria específico e necessário em cada curso. Daí nasceu essa primeira integração, disponível neste site: [Engenharia de Software e Sistemas](https://sites.google.com/a/cin.ufpe.br/if682/).

A segunda integração ocorreu de maneira **vertical**, ou seja, dentro do curso de Sistemas de Informação e buscamos uniformizar o conhecimento, a metodologia, os tópicos cobertos e até mesmo os projetos que deveriam ser executados nas disciplinas intimamente relacionadas:

- [IF977 – Engenharia de Software](http://www.cin.ufpe.br/~if977)
- [IF976 – Banco de Dados](http://www.cin.ufpe.br/~if976)
- IF979 – Planejamento e Gerenciamento de Projetos

Até o presente momento estas três disciplinas tem rodado ainda desta forma. Não ocorreram mais conversas ou atualizações horizontais entre as disciplinas de Engenharia de Software.

Após estes 4 semestres ministrando a disciplina e vendo as deficiências deste modelo, pontos de melhoria e a carência do [Arranjo Produtivo Local](http://www.portodigital.org/), num primeiro momento, e a carência nacional e mão de obra em produção de software, me senti motivado a fazer uma reengenharia desta disciplina e é esta reengenharia que eu vou ir apresentando aos poucos aqui.

Para começar, resolvi me inspirar no curso [CS 169 Software Engineering](https://sites.google.com/site/ucbsaas/) da [UC Berkeley](http://www.berkeley.edu/index.html). O curso tem um formato também já focado na prática, que gira em torno do uso das próprias metodologias ágeis na condução do curso em si bem como da aplicação de conceitos e tópicos da ES em um projeto executado por pequenos times formados pelos alunos.

Além disso, ele está plenamente de acordo com as novas plataformas de software e serviços, utiliza conceitos e recursos de _Software as a Service_ e [_Cloud Computing_](http://www.nist.gov/itl/cloud/) e preocupações com o projeto, atenção aos objetivos de negócios, entrega de [MVP](http://en.wikipedia.org/wiki/Minimum_viable_product) e exercitar mais uma vez a prática da programação, que no caso do curso de Sistemas da Informação é um pouco deficiente, na minha humilde opinião.

O cerne do curso vai continuar sendo o [Software Engineering Body of Knowledge (SWEBOK)](http://www.computer.org/portal/web/swebok) mas as novas tecnologias, metodologias e eventualmente ferramentas vão fazer parte do convívio dos alunos no curso.

A intenção principal é trabalhar a lacuna existente entre o que a **academia acredita** que deveriam ser cobertos em cursos de ES e o que a **indústria quer** ver nos alunos formados por estes cursos. As empresas não querem que as universidades se transformem em escolas profissionalizantes que ensinam tecnologias, ferramentas, linguagens ou _frameworks_ específicos; elas querem habilidades que transcendem estas “_coisas_“, incluindo lidar com código legado e trabalhar em equipe para atender a um cliente que não fala o “_computês_“.

Nos próximos posts vou apresentando este novo projeto que espero servir de estímulo para mais reengenharia em disciplinas de Engenharia de Software em outras instituições.
