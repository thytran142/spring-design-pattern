One of the primary places it's used is the BeanFactory. This is a little bit of a modification of a traditional factory pattern. 
1. BeanFactory
2. FactoryBean

In addition to the BeanFactory, there is a FactoryBean that goes with it , that gives you this concept of a factory of factories. 

The IoC container is based on the application context. The application context extends the BeanFactory. This is where all of your configured object references are stored in the Spring Framework. It's leveraged heavily in the framework. 

##### Pattern in a Nutshell
1. Factory allows construction of similar classes of different types using a factory method.
2. Method call creates the object for you and serves it back for you.
3. Constructed objects are from classes that share an interface or parent class.

##### Why use this pattern?
1. Allow you not to worry about the class construction in more than 1 place.
2. Allow you to leverage the interface for repetitive operations.
3. Lack of construction code cleans up code and also makes copy/paste errors less likely.