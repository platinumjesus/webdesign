# Chapter 2: Layout

## New tools

Install [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/).

Open the Atom settings, go to "packages" and install these packages:
* HTML Lint
* Color Picker
* Hover Color

## Gotchas
Some tips to avoid common problems we encoutered last time:
* Choose short filenames consisting only of lowercase characters
* Make sure that every tag you open has a corresponding closing tag
* If something doesn't work, look for missing characters, spaces and other typos in your tag names and attributes

## Browser Developer Tools
Right-click on any page and select "Inspect element" to open your browser's developer tools. Alternatively, you can use the keyboard combination `ctrl + shift + i`.

## Starting Point
Paste this code into a file called index.html to get started.
```
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>This is the title!</h1>
  <h2>A subtitle.</h2>
  <p>And this is a paragraph with some text in it.</p>
  <p>Check out this image:</p>
  <img src="img/image.png">
</body>
</html>
```

## New HTML Tags
* Link `<a href="http://url.com"> visible text </a>`
* Divider (Container for other things)
* Emphasis (italic) `<em> Italic Text </em>`
* Strong (boldface) `<strong> Bold Text </strong>`
```
<div>
...
</div>
```

## New CSS

### Classes and Ids
Classes and ids are identifiers which can be manually added to HTML in order to make it easier to style. Classes are generally used when many elements share the same styles, while ids should only be used for one element.

```
<div class="class1 class2 class3">
  ...
</div>

<div id="id">
  ...
</div>
```

```
.class {
  property: value;
}

#id {
  property: value;
}
```

**Note:** It's good practice not to use ids to style elements because they have a higher precedence than other selectors, which means overriding them can get messy.

### Pseudo-classes
Pseudo-classes specify a state of an element.

```
selector:pseudo-class {
  property: value;
}
```
examples:
```
a:hover {
  color: green;
}

.widget:last-of-type {
  margin-right: 0;
}

.container:nth-child {
  margin-right: 0;
}
```

### Advanced Selectors

Style everything on the page: `* {...}`

Style all the children of elements with class "header": `.header > * {...}`

Style all the children of elements with class "header" that are a tags: `.header > a {...}`

Style all the descendants (children, children of children and so on) of elements with class "header" that are a tags: `.header a {...}`

Style a tags, div tags and elements with the class "header": `a, div, .header {...}`

## CSS Layout

### Centering Elements

How to center different types of elements in different contexts:

**Text elements** (e.g. paragraphs, titles)
```
text-align: center;
```

**Block elements** (e.g. containers)
```
margin-left: auto;
margin-right: auto;
```

### Display
Defines the type of a box element.

value | explanation
---------|---------
`display: none` | Element disappears from page
`display: inline` | Element flows (like a word in a paragraph); Width, height and vertical margins cannot be set **(default)**
`display: block` | Element does not flow (displayed in a new line); Width, height and margins can be set freely
`display: inline-block` | Element flows; Width, height and margins can be set freely
`display: flex` | Magic rainbow unicorns! (more about it later)

### Position

value | explanation
---------|---------
`position: static` |
`position: absolute` |
`position: relative` |
`position: fixed` |
`position: sticky` |

### Float


## Page structure
