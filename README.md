## SpringBoot Framework

> Requisitos Básicos

1. [Java Development Kit(JDK) - 1.8 ou superior](https://www.oracle.com/java/technologies/javase-downloads.html)
2. [Intellij IDEA Community Edition ou outra de sua preferência](https://www.jetbrains.com/idea/download/)
3. [Maven 3.5.2](https://maven.apache.org/)
4. [Postman](https://www.postman.com/) 
5. [PowerShell - Opcional para execução em terminal](https://en.wikipedia.org/wiki/PowerShell)

## Clonar o Projeto

cd "diretorio de sua preferencia" 

git clone https://github.com/Januario86/springboot-configuration-properties.git


## Executar o Projeto

 mvn spring-boot:run

## Arquivo Aplication Properties

spring.profiles.active=prod ou spring.profiles.active=dev 
spring.application.name=Spring Boot Configuration Project

## Rodando servidor em Desenvolvimento - (PROPERTIES e YML)

app.message = This is te property file to the  ${spring.application.name} specfic to DEV Environment

spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.url=jdbc:h2:mem:db;DB_CLOSE_DELAY=-1
spring.datasource.username=sa
spring.datasource.password=sa

> YML

app:
  message: This is te property file to the  ${spring.application.name} specfic to DEV Environment

spring:
  datasource:
    driver-class-name: org.h2.Driver
    url: jdbc:h2:mem:db; DB_CLOSE_DELAY=-1
    username: sa
    password: sa


## Rodando o servidor em Produção PROPERTIES 

spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
spring.datasource.url=<MYSQL_URL>
spring.datasource.username=<USERNAME>>
spring.datasource.password=<PASSWORD>


## Documentação

Para referência adicional, considere as seguintes seções:

* [Official Apache Maven documentation](https://maven.apache.org/guides/index.html)
* [Spring Boot Maven Plugin Reference Guide](https://docs.spring.io/spring-boot/docs/2.2.6.RELEASE/maven-plugin/)
* [Spring Web](https://docs.spring.io/spring-boot/docs/2.2.6.RELEASE/reference/htmlsingle/#boot-features-developing-web-applications)

### Guias
Os seguintes guias ilustram como usar alguns recursos concretamente:

* [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
* [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
* [Building REST services with Spring](https://spring.io/guides/tutorials/bookmarks/)


