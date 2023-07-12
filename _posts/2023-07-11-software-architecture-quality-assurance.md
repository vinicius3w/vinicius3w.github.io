---
title: "O papel da Garantia de Qualidade da Arquitetura de Software no Desenvolvimento de Software Moderno"
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
  - Software Architecture Evolution
  - Software Development
  - Maintainability
  - Software Architectural Quality Assurance
  - SAQA
  - Principles and Practices
  - Modularity
  - Encapsulation
  - Tools and Techniques
  - Static Code Analysis
  - Code Reviews
  - Architectural Reviews
---

No contexto do desenvolvimento de software, a qualidade **não pode ser** uma reflexão tardia - ela é uma parte integrante do processo que começa com uma concepção (design, projeto) inicial e continua até o software entrar nos ciclos de manutenção e atualizações (em operação, sendo mais atual). Um dos principais aspectos para garantir a qualidade do software é a Garantia da Qualidade da Arquitetura do Software, que em inglês gosto de referenciar como **Software Architectural Quality Assurance (SAQA)**. Essa disciplina, por assim dizer, se concentra na **avaliação e no aprimoramento da arquitetura do software**, que forma a espinha dorsal de qualquer sistema de software.

## Entendendo a Garantia de Qualidade da Arquitetura do Software

A Garantia de Qualidade da Arquitetura do Software é um processo sistemático que tem por objetivo garantir que a arquitetura de software de um sistema atenda aos requisitos especificados e siga os padrões de qualidade estabelecidos. Ela envolve a aplicação de metodologias e técnicas para avaliar a qualidade da arquitetura de software, garantindo que ela seja projetada e implementada corretamente.

Esta qualidade é avaliada com base em vários atributos, geralmente chamados de "*ilidades*". Esses atributos incluem usabilidade, confiabilidade, disponibilidade, portabilidade, testabilidade, escalabilidade, flexibilidade, reutilização, capacidade de manutenção, capacidade de suporte, interoperabilidade, desempenho e segurança. Cada um desses atributos contribui para a qualidade geral do sistema de software e é fundamental para determinar se o software é de boa qualidade ou não.

## Princípios da Garantia de Qualidade da Arquitetura de Software

Os princípios do **SAQA** estão centrados na avaliação e melhoria dos atributos de qualidade acima mencionados. Aqui está uma breve **visão geral** desses princípios:

- **Usabilidade** (*Usability*): se concentra na eficácia com que um usuário pode utilizar um sistema e na facilidade com que os usuários podem aprender a operar ou controlar o sistema. Os aplicativos de software devem ser fáceis de usar.
- **Confiabilidade** (*Reliability*): é sobre a capacidade de um sistema continuar operando ao longo do tempo sem falhas.
- **Disponibilidade** (*Availability*): está relacionado com a relação entre o tempo disponível do sistema e o tempo total de trabalho necessário ou esperado para funcionar.
- **Portabilidade** (*Portability*): se concentra na capacidade de um aplicativo de software ser executado em várias plataformas.
- **Testabilidade** (*Testability*): mostra o quão bem o sistema ou componente facilita a realização de testes para determinar se os critérios de teste predefinidos foram atendidos.
- **Escalabilidade** (*Scalability*): é sobre a capacidade de um sistema de lidar com a demanda de estresse causada pelo aumento do uso sem diminuir o desempenho.
- **Flexibilidade** (*Flexibility*): é sobre a capacidade de um sistema de se adaptar a mudanças futuras.
- **Reusabilidade** (*Reusability*): é sobre o uso de software existente em mais de um software com pouca ou nenhuma alteração. É um atributo de qualidade econômico e que economiza tempo.
- **Manutenibilidade** (*Maintainability*): é sobre a capacidade de um aplicativo de software ser facilmente mantido e suportar mudanças de forma econômica.
- **Suportabilidade** (*Supportability*): é sobre a capacidade de um sistema que satisfaça os requisitos e necessidades necessários para identificar e resolver problemas.
- **Interoperabilidade** (*Interoperability*): é sobre a capacidade de dois ou mais sistemas se comunicarem ou trocarem dados facilmente e usarem os dados que foram trocados.
- **Desempenho** (*Performance*): é sobre a capacidade de um sistema na forma de capacidade de resposta a várias ações dentro de um determinado período de tempo.
- **Segurança** (*Security*): diz respeito à capacidade de um sistema resistir ou bloquear tentativas maliciosas ou não autorizadas que destroem o sistema e ao mesmo tempo fornecem acesso a usuários legítimos.

Esses princípios não são **exaustivos** e podem (devem?) ser priorizados com base nas **necessidades específicas de um projeto**. No entanto, eles fornecem um framework abrangente para entender e implementar o **SAQA**.

## A importância da Garantia de Qualidade da Arquitetura de Software

SAQA é crucial por vários motivos. Primeiro, porque procura criar meios que auxiliem o time de **desenvolvimento, entrega e operação de software** a garantir que o produto de software (muito importante compreender a solução como um **produto**) seja concebido, projetado e implementado corretamente, reduzindo a probabilidade de erros, falhas ou mal compreensões (ou até mesmo incompreensões) de aspectos fundamentais dele como produto (comportamentos, regras de negócio, entre outras preocupações).

Em segundo lugar, ajuda a identificar e abordar possíveis problemas no **início** do processo de desenvolvimento, **economizando tempo e recursos**.

Em terceiro lugar, contribui para a qualidade geral do software, aprimorando seu desempenho, confiabilidade e usabilidade.

E, por fim, melhora o retorno sobre o investimento (ROI) dos sistemas de TI e produz um produto de melhor qualidade.

## Metodologias em Garantia de Qualidade de Arquitetura de Software

Existem várias metodologias usadas em **SAQA**. Essas metodologias fornecem uma abordagem estruturada para avaliar e melhorar a qualidade da arquitetura de software, onde é possível citar:

1. **Revisões de Arquitetura**: Esta metodologia envolve uma revisão completa da arquitetura de software por uma equipe de especialistas. A revisão se concentra na avaliação da arquitetura em relação aos atributos de qualidade definidos e na identificação de possíveis problemas ou áreas para melhoria.
2. **Inspeções de código**: Esta metodologia envolve um exame detalhado do código-fonte. O objetivo é identificar quaisquer erros de codificação, vulnerabilidades de segurança ou violações de padrões de codificação que possam afetar a qualidade do software.
3. **Análise Estática**: Esta metodologia envolve o uso de ferramentas para analisar automaticamente o código-fonte sem executá-lo. O objetivo é detectar possíveis erros, bugs ou vulnerabilidades de segurança no código.
4. **Análise Dinâmica**: Esta metodologia envolve a execução do sistema de software sob condições controladas para observar seu comportamento e identificar eventuais anomalias.
5. **Verificação de modelos**: Esta metodologia envolve o uso de modelos matemáticos para representar a arquitetura do software e verificar suas propriedades.
6. **Simulação**: Esta metodologia envolve o uso de ferramentas de software para simular o comportamento do sistema de software sob várias condições e cargas.

Essas metodologias **não são mutuamente exclusivas** e geralmente são usadas em **combinação** para fornecer uma **avaliação abrangente** da arquitetura de software.

### Melhores práticas em Garantia de Qualidade de Arquitetura de Software

A implementação eficaz de uma cultura corporativa de **SAQA** requer adesão a certas práticas recomendadas. Essas melhores práticas garantem que o processo seja realizado de forma eficiente e produza os resultados desejados. Aqui estão algumas das melhores práticas a serem consideradas:

1. **Definir atributos de qualidade**: A primeira etapa na garantia de qualidade da arquitetura de software é definir os atributos de qualidade que são importantes para o sistema de software. Esses atributos devem ser claramente definidos e mensuráveis.
2. **Use uma abordagem estruturada**: A garantia de qualidade da arquitetura de software deve ser realizada usando uma abordagem estruturada. Isso envolve o uso de metodologias e técnicas comprovadamente eficazes na avaliação e melhoria da qualidade da arquitetura de software.
3. **Envolva as partes interessadas**: O processo de Garantia de qualidade da arquitetura de software deve envolver todas as partes interessadas relevantes, incluindo desenvolvedores, testadores, arquitetos e usuários. Isso garante que todas as perspectivas sejam consideradas e que o software atenda às necessidades e expectativas de todas as partes interessadas.
4. **Utilizar Ferramentas**: Existem diversas ferramentas disponíveis que podem auxiliar no processo de Garantia da Qualidade Arquitetural de Software. Essas ferramentas podem automatizar determinadas tarefas, tornando o processo mais eficiente e confiável.
5. **Melhoria Contínua**: Garantia de qualidade de arquitetura de software não é uma atividade única. Deve ser um processo contínuo que envolve monitoramento e melhoria contínua da arquitetura de software.

Seguindo essas boas práticas, as organizações podem garantir que seus sistemas de software sejam de alta qualidade e atendam às necessidades e expectativas de seus usuários.

## Preocupações de segurança e proteção na Garantia de Qualidade de Arquitetura de Software

No contexto do **SAQA**, segurança e proteção são primordiais. À medida que os softwares se tornam cada vez mais complexos e interconectados, eles também se tornam mais vulneráveis a ameaças e riscos de segurança. Portanto, é essencial considerar esses aspectos durante o processo de garantia da qualidade.

### Segurança (*Security*) no contexto de uma cultura orientada ao SAQA

Segurança na arquitetura de software refere-se às medidas tomadas para proteger o software contra ameaças como acesso não autorizado, violação de dados e ataques cibernéticos. No contexto de uma cultura orientada ao **SAQA**, a segurança é considerada um atributo chave de qualidade e é avaliada ao longo do processo.

Aqui estão algumas das principais considerações de segurança no escopo de uma cultura orientada ao **SAQA**:

1. **Autenticação e Autorização**: A arquitetura do software deve incluir mecanismos robustos de autenticação e autorização para garantir que somente usuários autorizados possam acessar o sistema e realizar ações.
2. **Proteção de Dados**: A arquitetura do software deve garantir a proteção dos dados, tanto em repouso quanto em trânsito. Isso inclui criptografia de dados confidenciais, armazenamento seguro de dados e transmissão segura de dados.
3. **Tratamento e registro de erros**: A arquitetura do software deve incluir mecanismos para tratamento e registro de erros. Isso pode ajudar na detecção e resposta a incidentes de segurança.
4. **Práticas de codificação segura**: A arquitetura de software deve promover práticas de codificação segura para evitar vulnerabilidades de segurança comuns, como injeção de SQL, script entre sites e estouro de buffer.

### Proteção (*Safety*) no contexto de uma cultura orientada ao SAQA

A proteção na arquitetura de software refere-se às medidas tomadas para evitar que o software cause danos aos usuários, ao ambiente ou a outros sistemas. No contexto de uma cultura orientada ao **SAQA**, a proteção é considerada juntamente com outros atributos de qualidade.

Aqui estão algumas das principais considerações de proteção no escopo de uma cultura orientada ao **SAQA**:

1. **Tolerância a Falhas**: A arquitetura do software deve ser projetada para ser tolerante a falhas. Isso significa que o sistema deve continuar a operar corretamente mesmo na presença de falhas ou falhas.
2. **Detecção e Recuperação de Erros**: A arquitetura do software deve incluir mecanismos para detecção e recuperação de erros. Isso pode ajudar a prevenir falhas e minimizar seu impacto.
3. **Monitoramento do sistema**: A arquitetura do software deve permitir o monitoramento do sistema. Isso pode ajudar a detectar e responder a problemas de segurança.
4. **Interfaces de usuário seguras**: A arquitetura do software deve promover o design de interfaces de usuário seguras. Isso inclui evitar erros do usuário e fornecer feedback claro ao usuário.

## Preocupações de continuidade de negócios na Garantia de Qualidade de Arquitetura de Software

A continuidade dos negócios é mais um aspecto crítico da garantia de qualidade da arquitetura de software moderna. Na era digital de hoje, as organizações dependem fortemente de sistemas de software para suas operações. Qualquer interrupção nesses sistemas pode ter consequências graves, incluindo perda de receita, danos à reputação e penalidades regulatórias. Portanto, é essencial considerar a continuidade dos negócios durante o processo de garantia de qualidade.

### Compreendendo a continuidade de negócios no contexto de uma cultura orientada ao SAQA

A continuidade de negócios no contexto da arquitetura de software refere-se à capacidade do sistema de software de continuar operando sob condições adversas, como falhas de sistema, ataques cibernéticos ou desastres naturais. Envolve o planejamento de possíveis interrupções, a implementação de medidas para evitar tais interrupções e a preparação para a recuperação se ocorrerem interrupções.

No **SAQA**, a continuidade do negócio é considerada um atributo chave de qualidade. A arquitetura de software deve ser projetada e implementada de forma a garantir a operação contínua do sistema, mesmo diante de interrupções.

### Principais considerações para continuidade de negócios no contexto de uma cultura orientada ao SAQA

Aqui estão algumas das principais considerações para a continuidade dos negócios na Garantia de Qualidade da Arquitetura de Software:

1. **Redundância**: A arquitetura de software deve incluir componentes redundantes para garantir que, se um componente falhar, outros possam assumir suas funções. Isso pode incluir servidores redundantes, bancos de dados ou conexões de rede.
2. **Planejamento de recuperação de desastres**: A arquitetura do software deve facilitar o planejamento de recuperação de desastres. Isso inclui a capacidade de fazer backup de dados, restaurar sistemas de backups e alternar para sistemas de backup em caso de desastre.
3. **Tolerância a falhas**: Conforme mencionado na seção de segurança, a arquitetura do software deve ser projetada para ser tolerante a falhas. Isso significa que o sistema deve continuar a operar corretamente mesmo na presença de falhas ou falhas.
4. **Escalabilidade**: A arquitetura de software deve ser escalável para lidar com o aumento da demanda durante os horários de pico ou períodos de crescimento. Isso pode ajudar a evitar sobrecargas do sistema que podem interromper as operações comerciais.
5. **Monitoramento e Alerta**: A arquitetura do software deve incluir mecanismos para monitoramento e alerta do sistema. Isso pode ajudar a detectar possíveis interrupções antecipadamente e responder a elas rapidamente.

Ao considerar esses aspectos durante o processo de garantia de qualidade, os desenvolvedores de software podem criar sistemas de software que garantem a continuidade dos negócios.

## Preocupações Data-Driven na garantia de qualidade da arquitetura de software

Na era do big data, os sistemas de software são cada vez mais necessários para lidar com grandes volumes de dados em alta velocidade e com grande variedade de tipos e formatos. Isso trouxe as preocupações Data-Driven para a vanguarda da Garantia de Qualidade Arquitetural de Software. Essas preocupações estão relacionadas à capacidade da arquitetura de software de gerenciar e utilizar os dados com eficiência.

### Compreendendo as preocupações bData-Driven na garantia de qualidade da arquitetura de software

As preocupações Data-Driven no contexto da arquitetura de software referem-se aos desafios associados ao manuseio de grandes volumes de dados (volume), processamento de dados rapidamente (velocidade), lidar com vários tipos de dados (variedade), garantir a precisão e consistência dos dados ( veracidade) e derivar valor dos dados (valor). Estes são muitas vezes referidos como os cinco Vs de big data.

No Software Architectural Quality Assurance, as preocupações orientadas por dados são consideradas os principais atributos de qualidade. A arquitetura de software deve ser projetada e implementada de forma a gerenciar e utilizar os dados de forma eficaz, levando em consideração os cinco Vs do big data.

### Principais considerações para preocupações Data-Driven na garantia de qualidade da arquitetura de software

Aqui estão algumas das principais considerações para preocupações Data-Driven na Garantia de qualidade da arquitetura de software:

1. **Gerenciamento de dados**: A arquitetura do software deve facilitar o gerenciamento eficaz dos dados. Isso inclui armazenamento de dados, recuperação de dados, processamento de dados e segurança de dados.
2. **Processamento de Dados**: A arquitetura do software deve ser capaz de processar grandes volumes de dados rapidamente. Isso pode envolver o uso de processamento paralelo, computação distribuída e outras técnicas de computação de alto desempenho.
3. **Integração de Dados**: A arquitetura do software deve facilitar a integração de vários tipos de dados. Isso pode envolver o uso de ferramentas de integração de dados, data warehouses e data lakes.
4. **Qualidade dos Dados**: A arquitetura do software deve garantir a qualidade dos dados. Isso inclui validação de dados, limpeza de dados e verificações de consistência de dados.
5. **Data Analytics**: A arquitetura do software deve facilitar a análise de dados. Isso inclui a capacidade de executar análises descritivas, preditivas e prescritivas nos dados.

Ao considerar esses aspectos durante o processo de garantia de qualidade, os desenvolvedores de software podem criar sistemas de software que gerenciem e utilizem os dados com eficiência.

## Conclusão

Software Architectural Quality Assurance é um aspecto vital do desenvolvimento de software que garante a qualidade da arquitetura de software. Concentrando-se nos principais atributos de qualidade e aplicando os princípios da Garantia de Qualidade Arquitetural de Software, os desenvolvedores de software podem criar sistemas de software de alta qualidade que atendam às necessidades e expectativas de seus usuários. Além disso, seguindo as melhores práticas e considerando segurança, proteção, continuidade de negócios e preocupações orientadas a dados, as organizações podem implementar a Garantia de qualidade arquitetônica de software de maneira eficaz e eficiente.

---

Para leitura adicional, temos alguns artigos:

1. Mistrík, I., Soley, R. M., Ali, N., Grundy, J., & Tekinerdogan, B. (Eds.). (2015). [Software quality assurance: in large scale and complex software-intensive systems](https://books.google.com.br/books?hl=pt-BR&lr=&id=NVaZBQAAQBAJ&oi=fnd&pg=PP1&dq=software+architecture+quality+assurance&ots=p4EhU3D2sk&sig=h3H9KawPLYbikfozacLxrQeGTEk#v=onepage&q=software%20architecture%20quality%20assurance&f=false). Morgan Kaufmann.
2. Christensen, H. B., Hansen, K. M., & Lindstrøm, B. (2010, August). [Lightweight and continuous architectural software quality assurance using the asqa technique](https://link.springer.com/chapter/10.1007/978-3-642-15114-9_11). In European Conference on Software Architecture (pp. 118-132). Berlin, Heidelberg: Springer Berlin Heidelberg. In this paper, we present a novel technique for assessing and prioritizing architectural quality in large-scale software development projects. The technique can be applied with relatively little effort by software architects and thus suited for agile development in which quality attributes can be assessed and prioritized, e.g., within each development sprint. We outline the processes and metrics embodied in the technique, and report initial experiences on the benefits and liabilities. In conclusion, the technique is considered valuable and a viable tool, and has benefits in an architectural, technical, context, as well as in a business and people context.
3. Axelsson, J., & Skoglund, M. (2016). [Quality assurance in software ecosystems: A systematic literature mapping and research agenda](https://www.sciencedirect.com/science/article/abs/pii/S0164121215002861). Journal of Systems and Software, 114, 69-81. Software ecosystems are becoming a common model for software development in which different actors cooperate around a shared platform. However, it is not clear what the implications are on software quality when moving from a traditional approach to an ecosystem, and this is becoming increasingly important as ecosystems emerge in critical domains such as embedded applications. Therefore, this paper investigates the challenges related to quality assurance in software ecosystems, and identifies what approaches have been proposed in the literature. The research method used is a systematic literature mapping, which however only resulted in a small set of six papers. The literature findings are complemented with a constructive approach where areas are identified that merit further research, resulting in a set of research topics that form a research agenda for quality assurance in software ecosystems. The agenda spans the entire system life-cycle, and focuses on challenges particular to an ecosystem setting, which are mainly the results of the interactions across organizational borders, and the dynamic system integration being controlled by the users.
4. Lim, A. P., Thenuardi, D. S., Soewito, B., & Antonyova, A. (2020, August). [Survey on quality assurance testing on service oriented architecture](https://ieeexplore.ieee.org/abstract/document/9211258). In 2020 international conference on information management and technology (ICIMTech) (pp. 443-447). IEEE. Service-Oriented Architecture (SOA) has greatly influenced the world of software development with the proposed combination of business process and application (service). Ensuring that correct implementation of business process in each service in SOA environment is quite different than monolithic applications, where each service must be tested independently and jointly, depending on targeted testing scope. With numerous proposed approaches for solving such challenge, this paper reviews some of those approaches to ease readers understanding of what can be done in testing in SOA environment. More specifically, this paper provides review on generic proposed approaches, unit testing, and integration testing approaches as part of quality assurance testing on SOA environment. In summary, the details of testing implementation will differ for each enterprise/organization as each has different set of requirements to satisfy.
5. [Lean Learning - Applying Lean Techniques to Improve Software Engineering Education](http://spiral.imperial.ac.uk/bitstream/10044/1/64240/6/paper.pdf) por Robert Chatley e T. Field. Este artigo discute como um programa no Imperial College London foi desenvolvido para preencher a lacuna entre o aprendizado acadêmico e as práticas de engenharia de software industrial. Ele fornece insights sobre a estrutura e a evolução do programa, centrado nas ferramentas, técnicas e questões que fazem parte do dia a dia de um desenvolvedor profissional que trabalha em uma equipe moderna.
6. [Software quality assurance in Scrum: The need for concrete guidance on SQA strategies in meeting user expectations](https://open.uct.ac.za/bitstream/11427/5670/1/thesis_com_2013_khalane_t.pdf) por Tiisetso Khalane e M. Tanner. Este estudo identifica e apresenta as preocupações dos stakeholders do projeto em relação ao Software Quality Assurance (SQA) em um ambiente Scrum. Ele revela os conceitos de SQA relacionados à principal preocupação de atender às expectativas do usuário e discute a falta de orientação concreta sobre estratégias, ferramentas e técnicas de SQA no Scrum.
7. [Assuring the Evolvability of Microservices: Insights into Industry Practices and Challenges](http://arxiv.org/pdf/1906.05013) por J. Bogner, J. Fritzsch, S. Wagner e A. Zimmermann. Este artigo discute a garantia da evolubilidade dos Microsserviços e os desafios enfrentados na indústria. Ele fornece insights sobre os processos de garantia de evolubilidade aplicados, o uso de ferramentas, métricas e padrões e reflexões sobre o tema.
8. [Software Architecture Decision-Making Practices and Challenges: An Industrial Case Study](http://arxiv.org/pdf/1610.09240) por Sandun Dasanayake, Jouni Markkula, Sanja Aaramaa e M. Oivo. Este artigo estuda as atuais práticas de tomada de decisão de arquitetura de software na indústria. Ele identifica diferentes práticas de tomada de decisão de arquitetura de software seguidas pelas equipes de software e discute os desafios associados a elas.
9. [Quality Assurance in Scrum Applied to Safety Critical Software](https://dx.doi.org/10.1007/978-3-319-33515-5_8) por G. Hanssen, Børge Haugset, T. Stålhane, T. Myklebust, Ingar Kulbrandstad. Este artigo discute os mecanismos de garantia de qualidade no Scrum e como eles podem ser insuficientes em certos casos, necessitando de tarefas adicionais para uma função interna de controle de qualidade da equipe. [PDF](https://link.springer.com/content/pdf/10.1007%2F978-3-319-33515-5_8.pdf)
10. [Influencers of Quality Assurance in an Open Source Community](https://dx.doi.org/10.1145/3195836.3195853) por A. Alami, Y. Dittrich, A. Wasowski. Este artigo estuda as práticas de garantia de qualidade da comunidade ROS, uma comunidade de código aberto em robótica. [PDF](https://dl.acm.org/doi/pdf/10.1145/3195836.3195853)
11. [Strategies to manage quality requirements in agile software development: a multiple case study](https://dx.doi.org/10.1007/s10664-020-09903-x) por Pertti Karhapää, W. Behutiye, Pilar Rodríguez, M. Oivo, D. Costal, X. Franch, Sanja Aaramaa, M. Choraś, J. Partanen, Antonin Abhervé. Este estudo discute as estratégias para gerenciar os requisitos de qualidade no desenvolvimento ágil de software. [PDF](https://link.springer.com/content/pdf/10.1007/s10664-020-09903-x.pdf)
12. [Towards Assurance-Driven Architectural Decomposition of Software Systems](https://arxiv.org/pdf/2106.09237): Este artigo apresenta uma meta-arquitetura 4-dimensional que separa artefatos computacionais, de coordenação e de software com estado desde o início o estágio de projeto para facilitar a garantia e para uma integração harmoniosa das ferramentas de garantia no Ciclo de Vida de Desenvolvimento de Software (SDLC).
13. [Quality Assurance for Microservice Architectures](https://doi.org/10.1109/ICSESS52187.2021.9522227): Uma visão geral da garantia de qualidade para arquiteturas de microsserviços é fornecida e alguns cheiros arquitetônicos e antipadrão são mostrados.
14. [Lightweight and Continuous Architectural Software Quality Assurance Using the aSQA Technique](https://dblp.org/rec/conf/ecsa/ChristensenHL10): Uma nova técnica para avaliar e priorizar a qualidade de arquitetura em projetos de desenvolvimento de software em larga escala e tem benefícios em um contexto arquitetônico, técnico, bem como em um contexto de negócios e pessoas.
