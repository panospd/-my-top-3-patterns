# Top 4 design patterns

1. ***Inversion of Control (Dependency Injection)***
A pattern I use (alsmost) always. The pattern aids in creating loosely coupled solutions by delegating dependency provision of objects to a third party entity

1. ***CQRS***
A pattern I use almost all the time. It provides freedom as separates commands with queries. It can also have a great deal of perfomance gains and simplicity as queries do not need to go through the app layer and read models can have exactly the data they need by using queries that get exactly what we need from the database without 
the need to fetch multiple aggregates first and then extract the data needed

1. ***Factory methods***
A pattern to use in replacement or in conjuction with IOC. Factory method can be a static method within the same object that creates (e.g in value objects) or separate 
classes/creators that know how to create and return implementations of interfaces that are used as dependencies. Can have a performance gain when creating dependicies dynamically only were needed instead of the constructor fucntion of the objects that use them.

1. ***Template method***
A pattern I use very often. Basically create a base abstract class with one public method that provides the template and orchestrates the execution of one or more abstract methods that will need to be implemented in the implementing classes.
So when using calling the public method it will call different implementaions of the abstract methods and hence serving each use case.

# Favourite solution architecture style
Onion architecture with a domain layer that is infrastructure agnostic
