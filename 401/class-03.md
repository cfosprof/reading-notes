# Class 3

## Reading

[Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)

1.  Explain the difference between an “int” and an “Integer” in Java.
			**int** - a 32-bit signed integer
-   **long** - a 64-bit signed integer
-   **float** - a 32-bit floating-point number
-   **double** - a 64-bit floating-point number
-   **char** - a single character
-   **boolean** - a true/false value
3.  What is the default value for ints? Integers?
-   The default value for an `int` is 0.
-   The default value for an `Integer` is null.
5. 
6.  What is autoboxing? Unboxing?
**Autoboxing** is the automatic conversion of a primitive data type to its corresponding object wrapper class.
```
9. int x = 10;
10. Integer y = x;
```
**Unboxing** is the automatic conversion of an object wrapper class to its corresponding primitive data type.

[Exceptions in Java (read the first three sections on the left: What is an Exception, The Catch or Specify Requirement, Catching and Handling Exceptions)](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

1.  List the three basic categories of exceptions.
-   **Checked exceptions** are exceptions that must be handled by the programmer. If a checked exception is not handled, the compiler will generate an error.
-   **Unchecked exceptions** are exceptions that do not need to be handled by the programmer. If an unchecked exception is not handled, the program will simply terminate.
-   **Runtime exceptions** are a type of unchecked exception. Runtime exceptions are typically caused by programming errors.
4.  What type of statement can you use to handle an exception?
The `try`-`catch` statement is used to handle exceptions. The `try` block contains the code that could potentially throw an exception. The `catch` block contains the code that will be executed if an exception is thrown

### Scanner
1. Scanner objects are used to break down formatted input into tokens and translate individual tokens according to their data type.
2. By default, a scanner uses white space to separate tokens, which include blanks, tabs, and line terminators.
3. To use a different token separator, invoke the useDelimiter() method, specifying a regular expression.
4. Scanner supports tokens for all Java primitive types (except for char), as well as BigInteger and BigDecimal.
5. Numeric values can use thousands separators, which are locale-specific.
6. To specify a locale for a scanner, use the useLocale() method with the desired Locale.
7. Remember to close the scanner object when you're done with it to indicate that you're done with its underlying stream.

Example: Reading words from a text file and printing them out

```java
import java.io.*;
import java.util.Scanner;

public class ScanXan {
    public static void main(String[] args) throws IOException {
        Scanner s = null;

        try {
            s = new Scanner(new BufferedReader(new FileReader("xanadu.txt")));

            while (s.hasNext()) {
                System.out.println(s.next());
            }
        } finally {
            if (s != null) {
                s.close();
            }
        }
    }
}
```
