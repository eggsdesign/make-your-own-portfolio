# Course summary

## Visual Studio Code editor

## HTML

### The anatomy of an html element

```html
<div>
  <!-- Content -->
</div>
```

```html
<div attribute="value" another-attribute="value">
  <!-- Content -->
</div>
```

Some html elements you will probably bump into

- `<div>` is a diverse element mostly used for grouping other elements. However, if you want to use more meaningful elements, feel free to check out the `<main>`, `<article>`. `<section>`, `<header>`, `<footer>` elements instead.
- `<img>` an image tag. It supports the attribute `src="my-cool-image.png"` which can point to an image in your project or on the internet.
- `<h1>` `<h2>` `<h3>` `<h4>` heading elements used for titles.
- `<p>` a paragraph, used for blocks of text.
- `<ul>` or `<ol>` respectively unordered- and ordered list containers, often paired with...
- `<li>` ...the list element

### The basic structure of an html file

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Meta information, like page title and link to css files -->
  </head>

  <body>
    <!-- Content on the page that people will actually see --->
  </body>
</html>
```

### Example of an html page with some elements in it

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My blog</title>
  </head>

  <body>
    <h1>Welcome to my blog</h1>

    <h2>Short about me</h2>
    <p>I like long walks on the beach</p>

    <img src="image-of-me.jpg" />

    <h2>Some of my favorite hobbies</h2>
    <ul>
      <li>Design</li>
      <li>Code</li>
      <li>Cooking</li>
    </ul>
  </body>
</html>
```

## CSS

### Selectors - which elements to style

All <div> elements

```css
div {
  /* styles go here */
}
```

Only the elements with the `blogpost` class

```css
.blogpost {
  /* styles go here */
}
```

### Styles

Styles can look like this

```css
.my-box {
  border: 1px solid black;
  border-radius: 16px;
  background-color: orange; /* can also be hex value #dd33aa */
  padding: 30px; /* Spacing inside of the element */
	margin: 20px; /* Spacing outside of the element /*
}
```

## Publish to GitHub Pages

For setting up, see the [dedicated article to Setup](setup.md)

Every time you want to upload your local changes to the internet-accessible website hosted on your username.github.io domain, do the following:

- Add your changes to a commit
- Commit your changes, and add a comment to describe what you did
- Push the changes
