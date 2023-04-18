# Class 2

# Readings

## Reading

[Java Imports](https://www.programiz.com/java-programming/packages-import)

1.  Use an analogy to explain Built-In packages. Give examples.
2. Package are like tools of related items like a tackle box. You import it when you're fishing, but not when going to eat fish.
3.  Explain the steps for creating a new package in IntelliJ.
4. 
5. 

[Different types of loops in Java](https://www.baeldung.com/java-loops)

1.  Which loop types use a loop counter?
> The For loop
3.  Explain the difference between While and Do-While loops.
> The while loop ==checks the condition prior== to executing the block of code. If it's true the loop is executed, and it continues executing until it becomes false. ==If false it doesn't execute at all==. Used when the number of times the loop should execute is unknown or if the loop shouldn't be executed at all if the condition is false from go.
> Do-while executes the code block first and then checks the condition. It guarantees the block of code will be executed at least once. Even if the condition is initially false. Use when the code needs to be executed at least once, or you want to check the condition aafter the block of code has been executed.
```java
do {

} while (condition)
```


[Java Arrays](https://www.tutorialspoint.com/java/java_arrays.htm)

1.  Describe 3 built-in methods for Arrays.
Arrays.sort(): Sorts the elements of an array in ascending order.
Arrays.CopyOf(): Creates a new arraywith a specified length, filling default values for extra elements.

3.  How is the size of an array determined in Java
>At creation and it doesn't change. 


## Notes
A Package is a container that groups related types(Java classes, interfaces, enumerations and annotations.
)

### Built in packages
Come with the JDK examples are java.lang, java.util, java.io
### User-defined package
Requires keyword `package` so `package packageName`
==Like Domain names, packages must be unique, so it's commonly com.company.name.==
It can be via import statement or by using fully qualifieed name.
```java
import java.util.Date;

class MyClass implements Date {
    // body
}

//or 
class MyClass implements java.util.Date {
    //body
}
```

