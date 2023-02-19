# Class 2
## Terms and Concepts

These aren't about this reading, but I'm revisiting objects for the weeks work.

Object Constructors
```javascript
function Product(name, filePath, totalExposure) {
    this.name = name;
    this.filePath = filePath;
    this.totalExposure = totalExposure;
);

let product1 = new Product(name, filePath, 0)



Defining methods

objectName.methodName = functionName;

const myObj = {
  myMethod: function (params) {
    // do something
  },

  // this works too!
  myOtherMethod(params) {
    // do something else
  },
};

<details markdown="block"><summary>Enumerating properties</summary>

### Three ways

#### for in loops

Traverses all enumerable string properties in an object

#### Object.keys(myObj)

returns an arry of keys in the object, but not those in the prototype chain

#### Object.getOwnPropertyNames(myObj)

Returns all property names regardelss of whether they're enumerable or not.



</details>



<details markdown="block"><summary>Things</summary>



</details>

<details markdown="block"><summary>Remember</summary>

### ThingToRemember



</details>

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>


Reading
Video and Audio Content

### 1. Explain how the ability to use video and audio on the web has evolved since the early 2000s.

Things have grown far more secure and moved away from things like flash, better codecs have compressed file sizes, and streaming technology is everywhere.

### 2. Describe the use of the src and controls attributes in the `<video>` element.

the src attribute contains the path to the video file you want to embed. Controls are for users to control the playback.

### 3. Why is it important to have fallback content inside the `<video>` element?

It will be displayed if th browser accessign the page doesn't support the video element.


### A Complete Guide To Grid


### 5. How does Grid layout differ from Flex?

Grid layout is two-dimensional whereas flex layout is one-dimensional.


### 6. Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.


Grid container is the element in which the display: grid is applied. it's the parent of the gridcontainer.

Grid line are the dividing lines that make up the structure of the grid they can be horizontal or vertical

Responsive Images

### 7. Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

Improved accessibility, performance, seo, and bandwidth usage are all good reasons.


### 8. Define the following `<img>` attributes srcset and sizes. Write an example of how they are used.

Srcset defines the set of images we allow the browser to choose between, and what size each of those images is. sizes defines a set of media conditions--screen widths--and indicates which size would be best to choose from when particular media conditions are true.

### 9. How is srcset more helpful for responsive images than CSS or JavaScript?

Because the browser begins preloading any images before it has any time to parse the css and JS. It makes it difficult to have responsive images ready to go.

</details>