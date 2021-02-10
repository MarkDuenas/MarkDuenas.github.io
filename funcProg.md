# Functional Programming

## What is functional programming?
  - Functional programming is a programming paradigm, a style of building the structure and elements of computer programs, 
    that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.
    
## Pure Functions
  - returns the same results if given same arguments
  - does not cause any observable side effects
  - Benefit is the code is easier to test, unit test pure functions with different contexts

## Immutability
  - When data i simmutable, its state cannot change after it's created.
  - If you want to change it, you need to create a new object with new values.
  - Use recursion on immutable objects

## Referential transparency
  - if a function consistently yields same results for the same input
  - pure function + immutable data = referential transparency

## Functions as first-class entities
  - Idea to treat functions as values and pass functions like data
  - refer to it from constants and variables
  - pass it as a parameter to other functions
  - return it as result from other functions

## Higer-order functions
  - take one or more functions as arguments
  - returns a function as its result

## Filter
  - expects true or false valuie to determine if the element should or should not be included in the result collection.
  
## Map
  - transforms a collection by applying a function to all of its elements and building a new collection from the returned values.
  - returns a new array
  
## Reduce
  - receive a function and a collection and return a value created by combining items
  
  
