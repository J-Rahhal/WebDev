# More HTML elements

## main

The `<main>` element is used to represent the main content of the body of an HTML document

```html
<body>
  <main>
    <h1>My first Webpage</h1>
    <p>my first paragraph</p>
  </main>
</body>
```

If we look at the code above we can see elements inside each other, such as the `main` is inside the `body`, the `h1` is inside the `main` etc.. this is called **nesting**

## image Tag

> Please go back to `../README.md` in the main folder.

## Anchor tag (link on webpage)

You can link to another page with the anchor tag `<a>`

```html
<a href="www.instagram.com">Instagram</a>
```

## target tag

To open links in a new tab you should use the `target` attribute and assign it the value of `_blank`

```html
<a href="instagram.com" target="_blank">Instagram</a>
```

## Section tag

The section element is used to define a new section in your html document.

```html
<main>
  <section>
    <h2>Title</h2>
    <p>Paragraph Content</p>
  </section>

  <section>
    <h2>Title</h2>
    <p>Paragraph Content</p>
  </section>
</main>
```

## unordered list

To create an unordered list of items you should use the `<ul></ul>` element

### add list items

list items `<li></li>` are used to add items to the list

```html
<ul>
  <li>item 1</li>
  <li>item 2</li>
  <li>item 3</li>
</ul>
```

## ordered lists

To create an ordered list of items you should use the `<ol></ol>` element

### add list items

list items `<li></li>` are used to add items to the list

```html
<ol>
  <li>item 1</li>
  <li>item 2</li>
  <li>item 3</li>
</ol>
```

## figure & figcaption elements

The `<figure></figure>` allows you to give a caption to the image associated with it. the image should be nested inside the figure element.

The `<figcaption><figcaption>` element is used to add a caption to describe the image contained within the figure element.

```html
<figure>
  <img src="image.jpg" alt="image description" />
  <figcaption>A pizza slice</figcaption>
</figure>
```

## Em element

The em element is used to emphasize specific words inside an element

```html
<p>Hello this is my <em>First</em> Paragraph</p>
```

## Strong element

The strong element is used to indicate the importance and the urgency of a word in an element

```html
<p>I <strong>Love</strong>food</p>
```

## footer element

The footer element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more.

```html
<main>
  <section>
    <h2>Title</h2>
    <p>Paragraph Content</p>
  </section>

  <section>
    <h2>Title</h2>
    <p>Paragraph Content</p>
  </section>
</main>
<footer>
  <p>Copyrights</p>
</footer>
```

## Divs

The `<div>` element is used as a container to group other elements

```html
<div>
  <p>Example paragraph element.</p>
</div>
```

You will mainly use the div element when you want to group HTML elements that will share a set of CSS styles

> you should know when to use div and when to use the more appropriate element.

```html
<section>
  <h2>Reptiles</h2>
  <p>
    Reptiles are cold-blooded animals with scaly skin. Most lay eggs on land.
  </p>
  <ul>
    <li>Snake</li>
    <li>Crocodile</li>
    <li>Turtle</li>
  </ul>
</section>
```

The `<section>` element has **meaning**, while `<div>` doesn't — that's the key difference.

"Semantic" just means "meaningful." A `<div>` is a plain box with no built-in meaning — it just says "here's a container." But `<section>` tells the browser (and anyone reading your code) _what this part of the page actually is_.

So when you use `<section>`, browsers, screen readers, and other tools understand: "this is a distinct section of content" — whether it's viewed on a desktop, phone, or anything else. A `<div>` can't communicate that.

# Homework

## Your tasks

- got to index.html in the elements folder
- create a boilerplate
- create a webpage about your favorite movies
- your page should have a minimum of 5 movies
- you should use all the elements you've seen until now.
- use git to submit your homework.

> no css or styling is needed.
