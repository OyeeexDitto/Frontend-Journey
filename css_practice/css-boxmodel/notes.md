# BOX MODEL

## Definition

The CSS Box Model describes how every HTML element is displayed as a rectangular box on a webpage.

It consists of four main components:

* Content
* Padding
* Border
* Margin

```text
+-------------------------+
|         Margin          |
|  +-------------------+  |
|  |      Border       |  |
|  |  +-------------+  |  |
|  |  |   Padding   |  |  |
|  |  | +---------+ |  |  |
|  |  | | Content | |  |  |
|  |  | +---------+ |  |  |
|  |  +-------------+  |  |
|  +-------------------+  |
+-------------------------+
```

### Components

#### Margin

The space outside the border that separates an element from other elements.

#### Border

The outline that surrounds the padding and content of an element.

#### Padding

The space between the content and the border.

#### Content

The innermost area that contains text, images, or other media.

---

# Padding Property

## Purpose

Defines the space between an element's content and its border.

### Individual Sides

Padding can be applied separately to each side:

```css
padding-top
padding-right
padding-bottom
padding-left
```

### Shorthand

```css
padding: 10px;
```

Applies equal padding to all sides.

```css
padding: 10px 20px 10px 20px;
```

Order:

```text
Top → Right → Bottom → Left
```

---

# Margin Property

## Purpose

Defines the space outside an element's border.

### Individual Sides

Margin can be applied separately to each side:

```css
margin-top
margin-right
margin-bottom
margin-left
```

### Shorthand

```css
margin: 10px;
```

Applies equal margin to all sides.

```css
margin: 10px 20px;
```

Order:

```text
Top & Bottom → Left & Right
```

```css
margin: 10px 20px 30px 40px;
```

Order:

```text
Top → Right → Bottom → Left
```

### Auto Value

```css
margin: auto;
```

Commonly used to center block-level elements horizontally.

---

# Border Property

## Purpose

Creates an outline around an HTML element.

### Components

A border consists of:

* Width
* Style
* Color

### Border Styles

Common styles include:

* solid
* dashed
* dotted
* double

### Shorthand

```css
border: 2px solid black;
```

---

# Border Radius

## Purpose

Used to create rounded corners on elements.

### Individual Corners

Each corner can be styled separately:

```css
border-top-left-radius
border-top-right-radius
border-bottom-right-radius
border-bottom-left-radius
```

### Shorthand

```css
border-radius: 10px;
```

Applies the same radius to all corners.

```css
border-radius: 10px 20px;
```

Applies different radii to corners.

### Circle Example

```css
height: 100px;
width: 100px;
border-radius: 50%;
```

Creates a perfect circle.
