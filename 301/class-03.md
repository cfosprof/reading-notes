# Class 2

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

#### 1. What does .map() return?

Map returns a copy of the original array with the changed values from the function.

#### 1. If I want to loop through an array and display each value in JSX, how do I do that in React?

```jsx
{myArray.map((value) => (
        <p>{value}</p>

```

#### 1. Each list item needs a unique ____.

key from their siblings


#### 1. What is the purpose of a key?

A special string attribute you need when creating lists of elements, they help React identify which items have changed, added or are removed.


#### 1. What is the spread operator?

A JS feature that spreads or expands the elements of an iterable object, such as an array or an object into a new array or object.

```js
let newArray = [...myArray, 4, 5];

let newObject = {...myObject, key: value, key: value}

let new Array = [...array1, ...array2]
```

#### 1. List 4 things that the spread operator can do.

Concatenate arrays, copy arrays, merge objects, pass arguments from an array as separate arguments to a function.

#### 1. Give an example of using the spread operator to combine two arrays.

Look above

#### 1. Give an example of using the spread operator to add a new item to an array.

Look above

#### 1. Give an example of using the spread operator to combine two objects into one.

Look above


#### 1. n the video, what is the first step that the developer does to pass functions between components?

Define the function

#### 1. In your own words, what does the increment function do?

increments a value by a number

#### 1. How can you pass a method from a parent component into a child component?

via prop

#### 1. How does the child component invoke a method that was passed to it from a parent component?

calls the method as a prop.

</details>

