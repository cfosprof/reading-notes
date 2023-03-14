<link rel="stylesheet" type="text/css" href="style.css">

# Class 1


<details markdown="block"><summary>Map vs forEach</summary>

### forEach

* Receives a function as an argument and executes it once for each array element, returns undefined unlike array which returns a new array

* Is a mutator method and can modify the original array with the callback function, unlike map which is immutable



### Map

* Receives a function as a parameter, then applies it to each element and returns a new array of values transformed after the original array value was passed through the function. ~Returns a new array~

* Map is also chainable, meaning you can attach reduce(), sort(), filter() and many other methods to it.

```javascript



```


</details>


<details markdown="block" default="open"><summary>Arrow Functions</summary>

* Arrow functions don't have their own bindings to `this` `arguments` or `super`, and should not be used as methods.

* Arrows cannnot be used as constructers, callling them with new throws a type error.

* Cannot use yield within their body.

#### Syntax

```javascript



() => expression

param => expression

(param) => expression

(param1, paramN) => expression

() => {
  statements
}

param => {
  statements
}

(param1, paramN) => {
  statements
}

```


<details markdown="block"><summary>Rest Parameters</summary>

* The rest parameter syntax allows a function to accept an indefinite number of arguments as an array, providing a way to represent variadic functions in JavaScript.

* 1

* 2

```javascript



```


</details>


<details markdown="block"><summary>Default Parameters</summary>

### Headertext

* 1

* 2

```javascript



```


</details>



<details markdown="block"><summary>Destructuring</summary>

### Headertext

* 1

* 2

```javascript



```


</details>





</details>



<details markdown="block"><summary>JSX</summary>

### JS in JSX with curlies



### Rules of JSX

#### 1. Return a Single root element

For a component to return multiple elements, it needs to embed them in a single parent tag.

```js

// <> also works

<div> 
  <h1>Title</h1>
  <ul>
    <li>item</li>
  </ul>
</div>

//</>

```


#### 2. All tags must be explicitly closed, for example `img`needs closing tag.

#### 3. Camel case most jsx

JSX turns into js and attributes written in JSX become keys of js objects.



</details>



## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>



### Component-Based Architecture



#### What is a “component”?

  A modular and reusable block of code that is often combined with other components to create large applications.

#### What are the characteristics of a component?

  Reusability--They are usually meant to be reused.

  Replaceable--They can be substituted with other components.

  Not context specific--Designed to operate in different environments and contexts.

  Extensible-- Additional functionality can be added to them.

  Independent--They have little dependency on other components.


#### What are the advantages of using component-based architecture?

  They're reusable, modular and easily inserted into applications, their reduced dependance on other components make them easy to test, they're flexible.

#### What is Props and How to Use it in React

  Props is just shorthand for properties and it's a feature that passes data from parent components to child components.



#### What is “props” short for?

  Answered above.


#### How are props used in React?

  They're passed as attributes to a component when it is used. Like
  ```js

  import React from 'react';

  class Header extends React.Component {
    render(){
      return <h1>Here is thy horned beast, {this.props.title}</h1>
    }
  }

  export default Header;

  ```

#### What is the flow of props?

  Unidirectional, from parent to child. The child can't pass up they're unmutable.

</details>
