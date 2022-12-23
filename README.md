
# Design Pattern

## What is pattern
Why do we need patterns? The blunt answer is we don't want to reinvent the wheel! Problems that occur frequently enough in tech life usually have well-defined solutions, which are flexible, modular and more understandable. These solutions when abstracted away from the tactical details become design patterns.

## Why do we need Design pattern ?
To making a system unknowingly in [telescoping pattern.](https://medium.com/@modestofiguereo/design-patterns-2-the-builder-pattern-and-the-telescoping-constructor-anti-pattern-60a33de7522e)


## Some suggestion to write in Object oriented design.

  - Separate out parts of code that vary or change from those that remain the same.
  - Always code to an interface and not against a concrete implementation.
  - Encapsulate behaviors as much as possible.
  - Favor composition over inheritance. Inheritance can result in explosion of classes and also sometimes the base class is fitted with new functionality that isn't applicable to some of its derived classes.
  - Interacting components within a system should be as loosely coupled as possible.
  - Ideally, class design should inhibit modification and encourage extension.
  - Using patterns in your day to day work, allows exchanging entire implementation concepts with other developers via shared pattern vocabulary.

## There are 23 Type of design pattern

  - Mention in book (Design Patterns: Elements Of Reusable Object-Oriented Software) writen by the famous gabg of four(GoF)
  - That is also divided into 3 sub suction 
    ### Creational
      - Creational design patterns relate to how objects are constructed from classes. New-ing up objects may sound trivial but unthoughtfully littering code with object instance creations can lead to headaches down the road. The creational design pattern come with powerful suggestions on how best to encapsulate the object creation process in a program.
      - There are several creational design patterns that can help you create objects in a more flexible and maintainable way. These patterns focus on creating objects in a way that is decoupled from the actual implementation of the objects being created.

      > **Abstract Factory:** This pattern provides an interface for creating families of related or dependent objects without specifying their concrete classes.

      > **Builder**: This pattern separates the construction of a complex object from its representation, allowing the same construction process to create various representations.(NOT Used in JS)

      > **Factory Method:** This pattern defines an interface for creating an object, but lets subclasses decide which class to instantiate. Factory Method lets a class defer instantiation to subclasses.

      > **Prototype:** This pattern specifies the kinds of objects to create using a prototypical instance, and creates new objects by copying this prototype.

      > **Singleton**: This pattern ensures that a class has only one instance, and provides a global access point to it.

      > **NOTE:** By using these patterns, you can create objects in a more flexible and maintainable way, and you can also improve the performance of your program by reusing existing objects instead of creating new ones.
    ### Structural
    - Structural patterns are concerned with the composition of classes i.e. how the classes are made up or constructed. 
    - Structural design patterns are concerned with how objects and classes can be composed to form larger structures. These patterns focus on creating relationships between objects to form more complex and flexible systems.

    *Here are some examples of structural design patterns:*

    > **Adapter:** This pattern allows you to adapt one interface to another, so that classes can work together that could not otherwise because of incompatible interfaces.

    > **Bridge:** This pattern decouples an abstraction from its implementation, allowing the two to vary independently.

    > **Composite:** This pattern allows you to compose objects into tree structures to represent part-whole hierarchies.

    > **Decorator:** This pattern allows you to add new behavior to existing objects dynamically by wrapping them in an object of a decorator class.

    > **Facade:** This pattern provides a simplified interface to a complex subsystem.

    > **Flyweight:** This pattern uses sharing to support large numbers of fine-grained objects efficiently.

    > **Proxy:** This pattern provides a surrogate or placeholder for another object to control access to it.

    > **NOTE:** By using these patterns, you can create more flexible and reusable systems, and you can also improve the performance of your program by reducing the number of objects that need to be created.


    ### Behavioural
    -Behavioral design patterns are concerned with the communication between objects and the way that responsibility is assigned and delegated. These patterns focus on the communication between objects and the way that responsibilities are assigned and delegated between them.

      *Here are some examples of behavioral design patterns:*

      > **Chain of Responsibility:** This pattern allows you to pass requests along a dynamic chain of objects until one of them handles the request.

      > **Command:** This pattern allows you to encapsulate a request as an object, separate from the object that executes the request.

      > **Interpreter:** This pattern allows you to represent a complex grammar in a simple language and evaluate it.

      > **Iterator:** This pattern provides a way to access the elements of an object sequentially without exposing its underlying representation.

      > **Mediator:** This pattern allows you to define a central object that coordinates communication between other objects, reducing the dependencies between them.

      > **Memento:** This pattern allows you to capture the internal state of an object and restore it later.

      > **Observer:** This pattern allows you to define a one-to-many dependency between objects, so that when one object changes state, all of its dependents are notified and updated automatically.

      > **State:** This pattern allows an object to alter its behavior when its internal state changes.

      > **Strategy:** This pattern allows you to define a family of algorithms, encapsulate each one, and make them interchangeable.

      > **Template Method:** This pattern defines the skeleton of an algorithm in a method, deferring some steps to subclasses.


      > <mark> **Visitor:** Most useful in web applications **Need more ** </mark>

      > **NOTE:** By using these patterns, you can create more flexible and reusable systems, and you can also improve the flexibility and maintainability of your program by decoupling the communication between objects.
  
### Creational (Base on the concept of creating an Object)
1. Class
   
- Factory Method
  
    > this makes an instance of serveral desired class based on interfeced data or event.

    > It's class-based creational pattern.

    > It's is use when we need to create a generic interface class/Object.

    > This pattern is frequently used when we need to manage or manipulate collections of objects that are different yet have many similar characteristics.

    > In this Pattern we create SubClasses base on the arg 

    **NOTE:** For Eg: look factory.js file 

1. Object
- Abstract Factory
    > Creating an instance of several families of classes without detailing concrete classes.

    > Provide an interface for creating families of related or dependent objects without specifying their concrete classes

    > This pattern is a like a factory pattern for similar factory 

    > It encapsulate a group of factory.

    > 1. It breaks the principle of Open-Closed Principle which gives code that is not clean; and that it is not easy to maintain when the software scales.
      1. The factoryManager class is attached to all types of objects that you want to build, creating code known as spaghetti code


   