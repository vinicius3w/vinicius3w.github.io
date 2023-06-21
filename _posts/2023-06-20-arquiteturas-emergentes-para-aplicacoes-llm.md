---
title:  "Arquiteturas Emergentes para Aplicações LLM"
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
  - artificial intelligence
  - deep learning
  - enterprise
  - SaaS
  - machine learning
  - generative artificial intelligence
---

Hoje, gostaria de compartilhar com vocês alguns *insights* importantes de um artigo fascinante publicado pela Andreessen Horowitz, intitulado "[Emerging Architectures for LLM Applications](https://a16z.com/2023/06/20/emerging-architectures-for-llm-applications/)" de autoria de [Matt Bornstein](https://a16z.com/author/matt-bornstein/) and [Rajko Radovanovic](https://a16z.com/author/rajko-radovanovic/). O artigo explora as arquiteturas emergentes para aplicações de [grandes modelos de linguagem (do inglês, *Large language models* - LLM)](https://bit.ly/3CF6Q6T), que são uma nova e poderosa ferramenta para a construção de software.

O artigo começa destacando que, embora os LLMs sejam uma nova ferramenta poderosa, nem sempre é óbvio como utilizá-los devido à sua novidade e comportamento distinto dos recursos computacionais normais. Para ajudar os desenvolvedores a navegar neste novo território, o artigo apresenta uma [arquitetura de referência](https://bit.ly/3NEJ552) para o emergente stack de aplicativos LLM, baseada em conversas com fundadores de startups de IA e engenheiros.

Um dos principais padrões de design discutidos no artigo é o [aprendizado em contexto (*in-context learning*)](https://en.wikipedia.org/wiki/In-context_learning_(natural_language_processing)). A ideia central é usar LLMs prontos para uso, controlando seu comportamento através de prompts inteligentes e condicionamento em dados "*contextuais*" privados. Este padrão efetivamente reduz um problema de IA para um problema de [engenharia de dados](https://bit.ly/3pdNlzg) que a maioria das startups e grandes empresas já sabe como resolver.

O fluxo de trabalho pode ser dividido em três etapas:

1. **Pré-processamento de dados/incorporação**: Esta etapa envolve o armazenamento de dados privados (documentos legais, em nosso exemplo) para serem recuperados posteriormente. Normalmente, os documentos são divididos em partes, passados por um modelo de incorporação e, em seguida, armazenados em um banco de dados especializado chamado banco de dados vetorial.
2. **Construção de prompts/recuperação**: Quando um usuário envia uma consulta (uma questão legal, neste caso), o aplicativo constrói uma série de prompts para enviar ao modelo de linguagem. Um prompt compilado normalmente combina um modelo de prompt codificado pelo desenvolvedor; exemplos de saídas válidas chamadas exemplos de poucos tiros; qualquer informação necessária recuperada de APIs externas; e um conjunto de documentos relevantes recuperados do banco de dados vetorial.
3. **Execução de prompts/inferência**: Uma vez que os prompts foram compilados, eles são enviados a um LLM pré-treinado para inferência - incluindo tanto APIs de modelos proprietários quanto modelos de código aberto ou auto-treinados. Alguns desenvolvedores também adicionam sistemas operacionais como registro, cache e validação nesta etapa.

O artigo também destaca a importância das [estratégias de prompting](https://www.promptingguide.ai/techniques) para LLMs e a incorporação de dados contextuais. As estratégias de prompting estão se tornando cada vez mais complexas e são uma fonte importante de diferenciação de produto. Frameworks de orquestração como [LangChain](https://docs.langchain.com/docs/) e [LlamaIndex](https://bit.ly/3NEcInb) são úteis aqui, pois abstraem muitos dos detalhes do encadeamento de prompts, a interface com APIs externas, a recuperação de dados contextuais de bancos de dados vetoriais e a manutenção da memória em várias chamadas LLM.

Quando se trata de modelos de linguagem, a [OpenAI](https://openai.com/) é a líder. Quase todos os desenvolvedores começam novos aplicativos LLM usando a API OpenAI, geralmente com o modelo gpt-4 ou gpt-4-32k. No entanto, quando os projetos entram em produção e começam a escalar, um conjunto mais amplo de opções entra em jogo, incluindo a mudança para gpt-3.5-turbo, experimentando outros fornecedores proprietários, ou triando algumas solicitações para modelos de código aberto.

Finalmente, o artigo discute a importância das ferramentas operacionais para LLMs. O caching é relativamente comum, pois melhora os tempos de resposta e o custo da aplicação. Ferramentas como [Weights & Biases](https://wandb.ai/site) e [MLflow](https://mlflow.org/) são bastante utilizadas para registrar, rastrear e avaliar as saídas LLM, geralmente com o objetivo de melhorar a construção de prompts, ajustar pipelines ou selecionar modelos.

Espero que vocês achem essas informações tão fascinantes quanto eu. Acredito firmemente que os LLMs têm o potencial de revolucionar a maneira como construímos e interagimos com plataformas de software e serviços. Eles representam uma **mudança arquitetônica significativa** no software, tornando possível para desenvolvedores individuais construir aplicações de IA incríveis em questão de dias (horas?), superando projetos de aprendizado de máquina supervisionado que levaram grandes equipes a trabalhar por meses (anos?) para construir e **colocar em produção**.

No entanto, é importante lembrar que, como qualquer **tecnologia emergente**, os LLMs vêm com seu próprio conjunto de **desafios e considerações**. A aprendizagem em contexto, por exemplo, é uma solução inteligente para o problema da escala, mas também levanta questões sobre **como gerenciar e proteger os dados privados usados para condicionar o modelo**. Além disso, à medida que os LLMs se tornam mais complexos e poderosos, também precisamos considerar questões de **responsabilidade e ética**.

Ainda assim, estou otimista sobre o futuro dos LLMs e ansioso para ver como eles continuarão a evoluir e moldar o campo da IA. Se você é um desenvolvedor, um entusiasta da IA, ou simplesmente alguém interessado em tecnologia, eu encorajo você a ler o artigo completo para obter uma compreensão mais profunda dessas arquiteturas emergentes.
