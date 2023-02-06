# Class 1

## Things I want to know more about

<details markdown="block"><summary>Things</summary>

okay

</details>

## Terms and Concepts

<details markdown="block"><summary>Terms</summary>

<dl>
    <dt>Nesting</dt>
    <dd>Elements placed in other elements. Common term we've come acrossed, so should make it a part of our language.</dd>
    <dt>Block and inline elements</dt>
    <dd>Block level elements are generally structural and represent sections like menus and paragraphs. Inline elements are contained within block level, and are used to emphasize smaller parts like text highlighting.</dd>
    <dt>Void Elements</dt>
    <dd>`Used to insert imbed something in a document. The image tag is an example.</dd>
    <dt>Attributes</dt>
    <dd>Contain extra information not contained in the content. <code><\details class ="toggle"></code></dd>
</dl>

</details>

<details markdown="block"><summary>Remember</summary>

### How to assign html class for styling

```
<details class="toggle" markdown="block">
```

</details>

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>


### 1. Describe how HTML, CSS, and JS files are “parsed” in the browser.

The browser first parses the HTML file which leads to the identification to any `<link>` or `<script>` elements that reference to any external CSS or JS documents.

As it parses the HTML it requests any css or JS files found in thier perspective elements from the server and then parses the css and js from their files.

The browser then generates the DOM tree from the html, an in-memory CSSOM structure from the CSS, and compiles and executes the parsed js.

As the browser builds the DOM tree, styles the CSS, and executes the JS a visual representation is created on the screen that that we can see and interact with.

### 3. How can you find images to add to a Website?
You can use google images, there is a copyright filter that will filter out any images that are copyrighted. You can also use your camera roll, or a billion other sources.

### 4. How do you create a String vs a Number in JavaScript?

`let string = "string"`

`let num = 45`

### 5. What is a Variable and why are they important in JavaScript?

A variable is a container used to store values in. They reduce the need to reenter a specific value every time it is needed.

### 1. What is an HTML attribute?

An attribute specifies an additional value or information that will not appear in the actual content itself.

### 2. Describe the Anatomy of an HTMl element.

1. An element name wrapped in opening and closing angle brackets. This is the beginning of the elements impact. 
2. The content of the element, which can be text or a number of other things. 
3. Followed by the closing tag WHich is the same opening angle bracket followed by a forward slash then the element name, and then a closing angle bracket.

### 3. What is the Difference between `<article>` and `<section>` element tags?

`<section>` Elements should only be used with generic standalone sections of a document when there isn't a more specific element to represent it. `article` elements are used as containers compoosing the composition for things like blog articles that have formatting that will be reused or syndicated for similar content in the future.

### 4. What Elements does a “typical” website include?

`<head>, <header>, <nav>, <main>, <article>, <section>, <div>, <aside>, <footer>, <p>`


### 5. How does metadata influence Search Engine Optimization?

Including a description with keywords relating to the content of your page because it has the potential to help it appear higher in relelvant searches performed in search engines--although keywords are often ignored in search engines now because of spammers filling lists with irrelevant keywords.

### 6. How is the `<meta>` HTML tag used when specifying metadata?

It is used in the `head` of a document, where we can assign values to attributes like name and content.

### 1. What is the first step to designing a Website?

Determine what it is that you want to accomplish, how your website can help you reach those goals, and what needs to be done and in what order to reach those goals. It's referred to as project ideation.

### 2. What is the most important question to answer when designing a Website?

What exactly do I wish to accomplish with this website?

### 1. Why should you use an `<h1>` element over a `<span>` element to display a top level heading?

Because most browsers have user agent styleshets that will style an `<h1>` with a large font meant to look like a heading, whereas `<span>`s will not receive the same benefits.

### 2. What are the benefits of using semantic tags in our HTML?

* Search engines will consider its contents as importent keywords that influence the page's search rankings.

* Screenreaders can use it as a signpost to help visually impaired users navigate a page.

* Finding blocks of meaningful code is much easier than searching through a bunch of `div`s.

* Gives the developer an idea of what type of data will be populated.

* Semantic naming mirrors proper custom element and component naming.

### 1. Describe 2 things that require JavaScript in the Browser?

Recording any click actions and updating the page with them, or storing user variables to use later both require JS

### 2. How can you add JavaScript to an HTML document?

By either using an internal `<script> somecode </script>` element with some JS in it or by creating an external js file with the javascript code and calling it with `<script src="jsFileNanme.js" defer></script>`

</details>
