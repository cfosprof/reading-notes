 # Class 1

`==` compares the reference of two objects to determine if they are the same object in memory. `.equals` compares the content or state of the two objects to see if they have the same content.

<details markdown="block"><summary>Things</summary>

[Java Basics](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

1. What does “strong typed” mean?
1. It means the language rules for handling data types is strictly enforced. Java is strongly typed and enforces strict rules that forbid things like adding an integer to a string directly. Javascript on the other hand, does not require variables to be explicitly declared with a data type, which is more flexible, but increases the potential for errors and type mismatching while also requires JS to do the work and convert before concatenating a number to a string.. Typescript is meatheadJS.
3. Also, Java is statically typed and forbids variables from changing after declaration.
3. What are the primitive data types?
1. Java has eight of them--bytes, shorts, int, long, float, double, char, and boolean.

The first response in this [Reddit thread on compiling](https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/)

[XKCD: Compiling](https://xkcd.com/303/)

1. Explain to a non-technical friend the difference in how compilation works in Java and JavaScript.
1. Java is compiled which is like serving a table a bucket of  steaks pre chopped into a form that could be consumed by all guests at the table without problem. JS on the other hand, serves the steaks whole and relies on each guest to chop it.
2. Does code complaining mean that it works correctly?
1. No, it just means the code adheres to the languages rules and doesn't catch logical errors or production of the desired output.

[Reading Java Documentation](https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/)

1. How many keywords does Java have?
1. 51 reserved keywords and 16 contextual keywords that cannot be used as identifiers in the code.
2. How do you print words to the console in Java?
1. System.out.println("hello, world")
1. adds new line character to end of output
2. System.out.print("")
1. pno new line
3. System.out.printf
1. int age = 25; double height = 1.75; String name = "Alice"; char initial = 'A'; boolean isImposter = true;
2. System.out.printf("In format %s is for string, %c for a character, %d for an integer, %.2f for a floating-point number with two decimal places, 1.  %b for a boolean, and then we provide the variables in the same order as the format specifiers" name, initial, age, height, 'isImposter')
3. Allows formatted output to the console.

</details>

# Random
You can create a Random object via the Random() constructor, which creates a new random number generator with a default seed based on the current time.

## Methods
`nextBoolean()` returns a random boolean value.
Basically there is one of these for every primitive

# Math
`Math.pow(double a, double b)` returns value of a raised to b
# LocalDateTime()
Works when timezone isn't needed
 ``"yyyy-MM-ddTHH:mm:ss"``
`LocalDateTime.now()`: Creates a `LocalDateTime` object representing the current date-time.
## Methods
`getYear()`, `getMonth()`, `getDayOfMonth()`, `getHour()`, `getMinute()`, `getSecond()`: Retrieve date-time field values for each
`plusDays(long days)`, `plusMonths(long months)`, `plusYears(long years)`, `plusHours(long hours)`, `plusMinutes(long minutes)`, `plusSeconds(long seconds)`: Adds the specified amount to the respective date-time field.

# Prep: Data Structures and Algorithms

## Watch

- [Basic Recursion](https://www.youtube.com/watch?v=vPEJSJMg4jY)
- [Data Structures in 15 Minutes](https://www.youtube.com/watch?v=sVxBVvlnJsM)
- [Big O Explained](https://www.youtube.com/watch?v=v4cd1O4zkGw)

## Read

- [Basic Data Structures](https://towardsdatascience.com/8-common-data-structures-every-programmer-must-know-171acf6a1a42)
- [Why Big O](https://triplebyte.com/blog/why-you-should-learn-big-o-and-stop-hacking-your-way-through-algorithms)

## Discussion Questions

What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

> The relationship between the elements, how elements will be accessed, the data types, and constraints that need to represented and processed.

How can we ensure that we’ll avoid an infinite recursive call stack?
> Limit recursion depth, convert to iteration when possible, and establish a base case.
>
## Basic data structures

### Arrays

An indexed structure of fixed size which can hold items of the same data type.

#### Operations

Traverse, or go through the elements and print them.
Search for an element in the array, by value or index.
Update the value of an existing element at a given index.

#### Important

Insertion and deletion cannot be done straight away because arrays are fixed in size. ==To insert you have to create a new array with increased size, copy the existing elements and add the new element same goes with deletion==

### Linked Lists

A sequential structure that consists of a sequence of items in linear order which are linked to each other. ==You have to access data sequentially random access is not possible.==

### Anatomy

Elements in linked list are known as ==nodes==
Each node contains a **key** and a pointer to its successor node, **next**
The attribute named **head** points to the first element of the linked list.
The last element is known as the tail.

### Types of list

Singly linked list Traversal of items can be done in the forward direction only.
Doubly Linked list-- Traversal of items can be done in both forward and backwards direction, which allows for an additional pointer, prev.
Circular linked list--Linked list where the prev pointer of the head points to the tail and the next pointer of the tail points to the head.

#### Operations

Search: Find the first element with the key k in the given list and returns a pointer.
Insert: Insert a key to the linked list. Insertion can be done in three ways, beginning, end, and the middle.
Delete, removes element x from given linked list.

#### Applications

## Stacks

Linear data type following LIFO. Two main operations push and pop. The top element is the most recently added and the only one that can be accessed direclty.

### Stack operations

1.  **Push**: Adds an element to the top of the stack.
2.  **Pop**: Removes the top element from the stack.
3.  **Peek/Top**: Returns the value of the top element without removing it from the stack.
4.  **IsEmpty**: Checks if the stack is empty or not. Returns true if the stack is empty, false otherwise.
5.  **Size/Length**: Returns the number of elements in the stack.

### Applications of stacks

**Undo/Redo operations**: Stacks can be used to implement undo and redo functionality in applications like text editors or image editing software.
**Syntax parsing**: Compilers and interpreters use stacks for parsing expressions and statements in programming languages.
**Backtracking**: Stacks are used in backtracking algorithms to solve problems like maze-solving, the eight-queens problem, and other combinatorial problems.
## Queues
Queues are linear data structures that follow the First In First Out (FIFO) principle, supporting enqueue (add) and dequeue (remove) operations. They are commonly used in scenarios like task scheduling, handling requests in web servers, and implementing algorithms like Breadth-First Search.
### Types

### Operations

### Application

## Hash Tables
Hash Tables are data structures that provide fast insertion, deletion, and retrieval operations using key-value pairs. They use a hash function to map keys to indices in an array. Hash Tables are widely used for caching, database indexing, and implementing programming languages' symbol tables.
### Types

### Operations

### Application

## Trees
Trees are hierarchical data structures with a root node and nodes connected by edges. They are used to represent hierarchical relationships and enable efficient searching, sorting, and insertion operations. Common types include Binary Trees, Binary Search Trees, and AVL Trees. Applications include file systems, DOM (Document Object Model) in web browsers, and decision-making in AI.
### Types

### Operations

### Application

## Heaps
Heaps are binary tree-based data structures that follow a specific ordering property (e.g., max-heap or min-heap). They are used for implementing priority queues, which are helpful in task scheduling, graph algorithms like Dijkstra's and Prim's, and for finding the kth smallest or largest element in a collection.
### Types

### Operations

### Application

## Graphs
Graphs are data structures consisting of nodes (or vertices) connected by edges, representing complex relationships between objects. They can be directed or undirected, weighted or unweighted. Graphs are widely used in social networks, transportation networks, and recommendation systems, with algorithms like Depth-First Search, Breadth-First Search, and pathfinding algorithms such as Dijkstra's and A*.
### Types

### Operations

### Application
