# Class 2

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>


### 1.How would you describe an object to a non-technical friend you grew up with?

an object is basically a collection of data. Much like a box holding multiple items and we can access those items through calling the box.

### 2.What are some advantages to creating object literals?

They're easy to create, readable, flexible and contain any data type, reusable, and dynamic.

### 3.How do objects differ from arrays?

Arrays are ordered lists of valuies where each item is accessible by index, where as objects are key value pairs.

### 4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.

When trying to access a dynamic value stored in a value in an objects properties.

### 5. Evaluate the code below. What does the term this refer to and what is the advantage to using this?

```js
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

`this` refers to the object dog, and it makes the function more flexible and reusable. 

### 6. What is the DOM?

The Document Object Model (DOM)

### 7. Briefly describe the relationship between the DOM and JavaScript.

Javascript manipulates the element within the DOM to chang webpages.

</details>;


Use curly braces and comma separated key value pairs

functions that are stored in objects are reffered to as methods

```js
let myArr = ['Chris', 31, true 'student'];

let person = {
  name: 'Chris',
  age: 31,
  isRemote: true,
  title: 'Student',
}
```

calling functions

dot notation:
`object.key`

or 

bracket notation
["Is Remote"]

assigning values

`person.interests = ['celebs', 'tattoos', 'art']`;


```js



```
