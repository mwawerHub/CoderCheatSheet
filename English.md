## Table of Contents
- [Table of Contents](#table-of-contents)
- [Object oriented programming - OOP](#object-oriented-programming---oop)
  - [Classes:](#classes)
  - [Obiekt](#obiekt)
- [SOLID](#solid)
  - [S: Single responsibility principle](#s-single-responsibility-principle)
  - [O: Open(for extensions)/Closed(for modifications)](#o-openfor-extensionsclosedfor-modifications)
  - [L: Liskov substitution](#l-liskov-substitution)
  - [I: Interface segregation](#i-interface-segregation)
  - [D: Dependency Inversion](#d-dependency-inversion)


***

## Object oriented programming - OOP

Object oriented programming is a concept which describes application logic as a set of classes and its dependencies. In object oriented programming we extend our application functionality by implementing new classes which represent concrete abstraction and its functionality. Object - instance of class has different states and implements its behavior with methods.


### Classes:

Classes are a part of object oriented languages. Their role is to describe application logic. Classes consist of elements such as:
* fields
* constructors
* properties
* functions
* events

Class is the definition of what an object whttp://www.albahari.com/nutshell/
ould look like.


### Obiekt
The object is an instance of class. Objects are created using the *new* keyword:
*var classInsctane = new Class();*
The above expression will call the class constructor. If the constructor is not implemented then the default constructor will be called.

Sources:

ENG: https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/classes
ENG: https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/intro-to-csharp/object-oriented-programming
PL: https://cezarywalenciuk.pl/blog/programing/kurs-obiektowosc-w-c-klasa-i-obiekty-01
Other Resources:

http://www.albahari.com/nutshell/

***

## SOLID
### S: Single responsibility principle

Class should be responsible only for one functionality. If you need to modify a class, you should have one concrete reason to do so.


### O: Open(for extensions)/Closed(for modifications) 

Class should be written in a way which allows the extension to application functionality without the necessity to make changes in the code. Polymorphism and Inheritance are vital paradigms of object-oriented programming which allows to preserve an open/close principle


### L: Liskov substitution

All of the base class functionalities should apply to derived classes. In other words, the derived class should be substitutable for its parent class. The name of the rule comes from the name of the American programmer Barbara Liskov.


### I: Interface segregation

Design your interfaces to deliver concrete and similar methods to implementing classes. Avoid situations when an interface forces a class to implement methods which it does not need or should not be able to use.


### D: Dependency Inversion

When building dependencies between objects, base them on abstractions rather than concrete types. Provide polymorphic interfaces to make classes less tight-coupled and allow the dependency injection pattern to be used.

Sources:

ENG: https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design
PL: https://www.p-programowanie.pl/paradygmaty-programowania/zasady-solid

Other Resources:

https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882