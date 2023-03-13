# Class 13

<details markdown="block"><summary>Okkay</summary>

To store data in modern browsers we can use the `localStorage.setItem(variableToStore, value)` method. `localStorage.getItem(variableToStore)` to return it's value, and localStorage.removeItem('variableToStore') to delete it.

</details>

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

### Why would a developer use local storage for a web application?

To keep data from being cleared everytime a user refreshes their browser. This way users don't lose set preferences, performance, or satisfaction. It also helps reduce server load.

### What information should not be stored in local storage?

Personally indentifying information, passwords, and other sensitive information.

### Local storage can store what type of data? How would you convert it to that type before storing?

The 'toString' method,json.stringify, and json.parse() methods


</details>
