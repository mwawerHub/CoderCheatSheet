## Table of Contents
[TOC]

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

## Sources:

https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design

## Other Resources:

https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882