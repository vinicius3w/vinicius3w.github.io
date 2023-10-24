---
title:  "A Magia do Design Orientado ao Domínio: Uma Jornada ao Coração do Desenvolvimento de Software"
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
  - technical debt
  - best practices
  - software development
  - project lifecycle
  - code sustainability
  - documentation
  - design patterns
  - lessons learned
  - success stories
  - ddd
  - domain oriented design
  - technology
---

Era uma vez, no multiverso do desenvolvimento de software, surgiu um conceito prometendo revolucionar a maneira como pensamos e construímos software. Este conceito foi chamado de [Design Orientado ao Domínio (DDD)](https://martinfowler.com/bliki/DomainDrivenDesign.html) (do inglês *[Domain-Driven Design](https://www.oreilly.com/library/view/domain-driven-design-tackling/0321125215/)*). Mas o que é o Design Orientado ao Domínio, você me pergunta? E por que você, como desenvolvedor (ou profissional) de software, deveria se importar com isso?

É o que eu tento responder - ou seria chamar a atenção!? - para a "magia" do DDD e mostrar como ele pode transformar a maneira como construímos software. E vou logo avisando, tem viés nesse texto porque eu sou um confesso admirador do trabalho do [Eric Evans](https://en.wikipedia.org/wiki/Domain-driven_design).

## O Conto de Dois Mundos: Negócios e Software

Vamos imaginar um universo - do portfólio de universos que temos no multiverso - em que você é um desenvolvedor de software trabalhando em um projeto para uma instituição financeira. Você tem a tarefa de construir um sistema para gerenciar transações, contas e clientes. Mas tem um detalhe, os especialistas de negócios falam uma língua diferente, repleta de termos como "débito", "crédito", "razão" e "saldo". Por outro lado, você, como desenvolvedor, pensa em termos de classes, objetos, métodos e bancos de dados. Como você faz a ponte entre essas diferenças?

É aqui que o Design Orientado ao Domínio entra em jogo. O DDD é uma **abordagem de desenvolvimento de software** que se concentra na construção de software que **reflete a realidade do domínio de negócios**. Trata-se de criar uma linguagem comum, um modelo compartilhado que ambos, especialistas de negócios e desenvolvedores, podem entender e usar para se comunicar **E-F-E-T-I-V-A-M-E-N-T-E**.

## Os Blocos de Construção do DDD

O DDD não é apenas um conceito, é uma coleção de práticas e padrões que nos orientam na concepção e implementação de software. A seguir eu listo alguns desses blocos de construção.

### Linguagem Ubíqua

Você já se perdeu na tradução? No DDD, a Linguagem Ubíqua é a linguagem compartilhada entre desenvolvedores e especialistas do domínio. É a linguagem usada em todas as discussões, diagramas e até mesmo no próprio código.

Podemos dizer que ela pode ser considerada a [**pedra angular**](https://bit.ly/3JGcYzR) do DDD. Trata-se de **um conjunto comum de termos e definições usados por todas as partes interessadas de um projeto**. Esta linguagem compartilhada promove a clareza e a compreensão entre todos, ajudando a prevenir mal-entendidos e conflitos que podem surgir de ambiguidades linguísticas.

**É a ponte que conecta o mundo dos negócios ao mundo do software.**

A importância da Linguagem Ubíqua se estende para além das discussões e documentações, também permeando o **código base**. O código que utiliza a Linguagem Ubíqua é mais fácil de entender e manter, pois reflete o domínio do negócio de uma maneira que todos os envolvidos podem compreender.

### Contexto Delimitado

Imagine tentar entender o universo inteiro de uma vez. Assustador, não é? O mesmo vale para sistemas de software complexos. O DDD introduz o conceito de Contexto Delimitado, que é uma maneira de dividir um grande sistema em partes gerenciáveis, cada uma com sua própria Linguagem Ubíqua e modelo.

O Contexto Delimitado é um componente essencial do DDD justamente porque ele ajuda a **gerenciar essa complexidade** em sistemas de software grandes e complexos. Dentro de um sistema, pode haver várias partes distintas ou subdomínios, cada um com seu próprio modelo e Linguagem Ubíqua. Um Contexto Delimitado serve para definir os limites dentro dos quais um modelo particular e sua Linguagem Ubíqua se aplicam.

A aplicação correta de Contextos Delimitados ajuda a evitar a poluição do modelo e a confusão linguística. Também promove um design de software mais modular, onde cada Contexto Delimitado pode ser desenvolvido, testado e implantado de forma independente.

### Entidades, Objetos de Valor e Agregados

No mundo do DDD, modelamos o domínio usando **Entidades**, **Objetos de Valor** e os **Agregados**.

**Entidades**: São objetos que têm uma identidade distinta e contínua ao longo do tempo, mesmo que suas propriedades possam mudar. Exemplos comuns são os usuários, contas ou pedidos em um sistema.

**Objetos de Valor**: São objetos que são definidos por seus atributos e não têm uma identidade distinta. Eles são frequentemente usados para representar conceitos simples e quantificáveis, como uma data, um endereço ou uma quantidade de dinheiro.

**Agregados**: São clusters de Entidades e Objetos de Valor que são tratados como uma única unidade. Um Agregado tem uma Entidade raiz, e a regra geral é que qualquer interação com o Agregado deve passar por essa Entidade raiz. Isso ajuda a manter a consistência e a integridade do Agregado.

Cada um desses conceitos desempenha um papel crucial na construção de software que reflete fielmente o domínio do negócio, facilitando assim a comunicação entre as partes interessadas, o entendimento do problema e a manutenção do software.

## O Poder do DDD: Um Exemplo do Mundo Real

Vamos pegar um exemplo do mundo real para ilustrar o poder do DDD. Considere um sistema de saúde onde médicos, pacientes e prontuários estão envolvidos. Em uma abordagem tradicional, você pode acabar com um design centrado no banco de dados com tabelas para médicos, pacientes e registros.

Por exemplo, um médico pode ter muitos pacientes e um paciente pode ter muitos registros médicos. Neste modelo, a relação entre médicos e pacientes pode ser considerada "muitos para muitos", e a relação entre pacientes e registros médicos pode ser considerada "um para muitos".

Mas o que acontece quando as regras de negócio mudam? E se um paciente agora pode ter vários médicos, ou um médico pode gerenciar várias clínicas? Talvez a clínica agora queira monitorar quais médicos se especializam em quais condições para referenciar corretamente os pacientes.

Nesses cenários, a abordagem DDD se mostraria bastante útil. Com o DDD, você começaria com as regras de negócios. Ao invés de começar pelo banco de dados, você começaria modelando as entidades do domínio - médicos, pacientes, registros médicos, clínicas, condições médicas, etc.

Em vez de um simples relacionamento "muitos para muitos" entre médicos e pacientes, você poderia ter um objeto Agregado "Cuidado ao Paciente" que inclui um médico, um paciente e talvez uma lista de condições médicas. Este agregado, então, poderia ser gerenciado como uma unidade única, com a garantia de que a lógica de negócios seja consistentemente aplicada sempre que um médico for atribuído a um paciente.

Além disso, cada vez que uma regra de negócios mudar, essa mudança é refletida no modelo de domínio, que por sua vez leva a mudanças no código. Ou seja, **mudanças nas regras de negócio levam a mudanças no modelo, que por sua vez levam a mudanças no código**.

É uma abordagem mais natural e flexível, permitindo que o software se adapte melhor às mudanças de negócios e simplificando a manutenção e a extensão do software a longo prazo.

## Conclusão: A Magia do DDD

Então, por que você deveria se importar com o Design Orientado ao Domínio? Porque não se trata **apenas de escrever código**. Trata-se de **entender o problema** que você está tentando resolver e **construir uma solução que reflita esse entendimento**. Conforme foi dito antes, é sobre **construir a ponte entre o mundo dos negócios e o mundo do software**. É sobre construir software flexível, sustentável e escalável que pode **se adaptar às mudanças nas necessidades de negócios**.

O DDD é como uma bússola te guiando através da complexa paisagem do desenvolvimento de software. Ele não é uma bala de prata, e não possui seus próprios desafios. Mas, quando aplicado corretamente, pode levar a um software que realmente **traduz a linguagem dos negócios**.

Portanto, na próxima vez que você embarcar em uma jornada de desenvolvimento de software, lembre-se da "magia" do Design Orientado ao Domínio. Lembre-se de que você não é apenas um **codificador**, mas um tradutor, um designer, um **resolvedor de problemas**. E quem sabe? Você pode descobrir -assim como eu descobri - que o DDD é a chave para ajudar a liberar todo o potencial do seu software.

Para leituras adicionais e um mergulho profundo no mundo do Design Orientado ao Domínio, recomendo fortemente o livro de Eric Evans "Domain-Driven Design: Tackling Complexity in the Heart of Software" [1] e "Implementing Domain-Driven Design" de Vaughn Vernon [2]. Ambos fornecem insights abrangentes e exemplos práticos que te ajudarão a entender e aplicar o DDD em seus projetos.

[1] Evans, E. (2003). [Domain-Driven Design: Tackling Complexity in the Heart of Software](https://www.oreilly.com/library/view/domain-driven-design-tackling/0321125215/). Addison-Wesley Professional.

[2] Vernon, V. (2013). [Implementing Domain-Driven Design](https://www.oreilly.com/library/view/implementing-domain-driven-design/9780133039900/). Addison-Wesley Professional.

Lembre-se, uma longa jornada começa sempre com o primeiro passo. Então, por que não dar esse passo com o Design Orientado ao Domínio?

Feliz codificação!

---

*Aviso: Esta postagem é uma **visão geral - BEEEMMMM - simplificada** do Design Orientado ao Domínio. O DDD é um tópico profundo e complexo que requer estudo e compreensão adicionais. Sempre considere as necessidades específicas e o contexto do seu projeto antes de aplicar qualquer abordagem de desenvolvimento de software.*
