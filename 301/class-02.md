# Class 2

\

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

  The render method is called first, generating the html for the component so the componentDidMount method can then take care of any additional tasks.

2. What is the very first thing to happen in the lifecycle of React?

  The constructor method creates an instance of the component class.


3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

  Constructor, render, componentDidMount, React Updates, componentWillUnmount




4. What does componentDidMount do?

  It performs any additional setup that requires access to the DOM before it can take place.


5. What types of things can you pass in the props?

  Data, user info, settings. Callback functions.


6. 7What is the big difference between props and state?
  
  State on the other hand, stores things like input values, open or closed detail elements, and the number of items added to a shopping cart. Propps pass data from a parent component to a child component, and are immutable and cant be changed by the child component. State is used to manage data within a component and can be changed by the component itself.


7. When do we re-render our application?

  Components are rerendered when props or state is changed.


8. What are some examples of things that we could store in state?

Input values, data fetched from an api, loading status.

</details>

## Things I want to know more about


<details markdown="block"><summary>Component Lifecycle Events</summary>

### Mounting

### Updating

### Unmounting

### Constructor

### Static getDerivedStateFromProps()

### render()

### ComponentDidMount()

### shouldComponentUpdate()

### getSnapshotBeforeUpdate()

### componentDidUpdate()

### componentWillUnmount()

</details>
