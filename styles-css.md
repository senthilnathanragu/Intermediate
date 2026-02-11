## CSS Styling & Page Layout (5 Hours)

### Teaching Content for 1st Year Students (Simple Level)

---

# 1. Introduction to CSS (What is CSS?)

### Meaning:

CSS stands for **Cascading Style Sheets**.

### Purpose:

CSS is used to **design and style** HTML web pages.

### What CSS can do?

* Change text color
* Change font style and size
* Add background colors/images
* Set spacing (margin/padding)
* Arrange layout (flexbox)
* Make websites responsive (mobile-friendly)

### Example:

HTML = Structure
CSS = Design / Beauty

---

# 2. Types of CSS

### 1. Inline CSS

Written inside the HTML tag.

```html
<h1 style="color: red;">Hello</h1>
```

### 2. Internal CSS

Written inside `<style>` tag in HTML.

```html
<style>
  h1 {
    color: blue;
  }
</style>
```

### 3. External CSS (Most Used)

Written in a separate `.css` file.

HTML:

```html
<link rel="stylesheet" href="style.css">
```

CSS File (style.css):

```css
h1 {
  color: green;
}
```

---

# 3. CSS Syntax

### Format:

```css
selector {
  property: value;
}
```

### Example:

```css
p {
  color: blue;
  font-size: 18px;
}
```

* Selector = `p`
* Property = `color`
* Value = `blue`

---

# 4. Colors in CSS

CSS supports multiple color formats.

### 1. Color Name

```css
color: red;
```

### 2. Hex Code

```css
color: #ff0000;
```

### 3. RGB

```css
color: rgb(255, 0, 0);
```

### Background color example:

```css
body {
  background-color: lightgray;
}
```

---

# 5. Fonts in CSS

### Change font style:

```css
p {
  font-family: Arial;
}
```

### Change font size:

```css
p {
  font-size: 20px;
}
```

### Bold and Italic:

```css
h1 {
  font-weight: bold;
  font-style: italic;
}
```

---

# 6. Backgrounds in CSS

### Background Color:

```css
div {
  background-color: yellow;
}
```

### Background Image:

```css
body {
  background-image: url("image.jpg");
}
```

### Background Repeat and Size:

```css
body {
  background-repeat: no-repeat;
  background-size: cover;
}
```

---

# 7. Box Model (Very Important Topic)

Every HTML element is treated as a **box**.

### Box Model Parts:

1. Content
2. Padding
3. Border
4. Margin

### Example:

```css
div {
  width: 200px;
  padding: 20px;
  border: 2px solid black;
  margin: 30px;
}
```

### Explanation:

* **Padding** = Space inside the box
* **Border** = Line around the box
* **Margin** = Space outside the box

---

# 8. Margin and Padding Difference

### Margin:

Space outside the element.

```css
div {
  margin: 20px;
}
```

### Padding:

Space inside the element.

```css
div {
  padding: 20px;
}
```

---

# 9. CSS Borders

### Example:

```css
div {
  border: 3px solid blue;
}
```

Border types:

* solid
* dotted
* dashed
* double

---

# 10. CSS Width and Height

```css
div {
  width: 300px;
  height: 150px;
}
```

---

# 11. Layout Techniques (Flexbox Basics)

Flexbox is used to arrange items in a row or column.

### Flexbox Example:

```css
.container {
  display: flex;
}
```

### Example with spacing:

```css
.container {
  display: flex;
  justify-content: space-between;
}
```

### Common Flexbox Properties:

* `display: flex`
* `justify-content` (horizontal alignment)
* `align-items` (vertical alignment)
* `gap` (space between items)

---

# 12. Flexbox Example Layout

HTML:

```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
  <div class="box">Box 3</div>
</div>
```

CSS:

```css
.container {
  display: flex;
  gap: 10px;
}

.box {
  background-color: lightblue;
  padding: 20px;
  border: 1px solid black;
}
```

---

# 13. Responsive Design Concepts

Responsive means the webpage should look good on:

* Mobile
* Tablet
* Laptop

### How to make responsive?

* Use percentage widths
* Use flexbox
* Use media queries

---

# 14. Media Queries (Basic)

Media queries apply CSS based on screen size.

Example:

```css
@media (max-width: 600px) {
  body {
    background-color: lightgreen;
  }
}
```

Meaning:
If screen width is less than 600px, apply this style.

---

# 15. Simple Responsive Layout Example

HTML:

```html
<div class="layout">
  <div class="left">Left</div>
  <div class="right">Right</div>
</div>
```

CSS:

```css
.layout {
  display: flex;
  gap: 10px;
}

.left, .right {
  padding: 20px;
  background-color: lightgray;
  width: 50%;
}

@media (max-width: 600px) {
  .layout {
    flex-direction: column;
  }

  .left, .right {
    width: 100%;
  }
}
```

---

# 16. Hands-On Task 1: Style a Web Page Using CSS

### Task:

Create a simple webpage with:

* Heading
* Paragraph
* Button
* Background color

HTML:

```html
<h1>Welcome to My Page</h1>
<p>This is my first styled webpage.</p>
<button>Click Me</button>
```

CSS:

```css
body {
  background-color: lightyellow;
  font-family: Arial;
  text-align: center;
}

h1 {
  color: darkblue;
}

p {
  font-size: 18px;
}

button {
  padding: 10px 20px;
  background-color: blue;
  color: white;
  border: none;
}
```

---

# 17. Hands-On Task 2: Create a Simple Responsive Layout

### Task:

Create 3 boxes in a row on desktop
and in a column on mobile.

HTML:

```html
<div class="container">
  <div class="box">Home</div>
  <div class="box">About</div>
  <div class="box">Contact</div>
</div>
```

CSS:

```css
.container {
  display: flex;
  gap: 10px;
}

.box {
  flex: 1;
  background-color: orange;
  padding: 20px;
  text-align: center;
}

@media (max-width: 600px) {
  .container {
    flex-direction: column;
  }
}
```

---

# 18. Summary (Final Notes for Students)

### CSS is used for:

* Styling text
* Changing colors and fonts
* Creating layouts
* Making webpages responsive

### Important topics:

* CSS syntax
* Colors and fonts
* Background
* Box model
* Flexbox basics
* Media queries

---

If you want, I can also give you a **5-hour teaching timetable** (hour-wise breakdown) for this topic.
