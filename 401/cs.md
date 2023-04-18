# Java Cheatsheet

## Idk
### for loops
#### Basic
```java
for (init; condition; update) {
//code
}
```
#### Enhanced or for each loop
Used to iterate over arrays or collections without needing to manage a loop counter. Reads as for each element in the array, do teh following
```java
int[] numbers = {1, 2, 3, 4, 5};

for (int number : numbers) {
    System.out.println("Number: " + number);
}

```
#### Nested for loop
Iterating over multi dimensional arrays or multiple levels of looping
```java
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 2; j++) {
        System.out.printf("i = %d, j = %d%n", i, j);
    }
}

```

