## Table of Contents
- [Table of Contents](#table-of-contents)
- [Object oriented programming - OOP](#object-oriented-programming---oop)
  - [Classes:](#classes)
  - [Object](#object)
- [SOLID](#solid)
  - [S: Single responsibility principle](#s-single-responsibility-principle)
  - [O: Open(for extensions)/Closed(for modifications)](#o-openfor-extensionsclosedfor-modifications)
  - [L: Liskov substitution](#l-liskov-substitution)
  - [I: Interface segregation](#i-interface-segregation)
  - [D: Dependency inversion](#d-dependency-inversion)
- [Computational complexity](#computational-complexity)
  - [Time complexity](#time-complexity)
  - [Memory complexity](#memory-complexity)
  - [Types of notations](#types-of-notations)
  - [Types of estimations:](#types-of-estimations)


***

## Object oriented programming - OOP

Object oriented programming is a concept which describes application logic as a set of classes and its dependencies. In object oriented programming we extend our application functionality by implementing new classes which represent concrete abstraction and its functionality. Class is a reusable blueprint of code which provides attributes and behaviour of objects. The object is an instance of class. It has specific values of its attributes and implements its behavior with methods.


### Classes:

Classes are a part of object oriented languages. Their role is to describe application logic. Classes consist of elements such as:
* fields
* constructors
* properties
* functions
* events

Class is the definition of what an object whttp://www.albahari.com/nutshell/
ould look like.


### Object
The object is an instance of class. Objects are created using the *new* keyword:
*var classInsctane = new Class();*
The above expression will call the class constructor. If the constructor is not implemented then the default constructor will be called.

Sources:

* ENG: https://www.educative.io/blog/object-oriented-programming
* ENG: https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/classes
* ENG: https://docs.microsoft.com/en-us/dotnet/csharp/tutorials/intro-to-csharp/object-oriented-programming
* PL: https://cezarywalenciuk.pl/blog/programing/kurs-obiektowosc-w-c-klasa-i-obiekty-01

Other Resources:

* http://www.albahari.com/nutshell/

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


### D: Dependency inversion

When building dependencies between objects, base them on abstractions rather than concrete types. Provide polymorphic interfaces to make classes less tight-coupled and allow the dependency injection pattern to be used.

Sources:

* ENG: https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design
* ENG: https://www.educative.io/blog/solid-principles-oop-c-sharp
* PL: https://www.p-programowanie.pl/paradygmaty-programowania/zasady-solid

Other Resources:

* https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882

***

## Computational complexity

A common way of describing an algorithm's complexity is an estimate.

### Time complexity

Time complexity is the algorithm's execution time.

### Memory complexity

Memory complexity is the size of work memory used by an algorithm

### Types of notations

<b>Big-O notation:</b>

Most popular type of estimation. It is described by a function *g(n)* which holds the property:<br> *∀n⩾n0:f(n)⩽c∗g(n)*<br>
At some point (*n0*) when we multiply *g(n)* function by some constant *c*, the *g(n)* function will always be greater than the function which describes an algorithm. We call that an upfront estimate.

<b>Ω Notation:</b>

This notation is the reverse of Big-O notation. So the estimation will be described by the function which holds the property:<br>
*∀n⩾n0:f(n)⩾c∗g(n).*<br>
At some point (*n0*) when we multiply *g(n)* function by some constant *c* the *g(n)* function will always be less than the function which describes an algorithm. We call that a lower estimate.

### Types of estimations:

* Ο(*1*) - Constant time. Fixed number of operations.
* O(*log n*) - Logarithmic time. Complexity depends on a *log n* function result. Typically used for algoriths which halves the number of operations in each iteration.
* O(*n*) - Linear time. Fixed number of operations which vary on the n size.
* O(*n2*) - Quadratic time. The number of operations can take up to n^2.

Sources:

* ENG: https://codility.com/media/train/1-TimeComplexity.pdf
* ENG: https://cs.stackexchange.com/questions/16461/memory-complexity
* PL: http://cpp0x.pl/kursy/Teoria-w-Informatyce/424
* PL: https://www.samouczekprogramisty.pl/podstawy-zlozonosci-obliczeniowej/