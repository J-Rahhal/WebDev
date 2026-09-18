# IDs & Classes

## ID attribute

the `id` attribute adds a unique identifier to an HTML element

```html
<h1 id="title">Page</h1>
```

You can reference the id name of title within your JavaScript or CSS.

```CSS
#title {
  color: red;
}

```

The id referenced in the CSS file by writing `#title`
this tells the computer that we want to target an `id` with that value.

- id names are unique and cannot have spaces between them

## Class attribute

the class attribute does not need to be unique and can contain spaces

```html
<div class="box black-box"></div>
```

this is also an example of having multiple classes for the element `div`.

classes are used when you want to apply the same styles to many elements. if you want to target a specific element it is better to use id.

## Script

The script element is used to embed executable code. Most developers will use this to execute JavaScript code. JavaScript is used to add interactivity to your web pages.

```html
<body>
  <script>
    // alert("This is a Javascript code");
  </script>
</body>
```

While you can technically write all of your JavaScript code inside the script tags, it is considered best practice to link to an external JavaScript file instead.

```html
<script src="path-to-javascript-file.js"></script>
```

The src (source) attribute is used here to specify the location for that external JavaScript file

> Please Check General folder
