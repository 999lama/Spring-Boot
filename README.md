# Foobar


## Spring Boot 
https://www.tutorialspoint.com/spring_boot/spring_boot_quick_guide.htm



##  What is Micro Service?

* Micro Service is an architecture that allows the developers to develop and deploy services independently

## What is Spring Boot?
* Spring Boot provides a good platform for Java developers to develop a stand-alone and production-grade spring application that you can just run.

## Why Spring Boot?
* It provides a flexible way to configure Java Beans, XML configurations, and Database Transactions.
* It provides a powerful batch processing and manages REST endpoints.
* In Spring Boot, everything is auto configured; no manual configurations are needed.
* It offers annotation-based spring application
* Eases dependency management
* It includes Embedded Servlet Container

## How does it work?
Spring Boot automatically configures your application based on the dependencies you have added to the project by using @EnableAutoConfiguration annotation.

The entry point of the spring boot application is the class contains @SpringBootApplication annotation and the main method.

Spring Boot automatically scans all the components included in the project by using @ComponentScan annotation.

## Spring Boot Starters
* Handling dependency management is a difficult task for big projects. Spring Boot resolves this problem by providing a set of dependencies for developers convenience.

## Examples
Spring Boot Starter Actuator dependency is used to monitor and manage your application. Its code is shown below −

```HTML
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
```

## Auto Configuration
* Spring Boot Auto Configuration automatically configures your Spring application based on the JAR dependencies you added in the project.

 you need to add @EnableAutoConfiguration annotation or @SpringBootApplication annotation to your main class file. Then, your Spring Boot application will be automatically configured

Observe the following code for a better understanding −

```Java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.EnableAutoConfiguration;

@EnableAutoConfiguration
public class DemoApplication {
   public static void main(String[] args) {
      SpringApplication.run(DemoApplication.class, args);
   }
}
```

