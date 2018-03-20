---
title:  "Chegou o Spring Boot 2.0"
header:
  teaser: "https://farm5.staticflickr.com/4076/4940499208_b79b77fb0a_z.jpg"
header:
  image: https://github.com/vinicius3w/vinicius3w.github.io/blob/master/images/header-by-jesus-kiteque-224069.jpg?raw=true
  caption: "Photo credit: @ikukevk on [**Unsplash**](https://unsplash.com/photos/w7ZyuGYNpRQ)"
categories: 
  - Development
tags:
  - programação
  - Engenharia de Software
  - desenvolvimento
  - boas práticas
  - microservices
  - spring boot
---

Neste semestre estou ministrando pela primeira uma disciplina inteiramente focada em investigar o desenvolvimento de aplicações "nativas de nuvem" com arquitetura baseada em microservices (mais informações aqui: [Desenvolvimento de Aplicações com Arquitetura Baseada em Microservices](https://github.com/vinicius3w/if1007-Microservices). Como ferramenta adotei o [Spring Boot](https://projects.spring.io/spring-boot/) dado o conjunto de facilidades e benefícios acelerados que teria com o seu uso.

O foco ficaria muito mais nos conceitos e decisões de projetos do que em questões de codificação, digamos assim. Estratégia também adotada na disciplina de Engenharia de Software (maiores informações aqui: [
Engenharia de Software (if977)](https://sites.google.com/a/cin.ufpe.br/if977/)), que também ministro, e motivou a escolha da suite de ferramentas pra ela.

Bem, o Spring Boot 2 acabou de ser lançado e a comunidade já está pronta para vê-lo em ação nos próximos meses. Este lançamento coroa o ciclo de 17 meses de trabalho e mais de 6800 commits por 215 colaboradores diferentes. Existem algumas características realmente interessantes neste lançamento, e vou tentar abordar aqui.

## História

Antes de tratar do que há de novo, é interessante contextualizar um pouco a história do framework Spring Boot. Em uma publicação num blog publicada em agosto de 2013, [Phil Webb anunciou o lançamento do primeiro marco de um novo projeto chamado Spring Boot](https://spring.io/blog/2013/08/06/spring-boot-simplifying-spring-for-everyone/).

> Spring Boot aims to make it easy to create Spring-powered, production-grade applications and services with minimum fuss. It takes an opinionated view of the Spring platform so that new and existing users can quickly get to the bits they need. You can use it to create stand-alone Java applications that can be started using ‘java -jar’ or more traditional WAR deployments.

Cerca de 9 meses depois, em abril de 2014, o Spring Boot 1.0 foi lançado. Desde então, houveram inúmeros lançamentos menores e evluções até alcançarmos o estágio atual, conforme pode ser conferido neste post do [Dan Vega](http://therealdanvega.com/blog/2018/03/01/what-is-new-spring-boot-2?utm_content=educational&utm_campaign=2018-03-20&utm_source=email-sendgrid&utm_term=554668&utm_medium=760202).

## O que há de novo no Spring

A primeira grande evolução é a atualização para o [Spring Framework 5](https://springframework.guru/what-is-new-with-spring-framework-5/), lançado em setembro de 2017. O Spring Framework 5 apresenta uma longa lista de novos recursos, mas vamos destacar apenas alguns.

### O que há de novo no Spring Framework 5

- **Java 8+ Baseline**: Para criar aplicações baseadas Spring Framework daqui pra frente, o requisito mínimo é o Java 8. Inicialmente pode até parecer uma ótima  mudança para os desenvolvedores, mas, de fato, é ainda maior para a equipe Spring. Isso deu a eles a chance de fazer algumas mudanças importantes que tornaram viável atualizar a base de código para todos os novos recursos no Java 8, como Lambdas e streams. Isso não apenas melhora a legibilidade do código, mas também oferece algumas melhorias de desempenho no núcleo do framework.
- **Suporte ao Java 9**: Se você pretende usar o Java 9, terá que se atualizar para o Spring Framework 5 e, portanto, precisa atualizar para o Spring Boot 2. Provavelmente muitos não estão utilizando em produção, ainda, a última versão do Java, mas essa pode ser considerada uma ótima chance para começar a brincar com as novas funcionalidades desses dois frameworks.
- **Spring MVC**: Por enquanto o Spring MVC não é o personagem principal desta história, mas houveram algumas atualizações agradáveis. Não vamos abordá-las aqui, mas dá para conferir na documentação do [Spring Framework 5](https://github.com/spring-projects/spring-framework/wiki/What%27s-New-in-Spring-Framework-5.x#spring-web-mvc).
- **Spring Webflux**:
The reactive stack is our main character in the story of Spring Framework 5. This is a different way of thinking but fortunately for us, we don’t have to learn a whole new way of writing applications. Spring WebFlux is a fully asynchronous and non-blocking web framework built from the ground up allowing us to handle a massive number of concurrent connections. While this is a complete paradigm shift it is really easy to get started.

![]({{ BASE_PATH }}/images/2018-03-20-chegou-o-spring-boot-2/reactive_stack.png)

- **Kotlin**: O suporte a Kotlin foi adicionado ao <http://start.spring.io>, mas no Spring Framework 5 há suporte dedicado para a linguagem. Com o suporte dedicado, surgiram alguns novos recursos interessantes que podem ser vistos em detalhes [aqui](https://github.com/spring-projects/spring-framework/wiki/What%27s-New-in-Spring-Framework-5.x#kotlin-support).
- **Testes**: A maior mudança na área de testes é o suporte completo para o modelo de programação e extensão Jupiter do JUnit 5. Quando criamos uma nova aplicação Spring Boot 2, ainda estamos usando JUnit 4 por padrão, porém é uma mudança simples migrar para JUnit 5.

### O que há de novo no Spring Boot 2

**Atualizações de bibliotecas de terceiros**

Com a nova versão do Spring Boot, a equipe Spring teve a oportunidade de atualizar várias "dependências".

- Thymeleaf 3 (O Thymeleaf starter agora inclui ``thymeleaf-extras-java8time``)
- Jetty 9.4
- Tomcat 8.5
- Hibernate 5.2
- Flyway 5
- Gradle 4

**Reactive Spring Data & Spring Security**

Como o Spring WebFlux, o Spring Data também fornece suporte para aplicações reativas. Atualmente, Cassandra, MongoDB, Couchbase e Redis possuem suporte a APIs reativas. O Spring Boot inclui starter-POMs para todos eles, o que deve facilitar demais.

Também há a possibilidade agora de usar o Spring Security 5.0 nas aplicações reativos. Quando o Spring Security está no classpath, a configuração automática é fornecida para aplicativos WebFlux.

**Actuator**

O Spring Boot Actuator não é nenhuma novidade, mas foi completamente reescrito. O Actuator expõe os _endpoints_ automaticamente para obter informações sobre esse status de sua aplicação. O Actuator foi escrito para dar suporte aos novos requisitos e funcionalidades providas pelo stack reativo. Algumas das mudanças no Actuator:

- Redesign para trabalhar tanto com servlet & reactive
- Status & health (todos os detalhes) foram separados
- Modelo de segurança simplificado
- Migração para o micrometer (tipo o SLF4J mas para métricas)
- Melhoria nas Estruturas JSON
- Processo simplificado para a criação de Endpoints definidos pelo usuário
  - @Endpoint
  - @WebEndpoint
  - @JmxEndpoint

Esta pode ser uma área em que as pessoas tenham problemas para atualizar por causa das mudanças no modelo de segurança. Por padrão, todos os endpoints da web estão disponíveis abaixo do caminho ``/actuator`` com URLs na forma ``/actuator/{id}``. O caminho base do ``/actuator`` pode ser configurado usando a propriedade ``manage.endpoints.web.base-path``.

Existe um documento detalhado para a Spring Boot Actuator Web API Endpoints [disponível aqui](https://docs.spring.io/spring-boot/docs/2.0.x/actuator-api/html/).

**Segurança Simplificada**

No Spring Boot 2.x, um dos principais objetivos foi simplificar a configuração de segurança e facilitar a segurança personalizada. Por padrão, tudo está seguro, incluindo recursos estáticos e os pontos finais do Actuator. Se o Spring Security estiver no classpath, o Spring Boot irá adicionar a anotação @EnableWebSecurity e contar com a negociação de conteúdo do Spring Security para decidir qual mecanismo de autenticação usar.

Uma vez que os desenvolvedores decidam que querem adicionar uma segurança personalizada, a configuração de segurança padrão fornecida pelo Spring Boot será desativada completamente. Neste ponto, os desenvolvedores precisam definir explicitamente todos os bits que desejam proteger. Isso significa que a configuração de segurança está agora em um só lugar e evita qualquer tipo de problemas com os ``WebSecurityConfigurerAdapters`` existentes.

**Suporte a HTTP/2**

É difícil de acreditar, mas a especificação HTTP 1.1 foi lançada em **1996**. Não precisamos nem dizer isso, mas a web de hoje em dia é **muito** diferente. Se você quiser habilitar o HTTP/2 em suas aplicaçõess Spring MVC ou WebFlux, você pode usar a seguinte propriedade.

```java
server.http2.enabled=true
```

Claro que isso também depende do servidor web escolhido e do ambiente da aplicação, já que esse protocolo não é suportado "_out-of-the-box_" a pelo JDK8. [Verifique a documentação para obter mais detalhes](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/howto-embedded-web-servers.html#howto-configure-http2).

**Configuration Properties**

No Spring Boot 1.x, essa noção de ligação relaxada ("_relaxed binding_") foi suportada e tudo isso significava que havia várias maneiras de criar um nome de propriedade (_camel case, underscore, hyphen_) e todos se vinculariam à mesma propriedade.

Isso ainda funciona da mesma forma, mas o que eles apertaram foi a maneira como você lê variáveis em seu próprio código. A anotação @Value é um recurso de contêiner central e não fornece os mesmos recursos que as propriedades de configuração type-safe.

![]({{ BASE_PATH }}/images/2018-03-20-chegou-o-spring-boot-2/2018-02-28_07-12-58.png)

<https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/boot-features-external-config.html#boot-features-external-config-relaxed-binding>

**Métricas**

As métricas do Spring Boot foram substituídas por Micrometer, que está sendo desenvolvido pela Pivotal.

O Spring Boot Actuator fornece gerenciamento de dependência e configuração automática para Micrometer, uma fachada de métricas de aplicações que oferece suporte a vários sistemas de monitoramento, incluindo:

* [Atlas](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-atlas)
* [Datadog](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-datadog)
* [Ganglia](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-ganglia)
* [Graphite](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-graphite)
* [Influx](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-influx)
* [JMX](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-jmx)
* [New Relic](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-newrelic)
* [Prometheus](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-prometheus)
* [SignalFx](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-signalfx)
* [Simple (in-memory)](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-simple)
* [StatsD](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-statsd)
* [Wavefront](https://docs.spring.io/spring-boot/docs/2.0.x/reference/html/production-ready-metrics.html#production-ready-metrics-export-wavefront)

![]({{ BASE_PATH }}/images/2018-03-20-chegou-o-spring-boot-2/2018-02-28_06-59-52.png)

Mais informações sobre o Micrometerm visite <https://micrometer.io/>

**Quartz Scheduler**

O Spring Boot 2 fornece suporte para o Quartz Scheduler que pode ser usado através do iniciador dedicado ``spring-boot-starter-quartz``. Tanto no armazenamento na memória quanto JDBC podem ser configurados.

```xml
<dependency>
	<groupId>org.springframework.boot</groupId>
	<artifactId>spring-boot-starter-quartz</artifactId>
</dependency>
```

**HikariCP Connection Pool**

O pool de conexão padrão mudou do Tomcat para HikariCP. Se antes era utilizado ``spring.datasource.type`` para forçar o uso do Hikari em uma aplicação baseado no Tomcat, agora não há mais necessidade. Da mesma forma, se preferir ficar com o pool de conexão do Tomcat, basta adicionar o seguinte à sua configuração:

```java
spring.datasource.type=org.apache.tomcat.jdbc.pool.DataSource
```

**Dev Tools**

Por padrão, cada vez que a aplicação é reiniciada, um relatório que mostra o delta de avaliação de condição é registrado. O relatório mostra as mudanças na configuração automática da sua aplicação à medida que ocorrem as alterações como, por exemplo, adicionar ou remover beans e definir propriedades de configuração.

Para desativar o registro do relatório, defina a seguinte propriedade:

```java
spring.devtools.restart.log-condition-evaluation-delta=false
```

**JUnit 5**

Conforme já dito anteriormente, o padrão para um aplicativo Spring Boot é ainda usar o JUnit 4. Se quiser mudar para o JUnit 5, será preciso excluir JUnit 4 do teste de inicialização inicial do spring boot e adicionar as dependências necessárias. 

```xml
<dependencies>
	<dependency>
		<groupId>org.springframework.boot</groupId>
		<artifactId>spring-boot-starter-test</artifactId>
		<scope>test</scope>
		<exclusions>
			<exclusion>
				<groupId>junit</groupId>
				<artifactId>junit</artifactId>
			</exclusion>
		</exclusions>
	</dependency>
	<dependency>
		<groupId>org.junit.jupiter</groupId>
		<artifactId>junit-jupiter-api</artifactId>
		<scope>test</scope>
	</dependency>
	<dependency>
		<groupId>org.junit.jupiter</groupId>
		<artifactId>junit-jupiter-engine</artifactId>
		<scope>test</scope>
	</dependency>
</dependencies>
<build>
	<plugins>
		<plugin>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-maven-plugin</artifactId>
		</plugin>
		<plugin>
			<groupId>org.apache.maven.plugins</groupId>
			<artifactId>maven-surefire-plugin</artifactId>
			<dependencies>
				<dependency>
					<groupId>org.junit.platform</groupId>
					<artifactId>junit-platform-surefire-provider</artifactId>
					<version>${junit-platform.version}</version>
				</dependency>
			</dependencies>
		</plugin>
	</plugins>
</build>
```

Este é um post baseado no artigo publicado pelo [Dan Vega](http://therealdanvega.com/blog/2018/03/01/what-is-new-spring-boot-2?utm_content=educational&utm_campaign=2018-03-20&utm_source=email-sendgrid&utm_term=554668&utm_medium=760202).
