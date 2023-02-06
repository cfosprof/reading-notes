# Class 2

These topics matter because they're the basis of web development, and are key to understanding front end development.

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>

## HTML

### 1.Why is it important to use semantic elements in our HTML?

It gives meaning to the content and structure of a webpage, makes the page more accessible to other users and search engines by clearly defining the purpose of elements in the content.

### 2. How many levels of headings are there in HTML?

There are 6 levels.

### 3.What are some uses for the `<sup>` and `<sub>` elements?

The `<sup>` element is common in exponents and foot notes, the `<sub>` element is common in chemical formulas like H<sub>2</sub>0 and footnote references.

### 4. When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?

When using the abbreviation element you should include the title for the expanded form of the abbreviated term. it looks like `<abbr title="World Wide Web">WWW</abbr>` ends up looking like <abbr title="World Wide Web">WWW</abbr>


## CSS

### 1. What are ways we can apply CSS to our HTML?

* External stylesheet:
    * A separate file with a .css extension that is referenced via the HTML `<link>` element.
    ```html
    <head>
        <link rel="stylesheet" href="style.css" />
    <head>
    <body>
            <h1>Title</h1>
    <body>

    and then the css sheet
    h1 {
        color: blue;
    }
    ```

### 2. Why should we avoid using inline styles?

They're nonreusable, difficult to maintain, and make it harder to understand the code.

### 3. Review the block of code below and answer the following questions:

```
h2 {
color: black;
padding: 5px;
}
```

#### * What is representing the selector?

The h2 is the selector here

#### * Which components are the CSS declarations?

color: black; padding: 5px;

#### * Which components are considered properties?

The color and padding

## JS

### 1. What data type is a sequence of text enclosed in single quote marks?

A string

### 2. List 4 types of JavaScript operators.

Arithmatic`+`, Assignment`=`, comparision`==`, and conditional operators like if.

### 3. Describe a real world Problem you could solve with a Function.

You can write a function that automatically takes an NFL players yardage from week 1-18 and adds them all together to total out his season yardage.

### 4. An if statement checks a __ and if it evaluates to ___, then the code block will execute.

Conditional True

### 5. What is the use of an else if?

It is used to provide multiple conditions for the conditional to test true and execute

### 6. List 3 different types of comparison operators.

`==`, `!=`, `<=`

### 7. What is the difference between the logical operator && and ||?

`&&` returns true when the conditions on each side is true, and false otherwise

`||` returns true if the condition on either side is true, and false if neither is true.

</details>