# flex-box

---

cheatsheet: https://www.sketchingwithcss.com/samplechapter/cheatsheet.html

## flex parent property

align-content determines the spacing between lines

align-items determines how the items as a whole are aligned within the container.

When there is only one line, align-content has no effect

### align-items: if it is 2 row then the items will align 50% each. align-content is for multi line flexible boxes

### align-content: take the whole row

## flex children

### order: default 0, if less than 0 the item will go to the first position and so on.

### flex-basis: we can customize the spacing between children.

#### note: if we use gap we have to use calc to reduce the space, like:
---

```css
  gap: 10px;

  flex-basis: calc(50% - 5px);
```

### flex-shrink:

The flex-shrink CSS property sets the flex shrink factor of a flex item. If the size of all flex items is larger than the flex container, items shrink to fit according to flex-shrink.

### flex:

This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. The default is 0 1 auto.

# Grid

## parent property

### grid-template-columns: repeat(3, 1fr); // set 3 flexible column with same width based on the available space

### grid-template-columns: minmax(30px, 1fr) repeat(2, 1fr); // set 3 column the first column retain at least 20px

### grid-template-rows: can be use to resize rows height and width // but you have to specify the row count

### grid-auto-rows: can be used for resizing the all row at once

### grid-template: shorthand grid-template-rows, grid-template-columns, and grid-template-areas

### justify-items: remove the auto stretching and scaling as the determined horizontal alignment

### align-items: remove the auto stretching and scaling as the determined vertical alignment

### place-items: place-items sets both the align-items and justify-items properties in a single declaration.

# responsive web design

```css
  /* Extra small devices (phones, 600px and down) */
  @media only screen and (max-width: 600px) {
    ...
  }

  /* Small devices (portrait tablets and large phones, 600px and up) */
  @media only screen and (min-width: 600px) {
    ...
  }

  /* Medium devices (landscape tablets, 768px and up) */
  @media only screen and (min-width: 768px) {
    ...
  }

  /* Large devices (laptops/desktops, 992px and up) */
  @media only screen and (min-width: 992px) {
    ...
  }

  /* Extra large devices (large laptops and desktops, 1200px and up) */
  @media only screen and (min-width: 1200px) {
    ...
  }

  /* The web page will have a lightblue background if the orientation is in landscape mode: */

  @media only screen and (orientation: landscape) {
    body {
      background-color: lightblue;
    }
  }
```
