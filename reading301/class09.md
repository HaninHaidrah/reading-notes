# Functional Programming Concepts

1. What is functional programming?

* In computer science, functional programming is a programming paradigm where programs are constructed by applying and composing functions. ... This allows programs to be written in a declarative and composable style, where small functions are combined in a modular manner.

2.What is a pure function and how do we know if something is a pure function?

* A pure function is a function which: Given the same input, will always return the same output. Produces no side effects
  1.Given the same input, will always return the same output.
  2.Produces no side effects.
  3.Relies on no external state.

3.What are the benefits of a pure function?

* Pure functions are much easier to read and reason about. All relevant inputs and dependencies are provided as parameters, so no effects are observed that alter variables outside of the set of inputs. This means that we can quickly understand a function and its dependencies, just by reading the function's declaration.

4.What is immutability?

* In JavaScript, only objects and arrays are mutable, not primitive values. ... A mutable object is an object whose state can be modified after it is created. Immutables are the objects whose state cannot be changed once the object is created. Strings and Numbers are Immutable.

![img](https://image.slidesharecdn.com/functionalprogrammingpowerpoint-170523093123/95/functional-programming-with-immutable-js-4-638.jpg?cb=1495532103)

5.What is Referential transparency?

* Referential Transparency emphasizes that an expression in a JavaScript program may be replaced by its value or any other variable having the same value without changing the result of the program. As a result, methods should always return the same value for the given argument without any side effects

## Node JS Tutorial for Beginners #6 - Modules and require()

1. What is a module?

* Module pattern. The Module pattern is used to mimic the concept of classes (since JavaScript doesn't natively support classes) so that we can store both public and private methods and variables inside a single object — similar to how classes are used in other programming languages like Java or Python.
In Node. js, Modules are the blocks of encapsulated code that communicates with an external application on the basis of their related functionality. Modules can be a single file or a collection of multiples files/folders

![img](https://miro.medium.com/max/1200/1*GpS8sOvkhbj-NIXNtM084g.png)

2.What does the word ‘require’ do?

* Now require() is a special function call defined as part of the CommonJS spec. In node, it resolves libraries and modules in the Node search path, now usually defined as node_modules in the same directory (or the directory of the invoked javascript file) or the system-wide search path.

3.How do we bring another module into the file the we are working in?

* To import our own Node JS module.

 >var arthmetic = require("arthmetic");

4.What do we have to do to make a module available?
 > name of instance.listen(port,())
