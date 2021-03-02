# Data Modeling

## Advatages of TDD (Test Driven Development)

[Source](https://dzone.com/articles/20-benefits-of-test-driven-development)
  - Wrtiting tests first lets you consider what you want from your code.
  - Improved quality
  - Able to identify errors and problems quickly

## beforeEach() and afterEach()

[Source](https://jestjs.io/docs/en/setup-teardown)
  - `beforeEach()` is used right before each tests are run. If you need to call a function or do logic before your test, this is where it happens.
  - `afterEach()` is the same as `beforeEach()` except it happens right after each tests. This can be used to clear state, or some kind of variable for example.

## Downsides of TDD

[Source](https://www.geeksforgeeks.org/advantages-and-disadvantages-of-test-driven-development-tdd/)
  - One disadvantage of TDD is the slow process. Writing tests to begin your developement before even writing code for your app can be slow in the beginning.

## Differences between ES6 Classes and Constructor/Prototype Classes

[Source](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#:~:text=Prototypes%20vs.-,Classes,is%20itself%20an%20object%20instance.)
  - A class constructor creates an instance of the class while a constructor in JS is just a plain old function that returns an object.
  - Using ES6 classes we have access to easier inheritance by `extends` from each class. This will inherit all atributes and methods from the parent class and making cleaner and easier than the old `.prototype` 
    for each new method we want to attach to the constructor.

This is new ES6 Classes
```
class Person {
  constructor(name){
    this.name = name
  }
  getName(){
    return this.name;
  }
}

class SuperHero extends Person {
  constructor(power){
    super(name);
    this.power = power;
  }
} 
```

This is what old Constructor/Prototype Classes would look like
```
function Person(name) {
  this.name = name;
}

Person.prototype.getName = function() {
  return this.name;
}

function SuperHero(name, power) {
  this.name = name;
  this.power = ppower;
}

SuperHero.prototype.getName = function() {
  return this.name;
}
```

## Why REST?

Uniform interface: to transfer data, the REST system applies specific actions (POST, GET, PUT and DELETE) on the resources, provided they are identified with a URI. 
This makes it easier to obtain a uniform interface that systematizes the process with the information.

## Vocab

1. Functional Programming - process of building software by composing pure functions and avoiding shared state, mutable data and side-effects. It is declarative rather than imperative.
2. Object-Oriented Programming - programming paradigm  that organizes software design around data, or objects, rather than functions and logic.
3. Class - ES6 concept of creating a object using a constructor and adding its own methods inside the class. Other classes are able to extend from parent class, meaning they inherit all the fields available fromt he parent class.
4. `super` - the super keyword is used to access and call functions on an object's parent. Used in a class to call the parent class's constructor.
5. `this` - in javascript refers to the immidiate instance/scope of where the keyword is used. 
6. Test Driven Development - test first development where you write a tests before writing enough production code to fulfill the test and refactoring.
7. Jest - a JavaScript Testing Framework.
8. Continuous Integration - development practice that requires developers to integrate code into a shared repository several times a day.
9. REST - is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other.
10. Data Model - proccess of mapping out the data requirements and resources needed to support the app/system.



