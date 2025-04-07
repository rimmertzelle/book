# CSS - tailwind and positioning

## History of CSS

[https://www.youtube.com/watch?v=UvF0Zt4_NGU](https://www.youtube.com/watch?v=UvF0Zt4_NGU)

## Positioning HTML Elements with CSS

### Flexbox

Flexbox, or Flexible Box Layout, is a CSS3 web layout model. It's great for designing flexible responsive layout structure without using float or positioning.

To use Flexbox:

1. Set the container element to `display: flex;` This makes the direct children of the container become flex items.

```css
.container {
  display: flex;
}

```

1. Use properties like `justify-content`, `align-items`, and `flex-direction` to adjust the layout of these items.

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
}
```

### Grid

CSS Grid Layout is a 2-dimensional system, meaning it can handle both columns and rows. This makes it very powerful for building complex web layouts.

To use Grid:

1. Set the container element to `display: grid;`

```css
.container {
  display: grid;
}
```

1. Use properties like `grid-template-columns`, `grid-template-rows`, and `grid-gap` to define the structure of your grid.

```css
.container {
  display: grid;
  grid-template-columns: 1fr 2fr;
  grid-template-rows: auto;
  grid-gap: 20px;
}
```

### Assignment

---

Please implement the following design using CSS. Make sure your JavaScript is working as well.

![MacBook Pro 14_ - 1.png](CSS%20-%20tailwind%20and%20positioning%20cb2d50db95ee4bd69843d3e518ccc180/MacBook_Pro_14__-_1.png)

![iPhone 13 & 14 - 3.png](CSS%20-%20tailwind%20and%20positioning%20cb2d50db95ee4bd69843d3e518ccc180/iPhone_13__14_-_3.png)

### Further reading

---

[Basic concepts of flexbox - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)

[A Complete Guide to Flexbox | CSS-Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

[A Complete Guide to CSS Grid | CSS-Tricks](https://css-tricks.com/snippets/css/complete-guide-grid/)

[CSS grid layout - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout)