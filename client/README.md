# Questions Web App - Starter Project

A simple, modern web application built with HTML, CSS, and JavaScript that demonstrates fundamental web development concepts.

## 📁 Project Structure

```
starter-project/
├── client/
│   ├── index.html      # Main HTML structure
│   ├── script.js       # JavaScript functionality
│   └── style.css       # Styling and layout
└── README.md           # This file
```

## 🎯 Project Overview

This is a **single-page application (SPA)** designed to display different screens (like a questions app) without reloading the page. It uses modern CSS techniques for responsive design and clean layouts.

## 🏗️ HTML Structure (`index.html`)

### Document Setup
- **DOCTYPE**: HTML5 document declaration
- **Language**: English (`lang="en"`)
- **Meta tags**: UTF-8 encoding and responsive viewport
- **External files**: Links to CSS stylesheet

### Main Structure
```html
<div class="container">
    <div class="screen active" id="start-screen"></div>
    <div></div>
</div>
```

### Key Concepts: Classes vs IDs

#### **Classes (`class="..."`)**
- **Purpose**: Group multiple elements with similar styling/behavior
- **Multiple elements**: Can be applied to many elements
- **CSS selector**: Use dot (`.`) - `.screen`, `.active`
- **JavaScript**: `document.getElementsByClassName()`

**In your code**:
- `screen` - Groups all screen elements together
- `active` - Indicates currently visible screen

#### **IDs (`id="..."`)**
- **Purpose**: Uniquely identify a single element
- **Single element**: Only one element per ID
- **CSS selector**: Use hash (`#`) - `#start-screen`
- **JavaScript**: `document.getElementById()`

**In your code**:
- `start-screen` - Uniquely identifies the starting screen

## 🎨 CSS Concepts (`style.css`)

### 1. CSS Reset (`*` selector)
```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```
- **Universal selector**: `*` targets every element
- **Clean slate**: Removes browser default styles
- **Box model**: `border-box` includes padding/borders in dimensions

### 2. Body Styling
```css
body {
    background-color: #f5efe6;        /* Light beige background */
    display: flex;                    /* Flexbox container */
    justify-content: center;          /* Center horizontally */
    align-items: center;              /* Center vertically */
    min-height: 100vh;               /* Full viewport height */
    padding: 1rem;                   /* 16px spacing */
    font-family: sans-serif;         /* Clean font */
}
```

**Flexbox Layout**:
- **`display: flex`**: Creates flexible container
- **`justify-content: center`**: Centers content horizontally
- **`align-items: center`**: Centers content vertically

**Units Explained**:
- **`rem`**: Relative to root font size (1rem = 16px)
- **`vh`**: Viewport height (100vh = full screen)
- **`px`**: Fixed pixel values

### 3. Container Styling
```css
.container {
    background-color: white;          /* White background */
    border-radius: 1rem;             /* Rounded corners (16px) */
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1); /* Subtle shadow */
    width: 100%;                     /* Full width */
    max-width: 600px;                /* Maximum width limit */
    overflow: hidden;                 /* Hide overflow content */
    position: relative;               /* Positioning context */
}
```

**Visual Effects**:
- **`border-radius`**: Rounds corners for modern look
- **`box-shadow`**: Creates depth with shadow
  - Format: `horizontal-offset vertical-offset blur-radius color`
  - Example: `0 10px 30px rgba(0, 0, 0, 0.1)`

**Layout Control**:
- **`max-width`**: Responsive design (100% width up to 600px)
- **`overflow: hidden`**: Hides content outside container
- **`position: relative`**: Sets positioning context for children

## 🔧 JavaScript (`script.js`)

Currently empty, but ready for:
- Screen switching logic
- Question handling
- User interactions
- Dynamic content updates

## 🎯 How It All Works Together

1. **HTML** provides the structure with screens and container
2. **CSS** creates a centered card layout with modern styling
3. **JavaScript** (when added) will handle screen transitions and functionality

## 🚀 Getting Started

1. **Open** `client/index.html` in a web browser
2. **View** the centered white container on beige background
3. **Inspect** the code to understand the structure
4. **Modify** CSS values to see how they affect the layout

## 📚 Key Learning Concepts

### **CSS Box Model**
- **Margin**: Space outside element
- **Border**: Element boundary
- **Padding**: Space inside element
- **Content**: Actual element content

### **Flexbox Layout**
- **Container**: Parent element with `display: flex`
- **Items**: Child elements that flex
- **Justify**: Horizontal alignment
- **Align**: Vertical alignment

### **Responsive Design**
- **Viewport units**: `vh`, `vw` for screen-relative sizing
- **Max-width**: Prevents elements from becoming too wide
- **Percentage widths**: Adapt to parent container

### **Modern CSS Features**
- **Box shadows**: Create depth and visual interest
- **Border radius**: Rounded corners for modern look
- **CSS reset**: Consistent cross-browser styling

## 🔮 Next Steps

To complete this app, you could add:
- More screen divs for different questions
- CSS for screen transitions
- JavaScript for showing/hiding screens
- Question content and user interactions
- Animations and transitions

## 💡 Tips for Learning

1. **Experiment**: Change CSS values and see what happens
2. **Inspect**: Use browser dev tools to see how elements are styled
3. **Comment**: Add comments to explain what each CSS rule does
4. **Practice**: Try recreating similar layouts from scratch

---

**Happy Coding! 🎉**
