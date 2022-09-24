# Thinking in Java

> Bruce Eckel
> [Source code](https://github.com/BruceEckel/TIJ4-code/tree/master/examples)

## Preface

Programming is about managing complexity. Due to this lots of projects fail.

Sun: "We care about reducing the time and difficulty of producing robust code".

**Conclusion:** Java is not the fastest language but it conquers complexity
and reduces time of writing robust software.

## Introduction

The design of Java conditioned by the set of programming problems.

Every feature would be considered through that prism.

## Introduction to Objects

Programmer must establish association between computer and business problem.
The more difficult it is, the more expensive and unmaintainable
the program would be.

* Lisp: "All problems are lists"
* APL: "All problems are algorithmic"
* Prolog: casts all problems into chains of decisions

OOP is generic enough to cover all problems (sidenote: probably no, so
there is multiparadigm language design). OOP allows you to describe
the problem in terms of problem instead of computer.


### Basic characteristics of OOP language. Pure OOP approach `p. 16`:

**A program is a bunch of objects telling each other what to do
by *sending messages***
1. Everything is an object.
2. **A program is a bunch of objects telling each other what to do
by *sending messages***.
3. Each object has it's own memory made of objects.
4. Each object has a type. "class" is synonymous with "type"
5. All objects of a particular type can recieve same messages.

**An object has state, behaviour and identity**.
It has data, methods and unique address in memory.

First OOP language - Simula-67. Introduced keyword `class`.

Class is an Abstract Data Type - *functional concept in OOP*.

---

Best way to think about objects is as **"service providers"**. It helps
to improve the cohesiveness of the object.

**High cohesion** is a fundamental quality of software design. `p. 19`.

---

Code reuse is one of the greatest advantages of OOP languages.

**Inheritance** is very importent to OOP, but it leads to awkward and
overly complicated designs. Instead, you should first look to
**composition**, when creating new classes, since it is simpler and
more flexible.

> When Bruce talks about inheritance, it seems he means implementation of
an interface, not overriding existing functionality (at least in the examples).
And it didn't convince me that inheritance and overrides are a good thing.

Java uses **late binding** by default: means that calls of all polymorphic
method calls are calculated in runtime. `p. 26`. It is so because
the compiler can not know at compile time what code to execute, like
Box<dyn> in Rust.

Downcasting reqiure extra runtime resources.

Java uses dynamic memory allocation exclusively.

## Everything is an object
