# Class 5

## Reading Objectives

<details markdown="block"><summary>Prompt Questions/answers</summary>


### 1. What is a real world use case for the `alt` attribute being used in a website?

It is used to provide alternative text for an image for users who are unable to view it. It's an accessiblity thing, seo thing, slow internet thing, and broken image thing.

### 2. How can you improve accessibility of images in an HTML document?

Use descriptive alternative text, provide context, accurate file names, avoid using images to conveyu important info, and use appropriate formats.

### 3. Provide an example of when the `figure` element would be useful in an HTML document.

They provide a semantic container for figures that clearly link them to their caption.

```html
<figure>
  <img
    src="images/dinosaur.jpg"
    alt="The head and torso of a dinosaur skeleton;
            it has a large head with long sharp teeth"
    width="400"
    height="341" />

  <figcaption>
    A T-Rex on display in the Manchester University Museum.
  </figcaption>
</figure>
```

### 4. Describe the difference between a `gif `image and an `svg` image, pretend you are explaining to an elder in your community.

A gif is a image type that shows simple animations or a series of images looping together to look lik motion. An svg image is a type of image that uses vector graphics, or math to create images rather than pixels.

### 5. What image type would you use to display a screenshot on your website and why?

I think my iphone usually uses png's jpegs are also common. PNG is a lossless format, so compresses well without losing quality.

### 6. Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

THe color inside the html boxes are the foreground colors, and the color of the boxes themselves are the background colors. 

### 7. Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

I would color his background a black color, his headers hot pink text, and probably add some photos.

### 8. What should you consider when choosing fonts for an HTML document?

Readability, accessability, whether it's widely available, performance, and whether you like the font or not.

### 9. What do `font-size`, `font-weight`, and `font-style` do to HTML text elements?

`font-size` sets the size of the text
`font-weight` sets the boldness-thickness of the text
`font-style` sets the style of the text

### 10.Describe two ways you could add spacing around the characters displayed in an `h1` element.

`letter-spacing`, where you change the spacing between individual characters, `word-spacing` where you change the spacing between words.

</details>