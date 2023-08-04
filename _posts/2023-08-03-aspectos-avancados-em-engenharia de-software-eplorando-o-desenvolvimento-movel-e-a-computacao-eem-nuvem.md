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

Os aplicativos híbridos são uma mistura de soluções nativas e da Web. O núcleo do aplicativo é escrito usando tecnologias da Web, como HTML, CSS e JavaScript, e depois agrupado em um contêiner nativo que permite que o aplicativo seja executado em diferentes plataformas. Por exemplo, um aplicativo híbrido pode usar estruturas como [React Native](https://reactnative.dev/), [Flutter](https://viniciusgarcia.me/education/um-ensaio-sobre-flutter/), [Xamarin](https://learn.microsoft.com/pt-br/xamarin/get-started/what-is-xamarin), [Ionic](https://ionicframework.com/), [NativeScript](https://nativescript.org/) ou [Framework7](https://framework7.io/) para criar uma camada de interface do usuário de plataforma cruzada que interage com os componentes nativos do dispositivo.

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

- **Ambiente de desenvolvimento**: Os aplicativos móveis podem ser desenvolvidos usando diferentes ferramentas e frameworks, dependendo do tipo de aplicativo (nativo ou híbrido) e da plataforma de destino (Android ou iOS). Por exemplo, aplicativos Android nativos podem ser desenvolvidos usando [Android Studio](https://developer.android.com/studio) e [Kotlin](https://www.w3schools.com/kotlin/index.php) ou Java, enquanto aplicativos iOS nativos podem ser desenvolvidos usando Xcode e [Swift](https://www.devmedia.com.br/desenvolvimento-ios-conheca-a-linguagem-swift/31860) ou Objective-C. Os aplicativos híbridos podem usar estruturas de plataforma cruzada como React Native, Flutter, Xamarin, Ionic, NativeScript ou Framework7 para criar uma camada de interface do usuário comum que interage com os componentes nativos do dispositivo. A escolha do ambiente de desenvolvimento depende de diversos fatores, como desempenho, funcionalidade, experiência do usuário, custo, tempo e habilidades necessárias para o projeto.
- **Testes**: os aplicativos móveis precisam ser testados minuciosamente antes da implantação para garantir sua qualidade e funcionalidade. Testar aplicativos móveis envolve diferentes tipos de testes, como testes de unidade, testes de integração, testes funcionais, testes de usabilidade, testes de desempenho, testes de segurança, etc. Testar aplicativos móveis também envolve diferentes métodos e ferramentas, como emuladores, simuladores, dispositivos reais, serviços de teste em nuvem, etc. A escolha dos métodos e ferramentas de teste depende de vários fatores, como disponibilidade de recursos, abrangência de dispositivos e plataformas, complexidade do aplicativo, etc.
- **Garantia de qualidade**: A garantia de qualidade é o processo de garantir que o aplicativo móvel atenda aos requisitos e expectativas dos usuários e partes interessadas. A garantia de qualidade envolve diferentes atividades e padrões, como revisões de código, documentação, diretrizes de design, convenções de codificação, melhores práticas, etc. A garantia de qualidade também envolve diferentes métricas e indicadores para medir e avaliar a qualidade do aplicativo móvel, como funcionalidade, confiabilidade , usabilidade, eficiência, manutenibilidade, portabilidade, etc.
- **Design e arquitetura**: Design e arquitetura são os processos de definição e organização da estrutura e comportamento do aplicativo móvel. Design e arquitetura envolvem diferentes aspectos e princípios, como design de interface do usuário, design de experiência do usuário, arquitetura da informação, design de navegação, design de interação, design visual, etc. Design e arquitetura também envolvem diferentes modelos e padrões para representar e implementar o aplicativo móvel, como [MVC](https://pt.wikipedia.org/wiki/MVC) (Model-View-Controller), [MVP](https://pt.wikipedia.org/wiki/Model-view-presenter) (Model-View-Presenter), [MVVM](https://learn.microsoft.com/en-us/dotnet/architecture/maui/mvvm) (Model-View-ViewModel), etc.
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

### Como o desenvolvimento móvel pode se beneficiar dos serviços de computação em nuvem

O desenvolvimento móvel pode se beneficiar dos serviços de computação em nuvem de várias maneiras, como:

- **A computação em nuvem pode fornecer serviços de back-end escaláveis e flexíveis**: os aplicativos móveis geralmente precisam interagir com serviços de back-end, como armazenamento de dados, autenticação, análise, notificações por push, etc. A computação em nuvem pode fornecer esses serviços como uma plataforma ou um serviço (PaaS) ou um back-end como serviço (BaaS), que pode aumentar ou diminuir de acordo com a demanda do aplicativo, sem exigir que os desenvolvedores gerenciem a infraestrutura subjacente. Por exemplo, o AWS Amplify é uma plataforma de nuvem que fornece vários serviços de back-end para desenvolvimento móvel, como AWS AppSync, AWS Cognito, AWS Pinpoint etc.
- **A computação em nuvem pode habilitar a computação sem servidor**: A computação sem servidor é um modelo de computação em nuvem que permite aos desenvolvedores executar código sem provisionar ou gerenciar servidores. A computação sem servidor pode reduzir o tempo e o custo de desenvolvimento, além de melhorar o desempenho e a confiabilidade do aplicativo. A computação sem servidor também pode oferecer suporte a arquiteturas de microsserviços e orientadas a eventos, que podem aprimorar a funcionalidade e a modularidade do aplicativo. Por exemplo, o AWS Lambda é um serviço de computação sem servidor que permite aos desenvolvedores executar código em resposta a eventos, como solicitações HTTP, alterações no banco de dados etc.
- **A computação em nuvem pode facilitar o desenvolvimento multiplataforma**: o desenvolvimento multiplataforma é uma abordagem que permite aos desenvolvedores criar aplicativos que podem ser executados em várias plataformas, como Android e iOS, usando uma única base de código. O desenvolvimento multiplataforma pode reduzir o esforço e a complexidade do desenvolvimento, bem como aumentar o alcance e a compatibilidade do aplicativo. A computação em nuvem pode oferecer suporte ao desenvolvimento de plataforma cruzada, fornecendo ferramentas e estruturas que podem gerar aplicativos nativos ou híbridos a partir de tecnologias da Web, como HTML, CSS e JavaScript. Por exemplo, o Google Cloud App Engine é uma plataforma de nuvem que permite aos desenvolvedores criar e implantar aplicativos da Web que podem ser executados em dispositivos Android e iOS.

#### Provedores de BaaS (Backend as a Service) para desenvolvimento móvel

Alguns provedores populares de BaaS para desenvolvimento móvel são:

- **Back4App**: Back4App é uma plataforma BaaS que fornece serviços de back-end escalonáveis e flexíveis para aplicativos móveis e da web. O Back4App é baseado na estrutura Parse de código aberto, que oferece vários recursos, como armazenamento de dados, autenticação do usuário, notificações push, funções de nuvem, suporte a GraphQL, etc. O Back4App também fornece um painel amigável, uma interface de linha de comando, e SDKs para diferentes plataformas, como Android, iOS, Flutter, React Native, etc.
- **Firebase**: Firebase é uma plataforma BaaS que fornece vários serviços de back-end para aplicativos móveis e da web. O Firebase faz parte do Google Cloud Platform, que oferece vários recursos, como armazenamento de dados, autenticação do usuário, notificações push, funções de nuvem, aprendizado de máquina, análise etc. O Firebase também fornece um console amigável, uma interface de linha de comando, e SDKs para diferentes plataformas, como Android, iOS, Flutter, React Native, etc.
- **AWS Amplify**: AWS Amplify é uma plataforma BaaS que fornece vários serviços de back-end para aplicativos móveis e web. O AWS Amplify faz parte da plataforma Amazon Web Services (AWS), que oferece vários recursos, como armazenamento de dados, autenticação de usuário, notificações por push, funções de nuvem, suporte a GraphQL, análises, etc. O AWS Amplify também fornece um console amigável, uma interface de linha de comando e SDKs para diferentes plataformas, como Android, iOS, Flutter, React Native, etc.
- **Azure Mobile Apps**: Azure Mobile Apps é uma plataforma BaaS que fornece vários serviços de back-end para aplicativos móveis e web. O Azure Mobile Apps faz parte da plataforma Microsoft Azure, que oferece vários recursos, como armazenamento de dados, autenticação do usuário, notificações push, funções de nuvem, análises, etc. O Azure Mobile Apps também fornece um portal amigável, uma interface de linha de comando , e SDKs para diferentes plataformas, como Android, iOS, Flutter, React Native, etc.

### Referências para Desenvolvimento Móvel

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
- [BaaS: o divisor de águas para o desenvolvimento ágil de aplicativos](https://www.synsoftglobal.com/blog/baas-the-game-changer-for-agile-app-development/)
- [Melhor software Mobile Backend-as-a-Service (mBaaS) - G2](https://www.g2.com/categories/mobile-backend-as-a-service-mbaas)
- [Top 9 Mobile Backend as a Service (MBaaS) Platforms in 2023](https://www.mobindustry.net/blog/top-9-mobile-backend-as-a-service-mbaas-platforms/)
- [Melhores provedores de back-end de BaaS como serviço de 2023 - DigitalCruch](https://digitalcruch.com/baas-backend-as-a-service/)

## Computação em nuvem

A computação em nuvem é a entrega de recursos de computação (como servidores, armazenamento, bancos de dados, rede, software, análise e inteligência) como serviços pela Internet. A computação em nuvem elimina a necessidade de indivíduos e empresas autogerenciarem recursos físicos e pagarem apenas pelo que usam. A computação em nuvem oferece vários benefícios, como escalabilidade, flexibilidade, confiabilidade, segurança e economia. Existem três tipos principais de modelos de serviço de computação em nuvem:

### Infraestrutura como serviço (IaaS)

A IaaS fornece acesso a recursos de computação de baixo nível, como máquinas virtuais, discos de armazenamento, dispositivos de rede, etc., que podem ser configurados e gerenciados pelo usuário de acordo com suas necessidades. A IaaS permite que os usuários tenham controle total sobre sua infraestrutura e a personalizem de acordo com seus requisitos. O IaaS é adequado para usuários que precisam de alto desempenho e flexibilidade para seus aplicativos e que possuem habilidades técnicas e recursos para gerenciar sua infraestrutura. Exemplos de provedores de IaaS incluem Google Cloud Compute Engine, Amazon Web Services EC2, Microsoft Azure Virtual Machines, etc.

### Plataforma como serviço (PaaS)

A PaaS fornece acesso a recursos de computação de alto nível, como ferramentas de desenvolvimento, ambientes de tempo de execução, middleware, bancos de dados etc., que podem ser usados para criar e implantar aplicativos em nuvem sem se preocupar com a infraestrutura subjacente. A PaaS permite que os usuários se concentrem na lógica e na funcionalidade do aplicativo, e não no gerenciamento da infraestrutura. A PaaS é adequada para usuários que precisam de desenvolvimento e implantação rápidos para seus aplicativos e que possuem habilidades e recursos de desenvolvimento para usar os serviços da plataforma. Exemplos de provedores de PaaS incluem Google Cloud App Engine, Amazon Web Services Elastic Beanstalk, Microsoft Azure App Service, etc.

### Software como Serviço (SaaS)

O SaaS fornece acesso a aplicativos prontos que são executados na nuvem e podem ser acessados pela Internet. O SaaS permite que os usuários usem os aplicativos sem instalá-los ou mantê-los em seus dispositivos. O SaaS é adequado para usuários que precisam de acesso simples e conveniente a aplicativos e que não possuem habilidades técnicas ou recursos para desenvolvê-los ou gerenciá-los. Exemplos de provedores de SaaS incluem Google Workspace, Salesforce, Dropbox, Netflix, etc.

### Desenvolvendo e implantando aplicativos na nuvem

O desenvolvimento e a implantação de aplicativos na nuvem envolvem o uso de serviços de computação em nuvem para criar, testar, executar e gerenciar aplicativos sem a necessidade de lidar com a infraestrutura subjacente. Desenvolver e implantar aplicativos na nuvem pode oferecer vários benefícios, como:

- **Escalabilidade**: os serviços de computação em nuvem podem aumentar ou diminuir automaticamente os recursos de computação de acordo com a demanda do aplicativo, sem exigir intervenção manual ou provisionamento. Isso pode melhorar o desempenho, a disponibilidade e a eficiência do aplicativo, além de reduzir o custo e a complexidade do dimensionamento.
- **Disponibilidade**: os serviços de computação em nuvem podem fornecer alta disponibilidade e confiabilidade para o aplicativo, replicando e distribuindo os recursos de computação em várias regiões e zonas. Isso pode garantir que o aplicativo continue operando mesmo em caso de falhas ou desastres, além de fornecer um tempo de resposta mais rápido para usuários em diferentes locais.
- **Flexibilidade**: os serviços de computação em nuvem podem oferecer uma ampla gama de opções e recursos para desenvolver e implantar aplicativos na nuvem, como diferentes tipos de modelos de serviço (IaaS, PaaS, SaaS), diferentes tipos de plataformas (GKE, Anthos, Cloud Run) , diferentes tipos de ferramentas e estruturas (Cloud Build, Jenkins, Skaffold), etc. Isso pode permitir que os desenvolvedores escolham a melhor solução para suas necessidades e preferências de aplicativos.

No entanto, desenvolver e implantar aplicativos na nuvem também envolve alguns aspectos, questões e desafios que precisam ser considerados, como:

- **Segurança**: Desenvolver e implantar aplicativos na nuvem exige garantir que os dados e o código do aplicativo sejam protegidos contra acesso ou modificação não autorizados, tanto em trânsito quanto em repouso. Isso envolve o uso de criptografia, autenticação, autorização, regras de firewall, políticas de segurança etc., além de seguir as melhores práticas e padrões de segurança. Os serviços de computação em nuvem podem fornecer vários recursos e serviços de segurança para ajudar os desenvolvedores a proteger seus aplicativos na nuvem, como Cloud IAM, Cloud KMS, Cloud Armor, etc.
- **Monitoramento**: Desenvolver e implantar aplicativos na nuvem requer monitorar o desempenho, integridade e uso do aplicativo e seus componentes, além de detectar e resolver quaisquer problemas ou erros que possam ocorrer. Isso envolve o uso de métricas, logs, alertas, painéis etc., além de seguir as melhores práticas e padrões de monitoramento. Os serviços de computação em nuvem podem fornecer vários recursos e serviços de monitoramento para ajudar os desenvolvedores a monitorar seus aplicativos na nuvem, como Cloud Monitoring, Cloud Logging, Cloud Trace, Cloud Debugger, etc.
- **Custo**: Desenvolver e implantar aplicativos na nuvem requer o gerenciamento do custo de uso de serviços de computação em nuvem para o aplicativo. Isso envolve estimar e otimizar o custo de uso de diferentes tipos de recursos e serviços, além de seguir as melhores práticas e padrões de gestão de custos. Os serviços de computação em nuvem podem fornecer vários recursos e serviços de custo para ajudar os desenvolvedores a gerenciar seus custos na nuvem, como Cloud Billing, Cloud Pricing Calculator, Cloud Recommendations, etc.

### Desafios comuns na computação em nuvem

Alguns desafios comuns na computação em nuvem são:

- **Segurança e privacidade de dados**: a computação em nuvem envolve o armazenamento e o processamento de dados em servidores remotos pertencentes e gerenciados por provedores terceirizados. Isso levanta preocupações sobre a confidencialidade, integridade e disponibilidade dos dados, bem como a conformidade com as leis e regulamentos de proteção de dados. Os usuários da nuvem precisam garantir que seus dados sejam criptografados, autenticados, autorizados e com backup, além de seguir as melhores práticas e padrões de segurança. Os provedores de nuvem precisam fornecer recursos e serviços de segurança transparentes e confiáveis para ajudar os usuários da nuvem a proteger seus dados na nuvem, como Cloud IAM, Cloud KMS, Cloud Armor, etc.
- **Vendor lock-in**: A computação em nuvem envolve confiar em um provedor de nuvem específico para o fornecimento de serviços e recursos em nuvem. Isso cria uma dependência e um risco potencial de perder o controle sobre o ambiente de nuvem, bem como enfrentar dificuldades para mudar para outro provedor ou migrar de volta para sistemas locais. Os usuários de nuvem precisam avaliar a compatibilidade, interoperabilidade e portabilidade dos serviços e recursos de nuvem que usam, bem como seguir as melhores práticas e padrões para evitar a dependência do fornecedor. Os provedores de nuvem precisam fornecer soluções de nuvem flexíveis e abertas que suportem várias plataformas, padrões e formatos, além de facilitar a migração e integração de serviços e recursos de nuvem.
- **Requisitos de conformidade e regulamentares**: a computação em nuvem envolve a transferência e processamento de dados em diferentes jurisdições e regiões que podem ter leis e regulamentos diferentes em relação à proteção de dados, privacidade, segurança, tributação etc. Isso cria desafios para garantir a conformidade e a responsabilidade de os serviços de nuvem e recursos utilizados, bem como enfrentar possíveis questões legais ou penalidades em caso de violações ou disputas. Os usuários de nuvem precisam entender as implicações e obrigações legais de usar serviços e recursos de nuvem em diferentes locais, bem como seguir as melhores práticas e padrões de conformidade. Os provedores de nuvem precisam fornecer informações transparentes e confiáveis sobre a localização, jurisdição e governança de seus serviços e recursos de nuvem, bem como cumprir as leis e regulamentos aplicáveis.
- **Integração de sistemas legados**: A computação em nuvem envolve a adoção de novas tecnologias e paradigmas para desenvolver e implantar aplicativos na nuvem. Isso cria desafios na integração dos sistemas e aplicativos legados existentes com o ambiente de nuvem, bem como na manutenção da consistência, compatibilidade e desempenho dos sistemas híbridos. Os usuários da nuvem precisam avaliar a viabilidade e adequação da migração ou modernização de seus sistemas e aplicativos legados para a nuvem, bem como seguir as melhores práticas e padrões de integração. Os provedores de nuvem precisam fornecer várias ferramentas e estruturas para ajudar os usuários da nuvem a migrar ou modernizar seus sistemas e aplicativos legados para a nuvem, como Cloud Build, Jenkins, Skaffold, etc.
- **Gerenciamento de custos**: a computação em nuvem envolve o pagamento pelos serviços e recursos em nuvem usados com base no pagamento conforme o uso, o que pode reduzir os gastos iniciais de capital e os custos operacionais. No entanto, isso também cria desafios para estimar e otimizar o custo de uso de diferentes tipos de recursos e serviços, além de gerenciar o orçamento e os gastos do projeto de nuvem. Os usuários de nuvem precisam monitorar e analisar o uso e o desempenho de seus serviços e recursos de nuvem, bem como seguir as melhores práticas e padrões de gerenciamento de custos. Os provedores de nuvem precisam fornecer vários recursos e serviços para ajudar os usuários da nuvem a gerenciar seus custos na nuvem, como Cloud Billing, Cloud Pricing Calculator, Cloud Recommendations, etc.

### Melhores práticas para evitar o bloqueio do fornecedor (vendor lock-in)

Algumas práticas recomendadas para evitar o bloqueio do fornecedor são:

- **Identifique dependências complexas**: revise sua pilha de tecnologia existente e identifique os componentes que estão fortemente associados ao serviço ou tecnologia de um fornecedor específico. Tente minimizar ou eliminar essas dependências usando padrões, formatos e protocolos abertos ou abstraindo-os com uma interface ou camada comum.
- **Entenda os pontos em comum**: compare os recursos e funcionalidades de diferentes fornecedores de nuvem e procure aqueles que são compatíveis ou interoperáveis com sua pilha de tecnologia existente e seus requisitos técnicos. Escolha os serviços e recursos de nuvem baseados em tecnologias comuns ou amplamente adotadas, como Linux, Java, SQL, etc.
- **Avalie as alternativas**: antes de se comprometer com um fornecedor de nuvem, pesquise e compare as alternativas disponíveis no mercado. Procure aqueles que oferecem serviços e recursos semelhantes ou melhores a um preço e qualidade competitivos. Considere os prós e contras de cada alternativa, como desempenho, confiabilidade, segurança, escalabilidade, flexibilidade etc.
- **Negocie os termos**: antes de assinar um contrato com um fornecedor de nuvem, negocie os termos e condições favoráveis às suas necessidades e objetivos de negócios. Evite contratos exclusivos ou de longo prazo que limitem sua liberdade e flexibilidade para mudar para outro fornecedor ou migrar de volta para sistemas locais. Procure cláusulas que permitam rescindir o contrato sem multas ou taxas, ou exportar seus dados e código sem restrições ou cobranças.
- **Monitore e otimize os custos**: Acompanhe o uso e os gastos da nuvem e procure maneiras de otimizá-los. Use ferramentas e serviços que ajudam a monitorar e analisar o consumo e o desempenho da nuvem, como Cloud Billing, Cloud Pricing Calculator, Cloud Recommendations etc. demanda, escolhendo o tamanho e o tipo certo de recursos, usando instâncias reservadas ou pontuais, etc.
- **Prepare uma estratégia de saída**: planeje com antecedência a possibilidade de mudar para outro fornecedor de nuvem ou migrar de volta para sistemas locais. Tenha um plano de backup que inclua as etapas e ferramentas necessárias para exportar seus dados e códigos do fornecedor da nuvem, bem como importá-los para outro fornecedor ou sistema. Teste sua estratégia de saída regularmente e atualize-a conforme necessário.

### Vantagens e desvantagens dos modelos de serviço de computação em nuvem

As vantagens e desvantagens de usar diferentes tipos de modelos de serviço de computação em nuvem (IaaS, PaaS, SaaS) são:

| **Modelo de Serviço** | **Vantagens** | **Desvantagens** |
| --- | --- | --- |
| IaaS | - Fornece controle e personalização de baixo nível sobre a infraestrutura <br> - Permite o dimensionamento rápido de recursos de computação de acordo com a demanda <br> - Reduz os custos operacionais e de capital de propriedade e manutenção de hardware físico | - Requer habilidades técnicas e recursos para gerenciar e configurar a infraestrutura <br> - Envolve riscos de segurança e conformidade de compartilhamento de infraestrutura com outros inquilinos <br> - Depende da disponibilidade e confiabilidade do provedor de nuvem |
| PaaS | - Fornece ferramentas e serviços de alto nível para desenvolvimento e implantação de aplicativos em nuvem <br> - Permite desenvolvimento e testes mais rápidos e fáceis sem se preocupar com a infraestrutura <br> - Suporta várias linguagens, estruturas e plataformas | - Limita o controle e customização sobre a infraestrutura <br> - Envolve o aprisionamento do fornecedor e problemas de compatibilidade com diferentes plataformas <br> - Depende da disponibilidade e confiabilidade do provedor de nuvem |
| SaaS | - Fornece aplicativos prontos que são executados na nuvem e acessíveis pela Internet <br> - Permite acesso simples e conveniente aos aplicativos sem instalá-los ou mantê-los <br> - Suporta vários dispositivos, navegadores e locais | - Limita o controle e customização sobre os aplicativos <br> - Envolve riscos de segurança e privacidade do armazenamento de dados na nuvem <br> - Depende da disponibilidade e confiabilidade do provedor de nuvem |

### Melhores práticas e padrões para projetar e implementar aplicativos em nuvem

Algumas práticas recomendadas e padrões para projetar e implementar aplicativos em nuvem são:

- **Escolha o modelo de serviço de nuvem apropriado**: dependendo dos requisitos e objetivos de seu aplicativo, você pode escolher entre diferentes tipos de modelos de serviço de nuvem, como IaaS, PaaS ou SaaS. Cada modelo tem suas próprias vantagens e desvantagens em termos de controle, flexibilidade, escalabilidade, custo, etc. Você deve avaliar as vantagens e desvantagens e selecionar o modelo que melhor atende às suas necessidades.
- **Design para escalabilidade e elasticidade**: os aplicativos em nuvem devem ser capazes de lidar com cargas de trabalho variáveis e imprevisíveis, ajustando dinamicamente os recursos de computação de acordo com a demanda. Você deve projetar seu aplicativo para ser sem estado, modular e fracamente acoplado e usar serviços que ofereçam suporte a dimensionamento automático, balanceamento de carga e armazenamento em cache.
- **Projeto para disponibilidade e confiabilidade**: os aplicativos em nuvem devem ser capazes de tolerar e se recuperar de falhas sem afetar a experiência do usuário ou a integridade dos dados. Você deve projetar seu aplicativo para ser resiliente, tolerante a falhas e autocorretivo e usar serviços que ofereçam suporte a backup, replicação, failover e monitoramento.
- **Projeto para segurança e conformidade**: os aplicativos em nuvem devem ser capazes de proteger os dados e a privacidade dos usuários e do sistema contra acesso ou modificação não autorizados. Você deve projetar seu aplicativo para seguir o princípio do menor privilégio, criptografar dados em trânsito e em repouso, implementar mecanismos de autenticação e autorização e cumprir as leis e regulamentos aplicáveis.
- **Projeto para desempenho e eficiência**: os aplicativos em nuvem devem ser capazes de fornecer desempenho rápido e suave, minimizando o consumo e o custo de recursos. Você deve projetar seu aplicativo para otimizar a latência de rede, largura de banda e taxa de transferência, usar serviços que oferecem suporte a redes de entrega de conteúdo (CDNs), compactação, cache etc. e seguir as práticas recomendadas para otimização de código.

### Migrar e integrar sistemas e aplicativos existentes aos desafios e soluções da nuvem

Alguns dos principais desafios e soluções para migrar e integrar sistemas e aplicativos existentes para a nuvem são:

- **Desafio de compatibilidade**: os sistemas e aplicativos existentes podem não ser compatíveis com o ambiente de nuvem, especialmente se forem legados, não relacionados à nuvem ou específicos da plataforma. Isso pode exigir a modificação ou nova arquitetura dos sistemas e aplicativos para torná-los prontos para a nuvem, o que pode ser demorado, caro e arriscado. Uma solução possível é usar uma abordagem em fases para migrar os sistemas e aplicativos com base em seu nível de compatibilidade, como lift-and-shift, re-plataforma ou refatoração. Outra solução possível é usar ferramentas e serviços que podem ajudar no processo de migração, como Google Cloud Migration Center, AWS Migration Hub ou Azure Migrate.
- **Desafio de segurança e conformidade**: os sistemas e aplicativos existentes podem ter requisitos de segurança e conformidade diferentes do ambiente de nuvem, especialmente se envolverem dados confidenciais ou regulamentados. Isso pode exigir a implementação de medidas e controles de segurança adicionais para proteger os dados e a privacidade dos usuários e do sistema, bem como o cumprimento das leis e regulamentos aplicáveis. Uma solução possível é usar técnicas de criptografia, autenticação, autorização, auditoria e monitoramento para proteger os dados em trânsito e em repouso. Outra solução possível é usar ferramentas e serviços que possam ajudar na avaliação e gerenciamento de segurança e conformidade, como Google Cloud Security Command Center, AWS Security Hub ou Azure Security Center.
- **Desafio de desempenho e confiabilidade**: sistemas e aplicativos existentes podem ter expectativas de desempenho e confiabilidade diferentes do ambiente de nuvem, especialmente se envolverem alta disponibilidade, escalabilidade ou cargas de trabalho sensíveis à latência. Isso pode exigir a otimização dos sistemas e aplicativos para aproveitar os recursos e serviços da nuvem que podem aprimorar seu desempenho e confiabilidade, como escalonamento automático, balanceamento de carga, armazenamento em cache etc. Uma solução possível é usar ferramentas e serviços de teste e monitoramento de desempenho para medir e melhorar o desempenho e a confiabilidade dos sistemas e aplicativos no ambiente de nuvem. Outra solução possível é usar ferramentas e serviços que possam ajudar na otimização de desempenho e solução de problemas, como Google Cloud Operations Suite, AWS CloudFormation ou Azure DevOps.
- **Desafio de integração**: sistemas e aplicativos existentes podem ter requisitos de integração diferentes do ambiente de nuvem, especialmente se envolverem vários componentes ou dependências que precisam se comunicar ou coordenar entre si. Isso pode exigir a concepção e implementação de estratégias e soluções de integração que possam permitir a interoperabilidade perfeita entre os sistemas e aplicativos no ambiente de nuvem. Uma solução possível é usar arquiteturas orientadas a serviços ou microsserviços que possam desacoplar os sistemas e aplicativos em unidades menores, independentes e reutilizáveis. Outra solução possível é usar ferramentas e serviços que possam ajudar no desenvolvimento e gerenciamento da integração, como Google Cloud API Gateway, AWS AppSync ou Azure Logic Apps.

### Referências para Computação em Nuvem

- [Best practices for deploying your apps in the cloud -- IBM Developer](https://developer.ibm.com/articles/cl-best-practices-deploying-apps-in-cloud/)
- [Deploy your application -- Google Cloud](https://cloud.google.com/deploy/docs/deploying-application)
- [Build Cloud Applications -- Google Cloud Training](https://cloud.google.com/learn/training/application-development)
- [7 Most Common Cloud Computing Challenges - GeeksforGeeks](https://www.geeksforgeeks.org/7-most-common-cloud-computing-challenges/)
- [Five challenges to cloud adoption and how to overcome them](https://www.pwc.com/m1/en/publications/five-challenges-cloud-adoption-how-overcome-them.html)
- [Top 15 Cloud Computing Challenges [with Solution] - KnowledgeHut](https://www.knowledgehut.com/blog/cloud-computing/cloud-computing-challenges)
- [Top 10 Challenges Of Cloud Computing- That Will Turn Your World Upside Down - ThinkCloudly](https://thinkcloudly.com/top-10-challenges-of-cloud-computing/)
- [10 Best Practices to Avoid Cloud Vendor Lock-In - BMC Software](https://www.bmc.com/blogs/vendor-lock-in/)
- [What is Vendor Lock-In? 6 Tips to Avoid Getting Trapped](https://www.mendix.com/blog/vendor-lock-in-6-tips-to-avoid-getting-trapped/)
- [What is Vendor lock-in? - IONOS](https://www.ionos.com/digitalguide/hosting/technical-matters/vendor-lock-in/)
- [The Best Ways to Avoid Vendor Lock-In - InformationWeek](https://www.informationweek.com/software/the-best-ways-to-avoid-vendor-lock-in)
- [What’s cloud computing? The advantages and disadvantages](https://www.microsoft.com/en-gb/microsoft-365/business-insights-ideas/resources/whats-cloud-computing-the-advantages-and-disadvantages)
- [Advantages Of Cloud Computing -- Google Cloud](https://cloud.google.com/learn/advantages-of-cloud-computing)
- [Benefits and challenges of three cloud computing service models](https://ieeexplore.ieee.org/document/6412402)
- [Best practices for deploying your apps in the cloud](https://developer.ibm.com/articles/cl-best-practices-deploying-apps-in-cloud/)
- [Best practices in cloud applications - Azure Architecture Center](https://learn.microsoft.com/en-us/azure/architecture/best-practices/index-best-practices)
- [AWS Well-Architected - Build secure, efficient cloud applications](https://aws.amazon.com/architecture/well-architected/)
- [13 Cloud Migration Challenges and their Solutions - Simform](https://www.simform.com/blog/cloud-migration-challenges/)
- [Application Migration -- Google Cloud](https://cloud.google.com/solutions/application-migration)
- [Most Common Challenges with Cloud Migration -- Lucidchart Blog](https://www.lucidchart.com/blog/challenges-with-moving-to-the-cloud)

## Fica, vai ter bolo

Neste artigo, discutimos dois aspectos avançados da engenharia de software: desenvolvimento móvel e computação em nuvem. Comparamos as vantagens e desvantagens de aplicativos nativos e híbridos para desenvolvimento móvel e explicamos as diferenças entre IaaS, PaaS e SaaS para computação em nuvem. Esperamos que este artigo tenha lhe dado uma melhor compreensão desses tópicos e ajudado a estimular um debate entre os alunos.
