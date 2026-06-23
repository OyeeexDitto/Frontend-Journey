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
* No space at the container edges.

#### `space-around`

* Equal space around items.
* Edge spaces are smaller than spaces between items.

#### `space-evenly`

* Equal spacing everywhere, including the edges.

---

## Flex Wrap

### Purpose

Controls whether flex items stay on a single line or wrap onto multiple lines.

### Values

#### `nowrap`

* Default value.
* All items remain on a single line.

#### `wrap`

* Items move onto the next line when necessary.

#### `wrap-reverse`

* Items wrap in reverse order.

### Example

```css
.container {
    display: flex;
    flex-wrap: wrap;
}
```

---

## Align Items

### Purpose

Aligns flex items along the **cross axis** (perpendicular to the main axis).

### Values

#### `stretch`

* Default value.
* Items stretch to fill the container.

#### `flex-start`

* Items align to the start of the cross axis.

#### `flex-end`

* Items align to the end of the cross axis.

#### `center`

* Items are centered along the cross axis.

---

## Align Content

### Purpose

Controls the spacing between flex lines when there are multiple rows or columns of wrapped items.

### Note

* Only works when `flex-wrap: wrap` is enabled.
* Similar to `justify-content`, but affects entire flex lines rather than individual items.

---

## Align Self

### Purpose

Allows an individual flex item to override the container's `align-items` property.

### Example

```css
.item {
    align-self: center;
}
```

---

## Flex Grow

### Purpose

Determines how much a flex item will grow relative to other items when extra space is available.

### Example

```css
.item {
    flex-grow: 1;
}
```

### Notes

* Default value is `0`.
* Higher values grow more.

---

## Flex Shrink

### Purpose

Determines how much a flex item will shrink relative to other items when there is insufficient space.

### Example

```css
.item {
    flex-shrink: 1;
}
```

### Notes

* Default value is `1`.
* Higher values shrink more.

---

## Order Property

### Purpose

Changes the visual order of flex items without changing the HTML structure.

### Example

```css
.item {
    order: 2;
}
```

### Notes

* Default value is `0`.
* Lower values appear first.
* Higher values appear later.

---

## Key Flexbox Rule

```text
display: flex;
        ↓
Parent becomes Flex Container
        ↓
Direct children become Flex Items
```

---

# CSS GRID

## Definition

CSS Grid is a two-dimensional layout system that allows developers to create layouts using rows and columns.

### Features

* Supports both rows and columns simultaneously.
* Activated using `display: grid`.
* Direct children become grid items.
* Layout structure is defined using grid properties.
* Individual units are called **grid cells**.

### Example

```css
.container {
    display: grid;
}
```

### Common Grid Properties

```css
grid-template-columns
grid-template-rows
gap
grid-column
grid-row
```
