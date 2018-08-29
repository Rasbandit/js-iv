# Personal Outline

## Scope

- Define Lexical (Lexical scoping is a convention used with many programming languages that sets the scope (range of functionality/accessibility) of a variable so that it may only be called or referenced from within the block of code in which it is defined. The scope is determined when the code is compiled)
- Start by making a function and logging a value from outside the function.
- make a variable with the same name inside and outside the function, what does it log?
- now try logging a value that is inside the function from outside. doesn't work.
- what happens if you make a function inside a function and log a value in the upper function? it works!

## Closures
- what happens if you return the inner function, and run it, can it access the value? spoiler, it can.
- well thats cool but why? Private data that can only be modified through methods.
- Reiterate how you can't access values inside a function in a lower scope.
- now what happens if we do this twice and get two closures!? MADNESS! and functionality.
- how can we use this? we can have a function that makes sandwiches.
- have them do practice problems 1 and 2
- lets add more functionality by making an object of functions(module pattern), closure still work!
- do iBuild, uBuild, weBuild calculator
- have them build a bank account.

## Context / this

- What is context?
  - The circumstances that form the setting for an event, statement, or idea, and in terms of which it can be fully understood
  - The parts of something written or spoken that immediately precede and follow a word or passage and clarify its meaning.
- 3 types of context explicit, implicit, default
  - default is the window
    - show example of how var is on global
  - implicit is when a method is on an object
    - show how this is the object it is attached too PP 1
  - explicit is when we set it
    - sometimes we have a function outside an object but we still want `this`
    - we can set the context of the function with .call .apply and .bind
  - arrow functions and how they effect this
    - used in setTimeout/interval
    - how it effects react and why we use it
    - its basically a bound function

## Constructor Functions

- A constructor function is a way of creating an object
- it uses the new keyword and we typically capitalize the first letter of the function
- we save the variables using the this keyword
- no return is needed
- methods can use the this keyword to access its own data

## Prototypes

- A prototype is a list of functions that the object can use to manipulate data.
- the prototype can be set for a type of custom object using the Constructor.prototype.newThing
- when we make an instance of our constructor function it will point to the prototype using the __proto property
- this saves on memory
- do practice problems

## Classes
- Classes are `Syntactic Sugar` for constructor function, it just makes life easier.
- the constructor function is nearly identical to the constructor function itself
- when we invoke a class it runs the constructor
- still need the new keyword
- adding prototype methods is just as easy as adding one to the class
https://repl.it/classroom/invite/HvHHOjq

## Extends
- (show extends equivalent if there is time)