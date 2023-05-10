



## Inheritance
* Enables us to reuse code by creating new classes based on existent classes, ya know kind of like generational wealth. 
* A subclass is a class that inherits from other classes
* The superclass is the parent class.
* Has access to all members of the super class
* can overwrite methods of super class.
* Can add new methods to the superclass
* 



## Hashsets
==Unordered, unique Hash table, Not thread-safe, can contain null, Unique(non duplicates), set==
* A hashset is a collection of objects that are unique, ==do not allow duplicates.==
* Implemented using a hash table, which is a data structure that stores data in buckets based on their hash codes.
* ==Unordered==, so the order elements are added to the set is not preserved.
* ==Not thread safe==, they cannot be safely accessed by multiple threads at the same time.
* Are mutable
* HashSets ==can contain null values==
* 
### Example of how and why it is used
* Used to store a collection of ==unique objects==, for example you can use a hashset to store a list of unique users who visited your website.
* They can also be used to **implement a set data structure**
* They're fast for lookup operations 
### Real-world examples:
* Used to store a set of cookies a user has accepted
* To store the set of unique values in a column
* cryptography, HashSets are often used to store the set of possible keys
* **Storing a list of unique words:** A spell checker might use a HashSet to store a list of all unique words in a dictionary.
* 

## Linked Lists
# Class 6

## Linked Lists
### Nodes, dynamic, data, pointer, Sequential, 
### Key Info
* Series of nodes.
* They are sequential, linear order. 
* Each node has a piece of data and a reference--pointer--to the next node in the list.
	* `data` and `next`
* Dynamic data structures--can grow or shrink as needed.
	* This makes them ideal for situations where you don't know the size in advance
	* Or situations where data set needs to be able to change frequently.
* Often used in applications where it is important to add or remove elements of the list quickly.
	* For example, queues and stacks.
* Ideal for:
	* Storing, tracking, and simulating data. Also efficient at traversing data in either forward or backward order.
* Not ideal for Sorting or accessing data by index due to their lack of index.


## Ideal linked list implementations
* Storing Player Data
	* Due to their easily accessible data, they're ideal for storing player data--such as name, position, team, and stats. 
	* They can also be used to track player performance and identify players who are trending up or down.

## Not good implementations:
* They're not well suited for sorting or accessing data by index, and for this reason leaderboard by position and stat would be a bad choice because you'd have to start from the beginning and go through every player before knowing whether a player was the longest
* In short, they are not good for ranking players, searching for players, calculating stats, or generating sports.
* They are good for Storing data and tracking its changes as long as it doesn't require sorting or accessing data by index or in a random order.




### Java Specific info.
Linked lists created via LinkedList() constructor.
Add an element to beginning via `oddFirst()`
Add end `addLast()`
`removeFirst()` and `removeLast()`
To iterate over linked list you can use the `forEach` method.
#### The node Class
```java
class Node {
    int data;
    Node next;
    
    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

```

```java
// Add elements
add(E e)
add(int index, E e)
addFirst(E e)
addLast(E e)

// Remove elements
remove()
remove(int index)
remove(Object o)
removeFirst()
removeLast()

// Access elements
get(int index)
getFirst()
getLast()

// Search elements
indexOf(Object o)
contains(Object o)

// Modify elements
set(int index, E e)

// Size or Empty
size()
isEmpty()

```

#### List--Ideal for storing and manipulating a collection of objects.
```java

// Create a list of integers
List<Integer> list = new ArrayList<>();

// Add an integer to the list
list.add(1);

// Remove an integer from the list
list.remove(0);

// Get the element at a specific index
int element = list.get(0);

// Iterate over the list
for (int i = 0; i < list.size(); i++) {
  System.out.println(list.get(i));
}

//For each
for (Integer value : myList) {
    System.out.println(value);
}


```

#### Dequeue Ideal for adding and removing from beginning, ending, and traversing in reverse.
Time complexity: LinkedList provides O(1) time complexity for inserting or removing elements at the beginning or end of the list
```java
// Create a deque of strings
Deque<String> deque = new ArrayDeque<>();

// Add a string to the beginning of the deque
deque.addFirst("Hello");

// Add a string to the end of the deque
deque.addLast("World");

// Remove a string from the beginning of the deque
String firstElement = deque.removeFirst();

// Remove a string from the end of the deque
String lastElement = deque.removeLast();

// Iterate over the deque in reverse order
for (int i = 0; i < deque.size(); i++) {
  System.out.println(deque.removeLast());
}

```
## Verbose first set of notes

### Details
* **Linked lists** data structures consisting of a series of nodes, each of which contains data and a pointer to the next node. 
* Linked lists are **dynamic** and can grow or shrink as needed, which makes them a good choice for storing data that is not known in advance, such as the search results of a search or the items in a shopping cart.

- **Linked lists** can be used to **store**, **track**, and **simulate** data, but are not well-suited for **sorting** or **accessing** data by index, but they are **efficient** for **traversing** data in either forward or backward order.
### Key Details
* Each node consist of two things: data and a pointer to the next node.
* The first node of a linked list is called the head.
* The last is the tail.
* They can be singly or doubly linked. Single only points to next node in the list, doubly to both **next** and **prev**
### Usage
* Storage: Well suited for storing data that is not known in advance such as items in a shopping cart or results of a search. They're good for data constantly changing because they can be easily placed and removed from a slot once accessed. 
	* Note this does not mean displaying the search results data. They are not well suited for displaying results, because accessing a given element would require transversing all elements proceeding it to select it--where as others could access it by index. They're bad for data that needs to be sorted or that needs to be accessed frequently, because they're not indexed. It's like going to costco for the first time and not knowing where things are, you look in this slot, then the next then the next and so on. With indexes it's like knowing where something is and going straight to it without looking into the ohter slots. 
* Sorting: Linked lists can be used to sort data quickly and efficiently. They can easily be traversed in forwards or backwards order.
	* Again, they're good at sorting, but not accessing sorted data.
* Linked lists can be used to search for data quickly and efficiently.
* Traversing  Linked lists can be traversed in either forward or backward order.
### Real World Examples
#### walk in Dr vs appointment doctor
Linked list are ideal for situations like walk in hours where you're not sure how many patients will show up, what ailments they're going to have, and whether you'll be able to fit them into the allotted space of time between them and the next person. The next person doesn't hold the space of their index, so you can begin seeing the next person before the last persons time slot ended. It would take longer to gather their records since you didn't know their index ahead of time. It's also easier to add and remove from the list because you just change the pointer to next, but not knowing person fives index makes it difficult to efficiently handle them when they show up. Appointment systems, however, would not work as efficiently. Accessing people takes longer, and requires too much transversing.
#### Storing browser history--Useful in back button
They're good for storing the history in your web browser because they store the url and have a pointer that points to the next node. But accessing them doesn't work well because you need to traverse through the history only looking at one url at a time: the next one. They're good at the back button because they don't traverse through much, but to get to yesterdays info you would need to scroll through all the old data--which is why searching for a page by index in the search bar is faster.

### Real world use cases they wouldn't be useful for:
Search engine results: Search engine results that weren't indexed by relevance or date would return a bunch of junk you needed to read, decide it wasn't relevant, and move on. 

Linked lists would not be useful for storing the list of files in a directory if you need to access the files in a random order, so looking for a particular item would require you to go through all the items before it that were not that particular item first.


A linked list is a data structure that consists of a series of nodes, each of which contains data and a pointer to the next node. Linked lists are a good choice for applications where memory is limited, as each node only needs to store a pointer to the next node.

### **Advantages of Linked Lists**

-   Memory efficient: Linked lists are memory efficient because each node only needs to store a pointer to the next node, which makes them good for limited memory applications.
-   Flexible: Linked lists are flexible and easily modified,  you can both add or remove node/

### **Disadvantages of Linked Lists**

-   Slow access of elements by index because you have to traverse the entire list to find the element you are looking for.
-   Not random access: Linked lists are not random access data structures. This means that you cannot access any element in the list directly. You can only access the elements in the list sequentially.


