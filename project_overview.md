# 📋 Project Overview — Color Vocabulary App

## 🎯 Goal
A focused beginner CSS exercise emphasizing **selector specificity** and basic visual properties. The HTML is intentionally locked to teach the lesson that CSS can fully control appearance without modifying HTML structure.

## 📄 HTML Structure (Pre-Built, Read-Only)
```html
<body>
  <h1>Colors</h1>               ← Page title
  <h2>Learn the colors...</h2>  ← Subtitle
  
  <h2 class="color-title" id="red">Rojo</h2>
  <img src="./assets/images/red.png" alt="red" />
  
  <h2 class="color-title" id="blue">Azul</h2>
  <img src="./assets/images/blue.png" alt="blue" />
  
  <!-- ...and orange, green, yellow -->
</body>
```

## 🧠 CSS Tasks Explained

### Task 1: Color the Headings
Each `h2` has a unique `id`. Use ID selectors to target each one:
```css
#red   { color: red; }
#blue  { color: blue; }
#orange { color: orange; }
#green { color: green; }
#yellow { color: gold; }
```

### Task 2: Normal Font Weight
The default `h2` weight is `bold`. Override it:
```css
.color-title { font-weight: normal; }
```

### Task 3: Fixed Image Size
Make all images exactly 200×200 pixels:
```css
img {
  width: 200px;
  height: 200px;
}
```

## 🎓 Key Concepts

### CSS Specificity (Why Some Rules Win)
Specificity determines which CSS rule applies when multiple rules target the same element:
- **ID selector** `#red` has specificity **0,1,0,0** (highest)
- **Class selector** `.color-title` has specificity **0,0,1,0** (medium)
- **Element selector** `h2` has specificity **0,0,0,1** (lowest)

This is why `#red { color: red; }` will correctly override any general `h2` color rule.

## 📊 Difficulty Level
| Aspect | Rating |
|---|---|
| HTML | ⭐ (none — pre-written) |
| CSS | ⭐⭐ (beginner, short) |
| Concepts | ⭐⭐ (id/class selectors, specificity) |
| Overall | ⭐ Very Beginner-Friendly |

## 💡 Next Steps
- Add a background gradient behind each color section
- Make each section a card with padding and border-radius
- Add hover animations
- Try doing the same with a CSS variable `--color-highlight`
