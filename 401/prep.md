This is a md file help me clean it up many of these are headers for future work.

<details markdown="block"><summary>Key Takeaways
</summary>
- Java is an Object-Oriented Programming (OOP) language.


</details>

<details markdown="block"><summary><h2>Command Line</h2></summary>

<details markdown="block"><summary><h3>Useful Commands</h3></summary>

#### Find the size of every directory inside your current directory:

* Use the command du -sh ./* to calculate and display the size of every directory in your current location. The -s option summarizes the total size, while the -h option displays the sizes in a human-readable format.

#### Display how much disk space is used and available:

* Use the command df -h to show disk space usage and availability in a human-readable format. The -h option makes the output easier to understand by displaying the sizes in a more readable format (e.g., KB, MB, GB).

#### Obtain a listing of processes and their IDs:

* Use the command ps to display a list of processes and their respective IDs. Including the option aux with the command ps aux will show all processes with additional details, such as user, CPU usage, memory usage, and the command used to start the process.

#### Monitor system activity in real-time:

* Use the command top to display a real-time, dynamic view of the processes running on your system. This command provides information about the system's performance, including CPU usage, memory usage, and more.


</details>

<details markdown="block"><summary><h3>Manipulating Files and Directories</h3></summary>

#### Create directories with necessary parent directories:

* Use the command mkdir `-p` followed by the desired directory path to create the target directory and any necessary parent directories that don't exist. For example: mkdir `-p exist/nonexistentsteppingstone/targetfile`. The `-p` option ensures that all parent directories are created as needed.

#### Verbose output while creating directories:

* Use the `-v` flag with mkdir to display messages about what the command is doing. For example: mkdir -v new_directory. The `-v` option provides verbose output, making it easier to understand what the command is doing.

#### Check available space on the hard drive:

* Use the command `df -h` to see the available and used space on the hard drive in a human-readable format. The `-h` option displays sizes in a more understandable format (e.g., KB, MB, GB).

#### Wildcard characters in commands:

```bash
* represents zero or more characters, often used for searching or matching multiple files or directories.
? represents a single character, used for more precise searching or matching files or directories.
[] represents a range of characters. For example, [a-z] represents all lowercase letters, and [0-9] represents all digits. Useful for matching patterns in file or directory names.
```

</details>

</details>

<details markdown="block"><summary><h2>Java Fundamentals Overview - Learn the Basics</h2></summary>

## Java Fundamentals Overview - Learn the Basics

<details markdown="block"><summary>Hello, World!</summary>

`public static void main(String[] args) {`

- `public` again means that anyone can access it.
- `static` means that you can run this method without creating an instance of Main.
- `void` means that this method doesn't return any value.
- `main` is the name of the method.

`System.out.println("This will be printed");`

- `System` is a pre-defined class that Java provides us and it holds some useful methods and variables.
- `out` is a static variable within System that represents the output of your program (stdout).
- `println` is a method of out that can be used to print a line.

</details>

<details markdown="block"><summary>Variables and Types</summary>

* Java has 8 primitive types:

    * `byte` (number, 1 byte)
    * `short` (number, 2 bytes)
    * `int` (number, 4 bytes)
    * `long` (number, 8 bytes)
    * `float` (float number, 4 bytes)
    * `double` (float number, 8 bytes)
    * `char` (a character, 2 bytes)
    * `boolean` (true or false, 1 byte)

* It is strongly typed, which means variables need to be declared with their appropriate type before they can be used.

Declaring a variable:

```java
int myNumber = 5;

//double floating point number
double d = 4.5;

//float
float f = 4.5f;

//Or
float f = (float) 4.5;

```

### Characters and strings

* A character is it's own type, char, and it's represented by single quotes.

```java
char a = 'a';
```

* Strings are not primitive types, they are objects. They are immutable, which means that once they are created, they cannot be changed.

* Strings are the only objects that can be created without the `new` keyword.

* Strings are also the only objects that can be concatenated with the `+` operator, which is called operator overloading.

<details markdown="block"><summary>Examples</summary>


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

<details markdown="block"><summary>String methods to dive into</summary>

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

</details>

</details>

## Create an artifact configuration for the JAR



From the main menu, select File | Project Structure (⌘ ;) and click Artifacts.
Click the Add button, point to JAR, and select From modules with dependencies.
To the right of the Main Class field, click the Browse button and select HelloWorld (com.example.helloworld) in the dialog that opens.
Apply the changes and close the dialog.


<details markdown="block"><summary><h2>Java Tutorial</h2></summary>

<details markdown="block"><summary><h3>Your First Java App</h3></summary>
Follow the tutorial up to the part about packaging. Topics covered:

Creating a project
Exploring the project structure
Creating a package and a class
Writing code for the HelloWorld class
Using a live template for the main() method
Using code auto-completion
Using a live template for println()
Building and running the application

</details>

<details markdown="block"><summary>Debugging Java</summary>

Follow through all the directions in every section of this page. Topics covered:

Before you start…Putting breakpoints
Starting a debugger session
Stepping through the application
Stepping through the statements directly
Stepping through the method calls
</details>

<details markdown="block"><summary>Submitting Your Work</summary>

Capture screenshots of your code and its output. Consolidate them into a folder and submit it into the Canvas assignment designated for the Java Tutorial prework.

Capture screenshots of you debugging your code. Write something offering your own definitions and explanations for each of these debugging concepts:

Breakpoint
Step-to-next-line
Step-inside-function-call
Step-out-of-function-call
</details>

</details>

<details markdown="block"><summary><h2>Java Introduction</h2></summary>

`public` - can be accessed from anywhere
`static` - can be accessed without creating an instance of the class
`void` - does not return anything
`main` - the entry point of the program
`System` - a pre-defined class in java that holds useful methods and variables
`System.out` - a static variable within system that represents the standard output of the program
`println` - a method that can be used to print a line

### Additional System Methods and Variables
`System.in`: This is an instance of InputStream and is used to read input from the console. Generally used with Scanner or BufferedReader to read user input.

`System.err`: This is an instance of PrintStream and is used to display error messages on the console, similar to System.out. The primary difference is that it writes to the standard error stream, allowing you to separate regular output from error messages.

`System.currentTimeMillis()`: This method returns the current time in milliseconds since the epoch (January 1, 1970, 00:00:00 GMT). Useful for measuring the time taken by a piece of code or for generating timestamps.

`System.nanoTime()`: Similar to System.currentTimeMillis(), but provides greater precision with nanosecond resolution. It is primarily used for measuring time intervals, not for obtaining wall-clock time.

</details>

