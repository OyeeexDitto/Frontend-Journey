# FLEXBOX - GRID - MEDIA QUERIES

---

## Float Property

### Purpose

Used to align elements to the left or right within their parent container.

### Values

* `left` → Floats the element to the left.
* `right` → Floats the element to the right.
* `none` → Default value; element does not float.

### Notes

* Commonly used in older website layouts.
* Less frequently used today because Flexbox and Grid provide better layout control.

---

# FLEXBOX

## Flex Direction

### Purpose

The `flex-direction` property defines the direction in which flex items are placed inside a flex container.

### Values

#### `row`

* Default value.
* Arranges items horizontally from left to right.

#### `column`

* Arranges items vertically from top to bottom.

#### `row-reverse`

* Arranges items horizontally from right to left.

#### `column-reverse`

* Arranges items vertically from bottom to top.

### Example

```css
.container {
    display: flex;
    flex-direction: row;
}
```

---

## Justify Content

### Purpose

The `justify-content` property aligns flex items along the **main axis**.

### Values

#### `flex-start`

* Items are aligned at the start of the container.

#### `flex-end`

* Items are aligned at the end of the container.

#### `center`

* Items are centered inside the container.

#### `space-between`

* Equal space between items.
* No space at the edges.

#### `space-around`

* Equal space around items.
* Edge spaces are smaller than the spaces between items.

#### `space-evenly`

* Equal spacing everywhere, including edges.

### Example

```css
.container {
    display: flex;
    justify-content: space-between;
}
```

---

## Key Flexbox Rule

```text
display: flex;
        ↓
Parent becomes Flex Container
        ↓
Direct children become Flex Items
```

### Example

```html
<div class="container">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
</div>
```

```css
.container {
    display: flex;
}
```

Result:

```text
[Item 1] [Item 2] [Item 3]
```
