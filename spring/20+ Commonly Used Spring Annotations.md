# 20+ Commonly Used Spring Annotations(Draft)

## Content

- [Introduction](#introduction)
- [Annotations](#annotations)
  
  - [Bean declaration](#bean-declaration)
  - [Bean injection](#bean-injection)
  - [Bean life-cycle and scope](#bean-life-cycle-and-scope)
  - [Bean construction and destruction](#bean-construction-and-destruction)
  - [Bean configuration](#bean-configuration)
  - [Property value injection](#property-value-injection)
  - [Asynchronous service](#asynchronous-service)
  - [Timer(Quartz)](#timerquartz)
  - [Features switches](#features-switches)
  - [Spring MVC](#spring-mvc)
  - [AOP](#aop)
  - [Test](#test)
  
  

## Introduction

Annotation is the most important part in Spring. We can do nothing without annotations. This doc shows 20+ annotations we may most commonly use in a Spring based project.

## Annotations

The following annotations are provided by Spring core framework, and only a few from other Spring modules like Spring MVC or Spring Data JPA.

### Bean declaration

As we all know, Spring brings a big concept IoC(or DI) in its framework. And we usually use the following annotations for bean declarations.

| Annotations | Related annotations | Path    | Attributes | Description                                                  |
| ----------- | ------------------- | ------- | ---------- | ------------------------------------------------------------ |
| @Component  |                     | on type |            | Identify a class as a Spring managed bean. No tier constraint. It can be used in all three layers. |
| @Service    |                     | on type |            | The alias for the annotation @Component. It is used to identify a class as a service bean in a business layer. |
| @Repository |                     | on type |            | The alias for the annotation @Component. It is used to identify a class as a data access object bean in a data persistence layer. |
| @Controller | @RestController     | on type |            | The alias for the annotation @Component. It is used to identify a class as a controller bean. |

`@RestController` is a convenient form of the combination of `@Controller` and `@ResponseBody`.

#### Example

```java
@Component
public class GenericToolKit {
    //...
}
```



### Bean injection
Before we get started with injection annotations, let's talk about Injection a little bit.



### Bean life-cycle and scope
@Singleton @Prototype @Request @Session @Application and websocket scope



### Bean construction and destruction

@PostConstruct @PreDestroy



### Bean configuration

@PropertySource @Profile



### Property value injection

@Value



### Asynchronous service



### Timer(Quartz)



### Features switches



### Spring MVC



### AOP



### Test



## Reference