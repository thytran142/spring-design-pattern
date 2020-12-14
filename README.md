### Spring: Design Patterns
Learn by Vanessa Tran from LinkedIn Course at https://www.linkedin.com/learning/spring-design-patterns/solving-problems-with-patterns-in-spring.

#### Patterns in Spring
1. Spring is based on design patterns.
2. From its core, patterns play a role in almost every aspect of the framework.
3. Operationally, Spring itself works using patterns and supports your patterns in the process.

#### Inversion of Control (IoC) pattern
1. This is the big one.
2. The entire runtime of the framework is based on IoC.
3. Improves testability, decreases coupling, enforces coding to an interface.

#### Proxy Pattern
It means every object that you create and configure to be managed by the platform, Spring wraps one or more proxies around that. And these proxies bring major caveats to the operation of Spring. We need to pay attention to because the expected behaviour in a non-proxied class may be different than a proxied class. 

1. Since 4.0, involved in every object managed by Spring.
2. Brings some major caveats to the operation of Spring.
3. Allow addition of behaviors that we leverage throughout the framework.


#### Factory Pattern
1. IoC container is itself a factory.This factory heavily leverages the start-up as well as the run time operation of the Spring Framework.
2. First class support for factories in your code.


#### Singleton and Prototype patterns
1. Most of your objects configured for Spring leverage these 2 patterns.
2. Singleton pattern is the most popular. If you want a bean to actually be a prototype, you have to tell Spring make this a prototype otherwise it's a singleton. 
3. Singleton in Spring is not a traditional singleton implementation, but works the same. Spring is handling the construction so they are handling you a bean that acts as a singleton within your runtime of your application.


#### Template Pattern
1. Used widely in remote calls.
2. JDBC and REST are the most popular situations.
3. Also implemented by third parties to remove boilerplate code for using their tooling.

#### Model-View-Controller Pattern
1. Entire web framework is based on this.
2. Traditional web pages as well as RESTful service.
3. Not a classic pattern, but very important in Spring. 

##### Inversion of Control (core pattern)
###### What is IoC?
It is not a Gang of Four design pattern. This is architectural pattern for relegating control of dependencies to the container instead of the developer having to be responsible for the construction of those dependencies. Often, this is called Dependency Injection, though, that is only one flavor of IoC.

###### How does it work?
1. Central container constructs and maintains all object references. 
2. Hands them to other objects when needed at runtime (or startup)
3. Centralized control and management.
4. Manages your dependencies. 
5. Objects injected at runtime, not compile time.
6. Ab object accepts the dependencies for construction instead of you constructing them. 

###### Benefit of IoC
1. Reduces noise in your code. (because you are not constructing your object, you are not tightly coupled of it)
2. Reduces the defects arise form incorrect construction.

###### Application Context
1. Spring: ApplicationContext is the IoC container.
2. Leverage the configuration to create the beans and manages the dependency injections.

