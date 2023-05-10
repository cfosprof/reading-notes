# Key Takeaways

- Java is an Object-Oriented Programming (OOP) language.

# Prep: Practice in the Terminal

<details markdown="block"><summary>Content</summary>

## Useful Commands

### Find the Size of Every Directory inside Your Current Directory

- Use the command `du -sh ./*` to calculate and display the size of every directory in your current location. The `-s` option summarizes the total size, while the `-h`option displays the sizes in a human-readable format.

### Display how much Disk Space is Used and Available

- Use the command `df -h` to show disk space usage and availability in a human-readable format. The `-h` option makes the output easier to understand by displaying the sizes in a more readable format (e.g., KB, MB, GB).

### Obtain a Listing of Processes and Their IDs

- Use the command ps to display a list of processes and their respective IDs. Including the option aux with the command ps aux will show all processes with additional details, such as user, CPU usage, memory usage, and the command used to start the process.

### Monitor System Activity in Real-time

- Use the command top to display a real-time, dynamic view of the processes running on your system. This command provides information about the system's performance, including CPU usage, memory usage, and more.

## Manipulating Files and Directories

### Create Directories with Necessary Parent Directories

- Use the command mkdir ``-p`` followed by the desired directory path to create the target directory and any necessary parent directories that don't exist. For example: `mkdir -p exist/nonexistentsteppingstone/targetfile`. The `-p` option ensures that all parent directories are created as needed.

### Verbose Output while Creating Directories

- Use the `-v` flag with mkdir to display messages about what the command is doing. For example: mkdir -v new_directory. The `-v` option provides verbose output, making it easier to understand what the command is doing.

### Check Available Space on the Hard Drive

- Use the command `df -h` to see the available and used space on the hard drive in a human-readable format. The `-h` option displays sizes in a more understandable format (e.g., KB, MB, GB).

### Wildcard Characters in Commands

```bash
`*` represents zero or more characters, often used for searching or matching multiple files or directories.
`?` represents a single character, used for more precise searching or matching files or directories.
`[]` represents a range of characters. For example, [a-z] represents all lowercase letters, and [0-9] represents all digits. Useful for matching patterns in file or directory names.
```

</details>

# Android builder

<details markdown="block"><summary>Photo</summary>

![](../assets/Pasted%20image%2020230416195726.png)

</details>

# Java Fundamentals Overview - Learn the Basics

I think I inserted these in reverse order.

<details markdown="block"><summary>Info</summary>

</details>

# IntelliJ Overview

<details markdown="block"><summary>Content</summary>

## Assignment Overview

## Your First Java App

[IntelliJ](https://www.jetbrains.com/help/idea/creating-and-running-your-first-java-application.html)
<https://canvas.instructure.com/courses/6504881/assignments/36513391>

## Your First Java App

![](../assets/Pasted%20image%2020230416130320.png)

![](../assets/Pasted%20image%2020230416133149.png)

## Debugging Java

Follow through all the directions in every section of this page. Topics covered:

### Before You start…Putting Breakpoints

![](../assets/Pasted%20image%2020230416141957.png)

### Starting a Debugger Session

![](../assets/Pasted%20image%2020230416142000.png)

### Stepping through the Application

![](../assets/Pasted%20image%2020230416143319.png)
![](../assets/Pasted%20image%2020230416142045.png)

## Submitting Your Work

Breakpoint
Defines what point you want to stop the program and begin walking through what happens during each of the following steps.
Step-to-next-line
The process of executing the current line and taking the exection point to the line following it in the current method
Step-inside-function-call
Executes the current line and steps into the called method if there is one.
Step-out-of-function-ca
Executes remaining lines and exits the methodstopping at the next line after the method call.

</details>

# Java Introduction

<details markdown="block"><summary>Content</summary>

`public` - can be accessed from anywhere
`static` - can be accessed without creating an instance of the class
`void` - does not return anything
`main` - the entry point of the program
`System` - a pre-defined class in java that holds useful methods and variables
`System.out` - a static variable within system that represents the standard output of the program
`println` - a method that can be used to print a line

## Additional System Methods and Variables

`System.in`: This is an instance of InputStream and is used to read input from the console. Generally used with Scanner or BufferedReader to read user input.

`System.err`: This is an instance of PrintStream and is used to display error messages on the console, similar to System.out. The primary difference is that it writes to the standard error stream, allowing you to separate regular output from error messages.

`System.currentTimeMillis()`: This method returns the current time in milliseconds since the epoch (January 1, 1970, 00:00:00 GMT). Useful for measuring the time taken by a piece of code or for generating timestamps.

`System.nanoTime()`: Similar to System.currentTimeMillis(), but provides greater precision with nanosecond resolution. It is primarily used for measuring time intervals, not for obtaining wall-clock time
</details>

# Java

## Hello, World

#### `public Static Void main(String[] args) {`

- `public` again means that anyone can access it.
- `static` means that you can run this method without creating an instance of Main.
- `void` means that this method doesn't return any value.
- `main` is the name of the method.

#### `System.out.println("This Will Be printed");`

- `System` is a pre-defined class that Java provides us and it holds some useful methods and variables.
- `out` is a static variable within System that represents the output of your program (stdout).
- `println` is a method of out that can be used to print a line

## Variables and Types

- Java has 8 primitive types:

  - `byte` (number, 1 byte)
  - `short` (number, 2 bytes)
  - `int` (number, 4 bytes)
  - `long` (number, 8 bytes)
  - `float` (float number, 4 bytes)
  - `double` (float number, 8 bytes)
  - `char` (a character, 2 bytes)
  - `boolean` (true or false, 1 byte)

- It is strongly typed, which means variables need to be declared with their appropriate type before they can be used.

#### Declaring a Variable

```java
int myNumber = 5;

//double floating point number
double d = 4.5;

//float
float f = 4.5f;

//Or
float f = (float) 4.5;

```

## Characters and Strings

- A character is it's own type, char, and it's represented by single quotes.

```java
char a = 'a';
```

- Strings are not primitive types, they are objects. They are immutable, which means that once they are created, they cannot be changed.

- Strings are the only objects that can be created without the `new` keyword.

- Strings are also the only objects that can be concatenated with the `+` operator, which is called operator overloading.

### Examples

```java
// strings are created both as literals and as objects

String str1 = "Hello, World!";
String str2 = new String("Hello, World!");

// strings can be concatenated with the + operator

String str3 = str1 + " " + str2;

// strings can be compared with the equals method

boolean equal = str1.equals(str2); // false

// String Lenght
String str = "Hello, World!";
int len = str.length(); // 13

// Accessing Characters by Index
String str = "Hello, World!";
char first = str.charAt(0); // 'H'

// String Case altering
String str = "Hello, World!";
String upper = str.toUpperCase(); // "HELLO, WORLD!"
String lower = str.toLowerCase(); // "hello, world!"

// Substrings
String str = "Hello, World!";
String substr = str.substring(0, 5); // "Hello"
String substr2 = str.substring(7); // "World!" (starts at index 7 until the end of the string)

// String Trimming
String str = "   Hello, World!   ";
String trim = str.trim(); // "Hello, World!"

// String Replacement
String str = "Hello, World!";
String replace = str.replace('H', 'J'); // "Jello, World!"
String replace2 = str.replace("Hello", "Goodbye"); // "Goodbye, World!"

// String Splitting
String str = "Hello, World!";
String[] array = str.split(", "); // {"Hello", "World!"}

//Joining strings:
String[] words = {"Hello", "World"};
String joinedStr = String.join(", ", words); // "Hello, World"


//Converting string to character array:
String str = "Hello, World!";
char[] chars = str.toCharArray(); // ['H', 'e', 'l', 'l', 'o', ',', ' ', 'W', 'o', 'r', 'l', 'd', '!']


//Converting other data types to strings:
int number = 42;
String str = Integer.toString(number); // "42"


//Converting strings to other data types:
String str = "42";
int number = Integer.parseInt(str);

//String formatting:
String formattedStr = String.format("Hello, %s!", "World"); // "Hello, World!"

```

## Conditionals

#### JavA Conditional Operators

```java
int a = 4;
int b = 5;
boolean result;
result = a < b; // true
result = a > b; // false
result = a <= 4; // a smaller or equal to 4 - true
result = b >= 6; // b bigger or equal to 6 - false
result = a == b; // a equal to b - false
result = a != b; // a is not equal to b - true
result = a > b || a < b; // Logical or - true
result = 3 < a && a < 6; // Logical and - true
result = !result; // Logical not - false
```

#### `==` And Equals

The operator `==` works a bit different on objects than on primitives. In objects `==` will check whether the object is the same, `a.equals` will check if they are logically the same. In other words, if you want to check if two objects are the same object use `==`, if you want to check if they're logically the same use `.equals.`

## Arrays

To declare an array that will hold integers use:
 `int[] arr;`
To create a new array with the size of 10 use
 `arr = new int[10];`
Create an array with values in the same line
`int[] arr = {1, 2, 3, 4, 5};`
Accessing the array and it's values

```java
arr [0] = 4;
arr [1] = [0] + 5;
```

Printing an array:

```java
for (int i =0; i < arr.length; i++) {
 System.out.println(arr[i]);
}
```

## Loops

There are two loop types in Java, for and while

#### For

`for (int i = 0; i < 3; i++) {}`
Like js, the first section initializes our entering position, the second is the bouncer screening for true before allowing us to run and enter the loop, if false we don't run that iteration. The third is the final statement that runs everytime the loop runs.

##### I'm not Sure why We'd Do This, but Apparently We Can Omit the First and Third Section and Make Our Code Look like it Forgot Its Pants when it Left the House

`for (;i < 5;) {}

#### While

`while (condition) {}`
The condition runs the first time when entering and every time the loop is done until it returns false.
To ensure the loop always runs at least once use `do-while`;

```java
do {

} while(condition);
```

#### For Each

Another version of for, is foreach. In js foreach accepts index as an optional argument, but java does not.

```java
int [] arr = {2, 0, 1, 3};
for (int el : arr)) {
 System.out.println(el);
}

//^ equates to

int[] arr = {1, 9, 9, 5};
for (int i = 0; i < arr.length; i++) {
    int el = arr[i];
    System.out.println(el);
}
```

#### Break and Continue

Allow us to control the loop from within it. `break` will stop immediatley, turn around, and exit the for loop work floor.  

```java

int i;
for (i = 0; i < 5; i++) {
    if (i >= 2) {
        break;
    }
    System.out.println("Yuhu");
}
System.out.println(i);
```

`continue` will stop the current iteration, and will move on to the next one.

```java
int i;
for (i = 0; i < 5; i++) {
    if (i >= 3) {
        break;
    }
    System.out.println("Yuhu");
    if (i >= 1) {
        continue;
    }
    System.out.println("Tata");
}
System.out.println(i);
```

## Functions

All function definitions in java must be within classes.

```java
public class Main {
 public static void foo() {
  //dowhatever, dog
 }
}
```

We define the method `foo` in class main.
`static` means thsi method belongs to the class Min and not to a specific instance of Main. This allows us to call the method from a different class like that Main.foo().
`void` means the method doesn't return a value. Methods can return a single value in Java and it has to be defined in the method declaration,, but you can use `return` by itself to exit the method.

#### Arguments

```java
 public void bar(int num1, int num2) {
  ...
}

int a = 3;
int b = 5;
bar(a, b);
```

With an object the rules are the same, but it acts a little differently.

```java
public void bar2(student s1, Student s2){
}

Student joe = new Student ("joe");
Student jack = new Student ("jack");
bar2(joe, jack);


```

#### Non Static Methods

Non-static methods are used more frequently than static methods in java. These methods can only be run on objects and not on the whole class.

Non static methods can access and alter the field of the object

```java
public class Student {
 private String name;
 public String getName() {
  return name;
 }
 public void setName(String name) {
  this.name = name;
 }
}
```

Calling the methods will require an object of type Student.

```java
Student s = new Student();
s.setName("Danielle");
String name = s.getName();

Student.setName("Bob"); //will not work
Student.getName();
```

## Objects

Everything in Java is within classes and objects. Java objects hold a state, state are variables which are saved together in an object. We call them fields or member variables.

Define a pint with x and y values:

```java
class Point {
 int x;
 int y;
}
```

Create an instance of the Point Class

```java
Point p = new Point();
```

Since we didn't use any argments there we used a default constructor. Any class without an explicitly defined constructor have a default constructor that does nothing.
Define  a constructor:

```java
class Point {
 int x;
 int y;
 Point(int x, int y) {
  this.x = x;
  this.y = y;
 }
}
```

This means we can no longer use the default constructor new Point(), and now have to use the defined constructor(4, 1).

We can allow a constructor that allows an instance ot be created in several ways by using this.
Note it has to be the first line within the constructor.

```java
class Point {
 int x;
 int y;

 Point() {
  this(0, 0);
 }

 Point(int x, int y) {
  this.x = x;
  this.y = y;
 }
}
```

When we define Point we can access x and y

#### Methods

```java
class Point {
    void printPoint() {
        System.out.println("(" + x + "," + y + ")");
    }

    Point center(Point other) {
        // Returns the center between this point the other point
        // Notice we are using integer, we won't get an accurate value
        return new Point((x + other.x) / 2, (y + other.y) / 2);
    }
}
```

#### Public and Private Variable Methods

Using the keyword private before a variable or method  restricts the use of the variable or method to only the class itself. Public allows everyone to access it.
Constructors are generally public, variables private, and methods are split.

## Gradle

Go through this tutorial, which will ensure that you have Gradle installed on your computer and that you’re able to create a new application, build it, and run it.

</details>

# String Methods to Dive into

<details markdown="block"><summary>Content</summary>
`charAt()`, char
  Returns the character at the specified index (position)
```java

```

`codePointAt()`, int
  Returns the Unicode of the character at the specified index
```java

```

`codePointBefore()`, int
  Returns the Unicode of the character before the specified index

```java

```

`codePointCount()`, int
  Returns the number of Unicode values found in a string.

```java

```

`compareTo()`, int
  Compares two strings lexicographically

```java

```

`compareToIgnoreCase()`, int
  Compares two strings lexicographically, ignoring case differences

```java

```

`concat()`, String
  Appends a string to the end of another string

```java

```

`contains()`, boolean
  Checks whether a string contains a sequence of characters

```java

```

`contentEquals()`, boolean
  Checks whether a string contains the exact same sequence of characters
    of the specified CharSequence or StringBuffer

```java

```

`copyValueOf()`, String
  Returns a String that represents the characters of the character array

```java

```

`endsWith()`, boolean
  Checks whether a string ends with the specified character(s)

```java

```

`equals()`, boolean
  Compares two strings. Returns true if the strings are equal, and false
    if not

```java

```

`equalsIgnoreCase()`, boolean
  Compares two strings, ignoring case considerations

```java

```

`hashCode()`, int
  Returns the hash code of a string

```java

```

`indexOf()`, int
  Returns the position of the first found occurrence of specified characters in a string

```java

```

`isEmpty()`, boolean
  Checks whether a string is empty or not

```java

```

`lastIndexOf()`, int
  Returns the position of the last found occurrence of specified characters in a string

```java

```

`length()`, int
  Returns the length of a specified string

```java

```

`replace()`, String
  Searches a string for a specified value, and returns a new string where the specified values are replaced

```java

```

`startsWith()`, boolean
  Checks whether a string starts with specified characters

```java

```

`toLowerCase()`, String
  Converts a string to lower case letters

```java

```

`toUpperCase()`, String
  Converts a string to upper case letters

```java

```

</details>
