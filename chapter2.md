# Chapter 2: Layout

## Browser Developer Tools

## Advanced CSS

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
