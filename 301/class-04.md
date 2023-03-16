# Class 4

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

Reading
React Docs - Forms




<ol>

<li><h3> What is a ‘Controlled Component’?</h3></li>

A controlled component in React is a form inut component where the value of the input is controlled by the state of the component. This means that the value of the input is always the same as the value of the state.


<li><h3> Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.</h3></li>

As soon as they enter them because it's a more responsive user experience.


<li><h3> How do we target what the user is entering if we have an event handler on an input field?</h3></li>

Use the event object passed to the event handler. The object contains info about the user's input, such as the value of the input field. We can then use the target property of the event object to access the value of the input field--`event.target.value`.

<li><h3> Why would we use a ternary operator?</h3></li>

For shorter more concise if/else statements. React also uses ternary operators to conditionally render components because if/else statements can't be used in JSX.


<li><h3> Rewrite the following statement using a ternary statement:</h3></li>
```js
if(x===y){
  console.log(true);
} else {
  console.log(false);
}
```

`console.log(x === y ? true : false)`

</ol>


</details>
