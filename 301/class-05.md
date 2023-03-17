# Class 5

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

### What is the single responsibility principle and how does it apply to components?

A software engineering principle that states a component should only have one reason to change. This is a good way to keep your code clean and easy to read.

### What does it mean to build a ‘static’ version of your application?

A version of your application without dynamic behavior. 

### Once you have a static application, what do you need to add?

Interactivity and dynamic behavior via state and user events.

### What are the three questions you can ask to determine if something is state?

Is it passed from a parent via props, does it remain unchange over time? Can you compute it based on any other state or props in your component?

### How can you identify where state needs to live?

Identify every component that rendders something based on that state, find a common owner component, and then either the common owner or a parent of theirs should own the state.

Higher-Order Functions

## What is a “higher-order function”?

A function that takes a function as an argument, or returns a function.

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

Passing a value through a function that determines whether it is greater than what it's being compared to and returns true if it is the case.


### Explain how either map or reduce operates, with regards to higher-order functions.

Map takes a function as an argument, and applies that function to each element in an array. Reduce takes a function as an argument, and applies that function to each element in an array, and returns a single value.

</details>