# PSEUDO CLASSES, TRANSITIONS, TRANSFORMS & ANIMATIONS

---

# Pseudo Classes

## Definition

Pseudo-classes are used to define special states of HTML elements.

### Syntax

```css
selector:pseudo-class {
    property: value;
}
```

### Common Pseudo Classes

#### `:hover`

Applies styles when the user hovers over an element.

#### `:active`

Applies styles when the element is being clicked.

#### `:first-child`

Targets the first child element of its parent.

### Example

```css
.btn {
    height: 20px;
    width: 70px;
    border: 1px solid blue;
    border-radius: 5px;
    background-color: aliceblue;
}

.btn:hover {
    height: 25px;
    width: 80px;
    border: 1px solid red;
}

.btn:active {
    height: 25px;
    width: 80px;
    border: 1px solid red;
    background-color: indianred;
}
```

### Uses

* Interactive buttons
* Navigation menus
* Form validation styling
* User interaction feedback

---

# CSS Transitions

## Definition

A CSS transition creates a smooth animation when a CSS property changes from one value to another.

### Transition Properties

#### `transition-property`

Specifies which CSS property will be animated.

#### `transition-duration`

Determines how long the transition takes.

#### `transition-timing-function`

Controls the speed curve of the transition.

Common values:

* `linear`
* `ease`
* `ease-in`
* `ease-out`
* `ease-in-out`

#### `transition-delay`

Adds a delay before the transition starts.

### Example

```css
.box {
    width: 100px;
    transition-property: width;
    transition-duration: 1s;
}

.box:hover {
    width: 200px;
}
```

---

# CSS Transform

## Definition

The `transform` property allows elements to be visually modified without affecting the layout of surrounding elements.

### Common Transform Functions

#### `rotate()`

Rotates an element around its center point.

```css
transform: rotate(45deg);
```

#### `scale()`

Increases or decreases the size of an element.

```css
transform: scale(1.5);
```

#### `translate()`

Moves an element from its original position.

```css
transform: translate(50px, 20px);
```

### Notes

* Does not affect surrounding elements.
* Useful for hover effects and animations.
* Can be combined with transitions.

### Example

```css
.box:hover {
    transform: rotate(20deg);
}
```

---

# CSS Animations

## Definition

CSS animations allow elements to change styles gradually over time using `@keyframes`.

### Animation Properties

#### `animation-name`

Specifies the name of the animation.

#### `animation-duration`

Defines how long one animation cycle takes.

#### `animation-timing-function`

Controls the animation speed curve.

Examples:

* `linear`
* `ease`
* `ease-in`
* `ease-out`
* `ease-in-out`

#### `animation-delay`

Adds a delay before the animation begins.

#### `animation-iteration-count`

Determines how many times the animation repeats.

Examples:

```css
animation-iteration-count: 3;
animation-iteration-count: infinite;
```

#### `animation-direction`

Controls the animation direction.

Values:

* `normal`
* `reverse`
* `alternate`
* `alternate-reverse`

### Example

```css
@keyframes moveRight {
    from {
        transform: translateX(0);
    }

    to {
        transform: translateX(200px);
    }
}

.box {
    animation-name: moveRight;
    animation-duration: 2s;
    animation-iteration-count: infinite;
}
```

---

# Difference Between Transition and Animation

| Transition                                 | Animation                          |
| ------------------------------------------ | ---------------------------------- |
| Triggered by an event (hover, click, etc.) | Can run automatically              |
| Requires a state change                    | Uses `@keyframes`                  |
| Simpler effects                            | More complex effects               |
| Usually used for hover effects             | Usually used for continuous motion |
