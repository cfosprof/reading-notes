# Class 12

## Things I want to know more about



## Terms and Concepts

<details markdown="block"><summary>Terms</summary>


```javascript

Set objects

`A value in a set may only occur once, and set() creates a new set object`

const mySet1 = new Set();

mySet1.add(1); // Set(1) { 1 }
mySet1.add(5); // Set(2) { 1, 5 }
mySet1.add(5); // Set(2) { 1, 5 }

`forEach()`

const items = ["item1", "item2", "item3"];
const copyItems = [];

// before
for (let i = 0; i < items.length; i++) {
  copyItems.push(items[i]);
}

// after
items.forEach((item) => {
  copyItems.push(item);
});


`filter()`

Copies the values passed in that return truthie

Finding prime numbers in an array
const array = [-3, -2, -1, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13];

function isPrime(num) {
  for (let i = 2; num > i; i++) {
    if (num % i === 0) {
      return false;
    }
  }
  return num > 1;
}

console.log(array.filter(isPrime)); // [2, 3, 5, 7, 11, 13]

includes() determines whether an array includes a certain value returning true or false as appropriate

const arr = ["a", "b", "c"];

arr.includes("c", 3); // false
arr.includes("c", 100); // false



```

</details>

<details markdown="block"><summary>Remember</summary>

### ThingToRemember

</details>

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

JavaScript Canvas

### 1.What does the <canvas> allow a developer to acheive?

It allows you to draw 2d graphics using javascript

### 2.What is the importance of the closing `</canvas> tag?

Any content between the opening and closing tags is fallback content that will display only if the browser doesn’t support the `<canvas>` element. 


### 3.Explain what the getContext() method does.

Takes one argument--the type of context--and returns a rendered context object

Chart.js Documentation:

### 4.What is Chart.js and how it can be brought into your project?

Chart provides chart types, plugins, and customization options.

### 5.List 3 different Chart types you can create using Chart.js.

Area Charts, Bar Charts, and bubble charts.

### 6.What are some advantages to displaying data via a chart over a table?

They're easier to look at, convey data more clearly, and don't have a bunch of elements that look exactly the same to spin your brain in circles of confusion.

### 7.How could Chart.js aid your previously created applications visually?

Well, it would certainly look prettier than my HTML table. I would have loved to use it back when I was still scraping fantasy football data from the web.

</details>