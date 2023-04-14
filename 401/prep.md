This is a md file help me clean it up many of these are headers for future work.

<details markdown="block"><summary>Key Takeaways
</summary>
- Java is an Object-Oriented Programming (OOP) language.


</details>

<details markdown="block"><summary>Command Line</summary>

### Miscellaneous

<details markdown="block"><summary>Useful Commands</summary>

<details markdown="block"><summary>Useful Commands</summary>
Find the size of every directory inside your current directory:

Use the command du -sh ./* to calculate and display the size of every directory in your current location. The -s option summarizes the total size, while the -h option displays the sizes in a human-readable format.

Display how much disk space is used and available:

Use the command df -h to show disk space usage and availability in a human-readable format. The -h option makes the output easier to understand by displaying the sizes in a more readable format (e.g., KB, MB, GB).

Obtain a listing of processes and their IDs:

Use the command ps to display a list of processes and their respective IDs. Including the option aux with the command ps aux will show all processes with additional details, such as user, CPU usage, memory usage, and the command used to start the process.

Monitor system activity in real-time:

Use the command top to display a real-time, dynamic view of the processes running on your system. This command provides information about the system's performance, including CPU usage, memory usage, and more.

</details>

</details>

<details markdown="block"><summary>Manipulating Files and Directories</summary>

#### Create directories with necessary parent directories:

Use the command mkdir `-p` followed by the desired directory path to create the target directory and any necessary parent directories that don't exist. For example: mkdir `-p exist/nonexistentsteppingstone/targetfile`. The `-p` option ensures that all parent directories are created as needed.

#### Verbose output while creating directories:

Use the `-v` flag with mkdir to display messages about what the command is doing. For example: mkdir -v new_directory. The `-v` option provides verbose output, making it easier to understand what the command is doing.

#### Check available space on the hard drive:

Use the command `df -h` to see the available and used space on the hard drive in a human-readable format. The `-h` option displays sizes in a more understandable format (e.g., KB, MB, GB).

#### Wildcard characters in commands:

```bash
* represents zero or more characters, often used for searching or matching multiple files or directories.
? represents a single character, used for more precise searching or matching files or directories.
[] represents a range of characters. For example, [a-z] represents all lowercase letters, and [0-9] represents all digits. Useful for matching patterns in file or directory names.
```

</details>

</details>

## Java Fundamentals Overview - Learn the Basics

1. Hello, World!

2. Variables and Types

3. Conditionals

4. Arrays

5. Loops

6. Functions

7. Objects

## Create an artifact configuration for the JAR



From the main menu, select File | Project Structure (⌘ ;) and click Artifacts.
Click the Add button, point to JAR, and select From modules with dependencies.
To the right of the Main Class field, click the Browse button and select HelloWorld (com.example.helloworld) in the dialog that opens.
Apply the changes and close the dialog.


## Java Tutorial

<details markdown="block"><summary>Your First Java App</summary>
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

## Java Introduction

<details markdown="block"><summary>Java Intro</summary>

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

