# Class 9

## Reading Objectives

What is a module?
<details markdown="block"><summary>Things</summary>



### 1. What is a module?

A self contained piece of code that can be used in other programs

### 2. What does the word ‘require’ do?

Imports a modue or specific function froma  module into a current file. WHen a module is required, the contents are made available to the current file.

### 3. How do we bring another module into the file the we are working in?

const myModule = require('./myModule.js');

### 4. What do we have to do to make a module available?

function myModule() {
  // do stuff
}
module.exports = myModule;

### 5. What is functional programming?

Programming that focuses on functions and their inputs and outputs.

### 6. What is a pure function and how do we know if something is a pure function?

A function that has no side effects and always returns the same output given the same input. If a function has side effects, it is not pure.

### 7. What are the benefits of a pure function?

Predictability, maintainability, and testability.

### 8. What is immutability?

The inability to be changed.

### 9. What is Referential transparency?

The property of a function that always returns the same output given the same input.

</details>