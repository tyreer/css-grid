# CSS Grid

### 3 CSS Grid Fundamentals

_implicit grid_ means sizing by default or assumption if not specified

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
<div>
```

```CSS
.container {
  display: grid;
  grid-template-columns: repeat(5, 100px);
  grid-template-rows: 200px 75px;
  grid-gap: 20px;
}
```

### 5 Implicit vs Explicit Tracks

```css
grid-auto-rows: 100px 20px;
```

+  Provides a rule for implicit grid rows
  + In this case the rows will alternate between the two heights

### 6 grid-auto-flow Explained

```css
grid-auto-flow: column;
grid-auto-columns: 100px 20px;
```

+ Default value is _row_, but _column_ allows horizontal tracks to be the implicit result
