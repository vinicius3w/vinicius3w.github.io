---
title: "Aspectos Avançados em Engenharia de Software: Explorando o Desenvolvimento Móvel e a Computação em Nuvem"
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
  - Advanced Aspects
  - Mobile Development
  - Native Applications
  - Hybrid Applications
  - Cross-platform frameworks
  - Cloud Computing
  - Cloud Services
  - IaaS
  - PaaS
  - SaaS
  - Scalability
  - Cost-effectiveness
  - Cloud migration
  - Cloud security
  - Cloud performance
  - Technology Advancements
---

Conforme temos discutido ao longo desta série, a Engenharia de Software é a aplicação sistemática de princípios e métodos de engenharia para desenvolver e manter sistemas de software de qualidade. Ela abrange uma ampla gama de tópicos, como ciclo de vida de desenvolvimento de software, gerenciamento de projetos de software, modelos de software, qualidade de software, design e arquitetura de software, teste de software, manutenção de software e evolução de software. Neste artigo, vamos nos concentrar em dois aspectos avançados da engenharia de software: desenvolvimento móvel e computação em nuvem.

## Desenvolvimento Móvel

O desenvolvimento móvel é o processo de criação de aplicativos executados em dispositivos móveis, como smartphones e tablets. Os aplicativos móveis podem fornecer várias funcionalidades, como comunicação, entretenimento, educação, negócios, saúde e redes sociais. O desenvolvimento móvel pode ser classificado em dois tipos principais: nativo e híbrido.

### Aplicações nativas

Os aplicativos nativos são desenvolvidos especificamente para uma plataforma, como Android ou iOS, usando a linguagem de desenvolvimento nativa e as ferramentas dessa plataforma. Por exemplo, um aplicativo iOS nativo seria escrito em Swift ou Objective-C e compilado usando Xcode, enquanto um aplicativo Android nativo seria escrito em Kotlin ou Java e compilado usando Android Studio. Os aplicativos nativos têm as seguintes vantagens:

- Eles podem acessar todos os recursos do dispositivo, como sensores, câmera, GPS, contatos, etc.
- Eles podem fornecer o melhor desempenho e experiência do usuário, pois são otimizados para a plataforma e seguem as diretrizes de interface do usuário específicas da plataforma.
- Eles podem aproveitar os recursos e serviços específicos da plataforma, como notificações push, distribuição na loja de aplicativos, compras no aplicativo etc.

No entanto, os aplicativos nativos também apresentam algumas desvantagens:

- Eles exigem desenvolvimento e manutenção separados para cada plataforma, o que pode aumentar o custo, o tempo e a complexidade do projeto.
- Eles dependem das atualizações da plataforma e problemas de compatibilidade, que podem afetar a funcionalidade e a estabilidade do aplicativo.
- Eles devem cumprir as regras e restrições específicas da plataforma para aprovação e distribuição na loja de aplicativos.

### Aplicações híbridas

Os aplicativos híbridos são uma mistura de soluções nativas e da Web. O núcleo do aplicativo é escrito usando tecnologias da Web, como HTML, CSS e JavaScript, e depois agrupado em um contêiner nativo que permite que o aplicativo seja executado em diferentes plataformas. Por exemplo, um aplicativo híbrido pode usar estruturas como React Native, Flutter, Xamarin, Ionic, NativeScript ou Framework7 para criar uma camada de interface do usuário de plataforma cruzada que interage com os componentes nativos do dispositivo.

As aplicações híbridas têm as seguintes vantagens:

- Eles podem reutilizar a mesma base de código para várias plataformas, o que pode reduzir o custo, o tempo e a complexidade do projeto.
- Eles podem aproveitar as habilidades e ferramentas de desenvolvimento da Web amplamente disponíveis e familiares a muitos desenvolvedores.
- Eles podem se beneficiar dos recursos e serviços da web, como atualizações dinâmicas, suporte offline, otimização de SEO, etc.

No entanto, os aplicativos híbridos também apresentam alguns desafios:

- Eles podem ter desempenho e experiência do usuário inferiores aos aplicativos nativos, pois dependem de uma camada intermediária para se comunicar com o dispositivo.
- Eles podem ter acesso limitado a alguns recursos do dispositivo ou recursos específicos da plataforma que não são suportados pelas tecnologias da Web ou pelo contêiner nativo.
- Eles podem enfrentar problemas de complexidade e compatibilidade de teste em diferentes plataformas, dispositivos, navegadores e versões.

### Ciclo de vida do desenvolvimento

O ciclo de vida de desenvolvimento de aplicativos móveis refere-se ao processo sistemático de pesquisa, design, desenvolvimento, teste e implantação do aplicativo na loja de aplicativos para os usuários. Cada etapa é interconectada por meio de um conjunto de entregas que atuam como entrada para a próxima. O ciclo de vida de desenvolvimento para aplicativos móveis pode ser baseado nos princípios do ciclo de vida de desenvolvimento de software, que consistem em várias fases, como concepção, planejamento, implementação ou execução e encerramento. No entanto, existem alguns aspectos e desafios específicos que precisam ser considerados para o desenvolvimento móvel, como:

- **Ambiente de desenvolvimento**: Os aplicativos móveis podem ser desenvolvidos usando diferentes ferramentas e frameworks, dependendo do tipo de aplicativo (nativo ou híbrido) e da plataforma de destino (Android ou iOS). Por exemplo, aplicativos Android nativos podem ser desenvolvidos usando Android Studio e Kotlin ou Java, enquanto aplicativos iOS nativos podem ser desenvolvidos usando Xcode e Swift ou Objective-C. Os aplicativos híbridos podem usar estruturas de plataforma cruzada como React Native, Flutter, Xamarin, Ionic, NativeScript ou Framework7 para criar uma camada de interface do usuário comum que interage com os componentes nativos do dispositivo. A escolha do ambiente de desenvolvimento depende de diversos fatores, como desempenho, funcionalidade, experiência do usuário, custo, tempo e habilidades necessárias para o projeto.
- **Testes**: os aplicativos móveis precisam ser testados minuciosamente antes da implantação para garantir sua qualidade e funcionalidade. Testar aplicativos móveis envolve diferentes tipos de testes, como testes de unidade, testes de integração, testes funcionais, testes de usabilidade, testes de desempenho, testes de segurança, etc. Testar aplicativos móveis também envolve diferentes métodos e ferramentas, como emuladores, simuladores, dispositivos reais, serviços de teste em nuvem, etc. A escolha dos métodos e ferramentas de teste depende de vários fatores, como disponibilidade de recursos, abrangência de dispositivos e plataformas, complexidade do aplicativo, etc.
- **Garantia de qualidade**: A garantia de qualidade é o processo de garantir que o aplicativo móvel atenda aos requisitos e expectativas dos usuários e partes interessadas. A garantia de qualidade envolve diferentes atividades e padrões, como revisões de código, documentação, diretrizes de design, convenções de codificação, melhores práticas, etc. A garantia de qualidade também envolve diferentes métricas e indicadores para medir e avaliar a qualidade do aplicativo móvel, como funcionalidade, confiabilidade , usabilidade, eficiência, manutenibilidade, portabilidade, etc.
- **Design e arquitetura**: Design e arquitetura são os processos de definição e organização da estrutura e comportamento do aplicativo móvel. Design e arquitetura envolvem diferentes aspectos e princípios, como design de interface do usuário, design de experiência do usuário, arquitetura da informação, design de navegação, design de interação, design visual, etc. Design e arquitetura também envolvem diferentes modelos e padrões para representar e implementar o aplicativo móvel, como MVC (Model-View-Controller), MVP (Model-View-Presenter), MVVM (Model-View-ViewModel), etc.
- **Implantar**: Implantar é o processo de liberar e distribuir o aplicativo móvel para os usuários por meio da loja de aplicativos ou de outros canais. A implantação envolve diferentes etapas e desafios, como empacotamento, assinatura, upload, revisão, aprovação, publicação, atualização, etc. A implantação também envolve diferentes estratégias e técnicas para otimizar e aprimorar o processo de implantação, como integração contínua, entrega contínua, implantação contínua , etc

### Frameworks cross-platform vs ferramentas de desenvolvimento nativas

As vantagens e desvantagens do uso de frameworks cross-platform versus ferramentas de desenvolvimento nativas para desenvolvimento móvel são:

- **Vantagens de frameworks multiplataforma**:
  - Eles permitem que os desenvolvedores reutilizem a mesma base de código para várias plataformas, o que pode reduzir o tempo, o custo e a complexidade do desenvolvimento.
  - Eles permitem que os desenvolvedores aproveitem as habilidades e ferramentas de desenvolvimento da Web amplamente disponíveis e familiares a muitos desenvolvedores.
  - Eles se beneficiam de recursos e serviços da web, como atualizações dinâmicas, suporte offline, otimização de SEO, etc.
- Eles permitem que os desenvolvedores reutilizem a mesma base de código para várias plataformas, o que pode reduzir o tempo, o custo e a complexidade do desenvolvimento.
- Eles permitem que os desenvolvedores aproveitem as habilidades e ferramentas de desenvolvimento da Web amplamente disponíveis e familiares a muitos desenvolvedores.
- Eles se beneficiam de recursos e serviços da web, como atualizações dinâmicas, suporte offline, otimização de SEO, etc.
- **Desvantagens dos frameworks multiplataforma**:
  - Eles podem ter desempenho e experiência do usuário inferiores aos aplicativos nativos, pois dependem de uma camada intermediária para se comunicar com o dispositivo.
  - Eles podem ter acesso limitado a alguns recursos do dispositivo ou recursos específicos da plataforma que não são suportados pelas tecnologias da Web ou pelo contêiner nativo.
  - Eles podem enfrentar problemas de complexidade e compatibilidade de teste em diferentes plataformas, dispositivos, navegadores e versões.
- Eles podem ter desempenho e experiência do usuário inferiores aos aplicativos nativos, pois dependem de uma camada intermediária para se comunicar com o dispositivo.
- Eles podem ter acesso limitado a alguns recursos do dispositivo ou recursos específicos da plataforma que não são suportados pelas tecnologias da Web ou pelo contêiner nativo.
- Eles podem enfrentar problemas de complexidade e compatibilidade de teste em diferentes plataformas, dispositivos, navegadores e versões.
- **Vantagens das ferramentas de desenvolvimento nativas**:
  - Eles permitem que os desenvolvedores acessem todos os recursos do dispositivo, como sensores, câmera, GPS, contatos etc.
  - Eles permitem que os desenvolvedores forneçam o melhor desempenho e experiência do usuário, pois são otimizados para a plataforma e seguem as diretrizes de interface do usuário específicas da plataforma.
  - Eles aproveitam os recursos e serviços específicos da plataforma, como notificações push, distribuição na loja de aplicativos, compras no aplicativo etc.
- Eles permitem que os desenvolvedores acessem todos os recursos do dispositivo, como sensores, câmera, GPS, contatos etc.
- Eles permitem que os desenvolvedores forneçam o melhor desempenho e experiência do usuário, pois são otimizados para a plataforma e seguem as diretrizes de interface do usuário específicas da plataforma.
- Eles aproveitam os recursos e serviços específicos da plataforma, como notificações push, distribuição na loja de aplicativos, compras no aplicativo etc.
- **Desvantagens das ferramentas de desenvolvimento nativas**:
  - Eles exigem desenvolvimento e manutenção separados para cada plataforma, o que pode aumentar o tempo, o custo e a complexidade do desenvolvimento.
  - Eles dependem das atualizações da plataforma e problemas de compatibilidade, que podem afetar a funcionalidade e a estabilidade do aplicativo.
  - Eles devem cumprir as regras e restrições específicas da plataforma para aprovação e distribuição na loja de aplicativos.
- Eles exigem desenvolvimento e manutenção separados para cada plataforma, o que pode aumentar o tempo, o custo e a complexidade do desenvolvimento.
- Eles dependem das atualizações da plataforma e problemas de compatibilidade, que podem afetar a funcionalidade e a estabilidade do aplicativo.
- Eles devem cumprir as regras e restrições específicas da plataforma para aprovação e distribuição na loja de aplicativos.

### Melhores práticas e padrões para projetar UI e UX para aplicativos móveis

Algumas práticas recomendadas e padrões para projetar interfaces de usuário e experiências de usuário para aplicativos móveis são:

- **Conheça seus usuários**: entenda seus objetivos, habilidades, preferências e tendências. Realize pesquisas de usuários, como entrevistas, pesquisas, personas, cenários, etc., para obter insights e feedback de seus usuários-alvo. Use esses insights para informar suas decisões de design e avaliar suas soluções de design.
- **Mantenha a interface simples**: As melhores interfaces são quase invisíveis para o usuário. Eles evitam elementos desnecessários e são claros na linguagem que usam nos rótulos e nas mensagens. Eles usam cores e contrastes para destacar informações e ações importantes. Eles fornecem feedback visual para ações do usuário e status do sistema. Eles seguem as diretrizes e convenções de interface do usuário específicas da plataforma para garantir consistência e familiaridade.
- **Torne a interface responsiva**: a interface deve se adaptar a diferentes tamanhos de tela, orientações, resoluções e dispositivos. Ele também deve fornecer desempenho rápido e suave, com tempos de carregamento e transições mínimos. Deve usar divulgação progressiva para mostrar informações e opções relevantes na hora e no lugar certo. Ele também deve suportar diferentes métodos de entrada, como toque, gestos, voz, etc.
- **Torne a interface acessível**: A interface deve ser utilizável por pessoas com diferentes habilidades e preferências, como visão, audição, motor, cognitivo, etc. Deve seguir os princípios e padrões de acessibilidade, como WCAG 2.1, para garantir que o conteúdo e a funcionalidade são perceptíveis, operáveis, compreensíveis e robustos. Também deve fornecer opções de customização e personalização, como tamanho da fonte, contraste, idioma, etc.
- **Torne a interface atraente**: a interface deve fornecer uma experiência de usuário positiva e satisfatória que atenda ou exceda as expectativas e necessidades do usuário. Deve usar estética, animações, sons, gamificação, etc., para criar uma conexão emocional e encantar o usuário. Também deve usar storytelling, personalização, interação social, etc., para criar um contexto significativo e uma proposta de valor para o usuário.

### Desafios e soluções de teste e depuração de aplicativos móveis

Alguns dos principais desafios e soluções para testar e depurar aplicativos móveis em diferentes dispositivos e plataformas são:

- **Fragmentação de dispositivo**: aplicativos móveis precisam ser executados em vários dispositivos com diferentes sistemas operacionais, versões, tamanhos de tela, resoluções, especificações de hardware etc. Isso cria um desafio para garantir a compatibilidade, funcionalidade e desempenho dos aplicativos em todas as configurações de dispositivo possíveis. Uma possível solução é usar uma plataforma de teste baseada em nuvem que forneça acesso a um grande conjunto de dispositivos reais e emuladores/simuladores para fins de teste. Por exemplo, o LambdaTest oferece uma nuvem de teste de aplicativos móveis que permite aos usuários testar seus aplicativos em mais de 3.000 dispositivos e navegadores reais.
- **Problemas de largura de banda de rede**: os aplicativos móveis precisam funcionar bem em diferentes condições de rede, como velocidade, latência, estabilidade etc. Isso cria um desafio para garantir a confiabilidade, disponibilidade e usabilidade dos aplicativos em vários cenários de rede. Uma possível solução é usar uma ferramenta de simulação de rede que permita aos usuários emular diferentes ambientes de rede e testar seus aplicativos de acordo. Por exemplo, o BrowserStack oferece um recurso de limitação de rede que permite aos usuários simular diferentes velocidades de rede e larguras de banda para fins de teste.
- **Segurança de aplicativos móveis**: os aplicativos móveis precisam proteger os dados e a privacidade dos usuários e do sistema contra acesso ou modificação não autorizados. Isso cria um desafio para garantir a segurança e a conformidade dos aplicativos contra várias ameaças e vulnerabilidades. Uma possível solução é usar uma ferramenta de teste de segurança que permita aos usuários realizar vários testes de segurança em seus aplicativos, como teste de penetração, verificação de vulnerabilidade, análise de código, etc. Por exemplo, o ZAP (Zed Attack Proxy) é um código aberto de segurança ferramenta de teste que permite aos usuários encontrar e corrigir problemas de segurança em seus aplicativos.
- **Teste de condição de usuário real**: os aplicativos móveis precisam fornecer uma experiência de usuário positiva e satisfatória que atenda ou exceda as expectativas e necessidades do usuário. Isso cria um desafio para garantir a usabilidade e acessibilidade dos aplicativos sob condições reais do usuário, como gestos, orientação, localização etc. utilizam suas aplicações em ambientes reais. Por exemplo, UserTesting é uma plataforma de teste de usuário que permite aos usuários obter feedback em vídeo de usuários reais que testam seus aplicativos em seus próprios dispositivos.
- **Diferentes tipos de aplicativos**: os aplicativos móveis podem ser classificados em diferentes tipos com base em sua abordagem de desenvolvimento, como aplicativos nativos, híbridos ou da Web. Isso cria um desafio para escolher as ferramentas e métodos de teste apropriados para cada tipo de aplicativo. Uma solução possível é usar uma ferramenta de teste que suporte vários tipos de aplicativos e forneça um ambiente de teste unificado. Por exemplo, o Appium é uma ferramenta de teste de código aberto que permite aos usuários testar aplicativos nativos, híbridos e da Web usando uma única estrutura.

### Referências

- [What is Hybrid Mobile App Development: Hybrid vs Native vs Web -- Ionic](https://ionic.io/resources/articles/what-is-hybrid-app-development)
- [What Is Hybrid Mobile App Development? A Complete Guide -- Turing](https://www.turing.com/resources/hybrid-mobile-app-development)
- [Native Vs Hybrid Mobile App Development: A Detailed Comparison](https://www.i2tutorials.com/native-vs-hybrid-mobile-app-development-a-detailed-comparison/)
- [Native Vs Hybrid Mobile App: Which is Right Development Approach](https://www.quytech.com/blog/native-vs-hybrid-mobile-app-development/)
- [Modeling the Mobile Application Development Lifecycle](http://www.iaeng.org/publication/IMECS2014/IMECS2014_pp596-600.pdf)
- [6 Stages of the Mobile Development Lifecycle -- G2](https://learn.g2.com/mobile-development-lifecycle)
- [Mobile software development lifecycle - Xamarin -- Microsoft Learn](https://learn.microsoft.com/en-us/xamarin/cross-platform/get-started/introduction-to-mobile-sdlc)
- [Application Development Life Cycle -- aist.global](https://aist.global/en/application-development-lifecycle)
- [Mobile app development process -- LANARS](https://lanars.com/blog/mobile-app-development-process)
- [Mobile App Development Life Cycle -- 5280 SOFTWARE](https://www.5280software.net/blog-post/the-modern-mobile-app-development-life-cycle/)
- [Native vs. Cross-Platform App Development: Which Should You Choose?](https://builtin.com/software-engineering-perspectives/native-vs-cross-platform-app-development)
- [Native vs. Cross Platform Apps -- Microsoft Power Apps](https://powerapps.microsoft.com/en-us/native-vs-cross-platform-apps/)
- [Deciding between native and cross-platform mobile frontend programming frameworks - IBM Developer](https://developer.ibm.com/articles/deciding-between-native-and-cross-platform-mobile-frontend-programming-frameworks/)
- [Native Development vs Cross-Platform Development: Myth and Reality](https://www.mobindustry.net/blog/native-development-vs-cross-platform-development-myth-and-reality/)
- [Native vs Cross-Platform App Development: Which is the Best Option For 2021?](https://javascript.plainenglish.io/native-vs-cross-platform-app-development-which-is-the-best-option-for-2021-ac571a66c568)
- [Accessibility, Usability, and Inclusion -- Web Accessibility Initiative (WAI) --  W3C](https://www.w3.org/WAI/fundamentals/accessibility-usability-inclusion/)
- [What is Mobile User Experience (UX) Design? -- IxDF](https://www.interaction-design.org/literature/topics/mobile-ux-design)
- [User Interface Design Basics -- Usability.gov](https://www.usability.gov/what-and-why/user-interface-design.html)
- [11 Key Challenges & Solutions Of Mobile App Testing - LambdaTest](https://www.lambdatest.com/blog/mobile-app-testing-challenges/)
- [Challenges in Mobile Testing (with Solutions) - BrowserStack](https://www.browserstack.com/guide/mobile-testing-challenges)
- [Mobile App Testing Basics [With Real-Time Examples] - LambdaTest](https://www.lambdatest.com/blog/mobile-app-testing-basics/)
