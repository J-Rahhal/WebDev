# What is HTML

HTML stands for HyperText Markup Language. It is the structure and content of a webpage.

## What is HTML mad up of?

HTML is made up of elements.

```html
<h1>Intro to HTML</h1>
```

Elements start with an opening tag `<h1>` and end with a closing tag `</h1>`.

## h1

An `<h1>` element is the main heading of a webpage and should on be used once per page.

## h2

`<h2>` is a subheading. you can have multiple subheadings per page.

## Headings

There are six heading elements in HTML `<h1>` through `<h6>`. They're used to show importance of sections on the webpage, with `<h1>` being the most important and `<h6>` being the least important.

## paragraph

`<p>` is used to add a paragraph on the webpage. It can be used any number of times.

## Void elements

An element that does not have a closing tag is called **void element**

```html
<img />
```

## HTML Attributes

we have mentioned the `<img/>` element earlier, this tag is used to display images on the webpage. until now this tag does not display anything. In order for it to display an image An **Attribute** inside the tag must be used.

> An attribute is a special value used to modify the behavior of the element.

### Src attribute

The `src` attribute should be used inside the tag in order to display an image by assigning a link or a path as a value to it.

```html
<img src="add link here" />
```

### atl Attribute

The `alt` attribute is used to provide a description of the image. This attribute is used for accessibility purposed.

## HMTL & CSS & JavaScript

- HTML is the structure and content of the webpage
- CSS is for styling
- JavaScript is for adding interactivity.

## Link Element

The link element is used to link external stylesheets and site icons to the HTML.

```html
<link rel="stylesheet" href="path to the css file" />
```

- `rel` attribute is used to specify the relationship between linked resources and the HTML document

- `href` is used to specify the location for the external resource.

> `./file_name` the `.` means to look in the current directory for the `file_name`
> The `link` element should be added in the `head` of the HTML file as seen here

```html
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Examples of the link element</title>
  <link rel="stylesheet" href="./styles.css" />
</head>
```

## HTML Boilerplate

An HTML boilerplate is a ready-made template for your webpages.

> please check ./boilerplate/boilerplate.html
