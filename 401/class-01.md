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
