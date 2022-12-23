
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


   