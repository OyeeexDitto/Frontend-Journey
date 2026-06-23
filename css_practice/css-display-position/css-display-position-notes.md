# DISPLAY, POSITION & RESPONSIVE UNITS

---

# Display Property

The `display` property determines how an HTML element is displayed on a webpage.

## Block Elements

### Characteristics

* Start on a new line.
* Occupy the full available width by default.
* Width and height can be set.
* Margins and padding work normally.

### Examples

```html
<div></div>
<p></p>
<h1></h1>
<ul></ul>
<li></li>
```

---

## Inline Elements

### Characteristics

* Remain in the same line as surrounding content.
* Only occupy the width required by their content.
* Do not start on a new line.
* Width and height cannot be set easily.

### Examples

```html
<span></span>
<a></a>
<strong></strong>
<em></em>
```

---

# Responsive Web Design

A responsive website automatically adapts to different screen sizes and devices.

### Benefits

* Adapts layouts for different screen sizes.
* Uses flexible layouts and units.
* Optimizes images and assets.
* Improves user experience on desktop, tablet, and mobile devices.

---

# Relative Units

## Percentage (%)

### Purpose

Used to size elements relative to their parent element.

### Benefits

* Creates flexible layouts.
* Helps build responsive designs.
* Commonly used for width and height.

### Example

```css
width: 50%;
height: 50%;
```

---

## EM Unit

### Purpose

Relative to the font size of the parent element.

### Benefits

* Scales with parent text size.
* Useful for responsive typography.

### Example

```css
font-size: 2em;
```

If the parent font size is `20px`:

```text
2em = 40px
```

---

## REM Unit

### Purpose

Relative to the root (`html`) font size.

### Benefits

* Consistent sizing throughout a website.
* Easier to manage than `em` in large projects.

### Example

```css
font-size: 2rem;
```

If the root font size is `16px`:

```text
2rem = 32px
```

---

## Viewport Units (vw / vh)

### Purpose

Relative to the viewport size.

### Definitions

* `1vw` = 1% of viewport width.
* `1vh` = 1% of viewport height.

### Uses

* Full-screen sections.
* Responsive layouts.
* Dynamic sizing.

### Example

```css
height: 100vh;
width: 100vw;
```

---

# Position Property

The `position` property controls how an element is placed on a webpage.

---

## Static

### Characteristics

* Default position value.
* Elements follow normal document flow.
* `top`, `right`, `bottom`, `left`, and `z-index` do not work.

```css
position: static;
```

---

## Relative

### Characteristics

* Element remains in normal document flow.
* Can be moved relative to its original position.

```css
position: relative;
top: 20px;
left: 10px;
```

---

## Absolute

### Characteristics

* Removed from normal document flow.
* Positioned relative to the nearest positioned ancestor.

```css
position: absolute;
top: 50px;
left: 100px;
```

---

## Fixed

### Characteristics

* Positioned relative to the viewport.
* Remains visible even when the page is scrolled.

```css
position: fixed;
bottom: 20px;
right: 20px;
```

---

# Z-Index

The `z-index` property controls the stacking order of elements along the Z-axis.

### Characteristics

* Works only on positioned elements:

  * relative
  * absolute
  * fixed
  * sticky
* Accepts positive and negative integer values.
* Higher values appear above lower values.

### Example

```css
.box1 {
    z-index: 2;
}

.box2 {
    z-index: 1;
}
```

Result:

```text
box1 appears above box2
```