> NOTE: Spring is an Dependency Injection Framework.

Software Dependency Layers:

[web/ui] --depends-on--> [business/spring] --depends-on--> [data]

Most business layer should be handled via Spring Framework.

> NOTE:
> Tight coupling is considered a bad practice.
> If you are creating a class instance directly, then you are implementing a tight coupling.

Your job as a developer is to instruct spring framework to create an instance of a dependency
then inject it. In other words, you need to config how spring framework will manage your
objects.

## Spring Framework Annotations

- [@Component](https://docs.spring.io/spring-framework/docs/current/javadoc-api/org/springframework/stereotype/Component.html)

  Tells Spring to manage instances of the class that has this annotation.

- [@Autowired](https://docs.spring.io/spring-framework/reference/core/beans/annotation-config/autowired.html)

  Tells Spring to manage an instance of the class on an object or variable that has this annotation.

## Common Terminologies

- [Beans](https://docs.spring.io/spring-framework/reference/core/beans/definition.html)
  - different objects managed by spring container
- Autworing
  - Process where spring identifies beans and dependency match then populates them.
- Dependency Injection
- Inversion of Control
  - Process where spring framework creates the instance of the required dependency classes.
- Inversion of Control Container (IoC Container)
  - Usually the ApplicationContext
- Application Context
  - Where all beans are created and managed.
