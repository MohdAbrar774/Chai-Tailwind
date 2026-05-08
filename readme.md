# 🎨 ChaiCSS — Lightweight Utility-First CSS Engine

A lightweight utility-first CSS engine built using pure JavaScript that dynamically converts custom utility classes into inline styles at runtime.

Inspired by utility-first CSS frameworks like Tailwind CSS, this project allows developers to write classes such as:

```html id="a41jvg"
<div class="chai-p-20 chai-bg-red chai-text-center chai-fs-24">
  Hello World
</div>
```

The JavaScript engine scans the DOM, parses all `chai-*` classes, and applies the corresponding styles dynamically.

---

## 🚀 Features

* ✅ Utility-first CSS engine built from scratch
* ✅ Pure HTML + JavaScript project
* ✅ Dynamic DOM traversal and parsing
* ✅ Runtime style generation
* ✅ Inline style application
* ✅ Lightweight and framework-independent
* ✅ Reusable utility parsing system
* ✅ Dynamic padding utilities
* ✅ Dynamic margin utilities
* ✅ Dynamic font-size utilities

---

## ⚙️ Tech Stack

### Frontend

* HTML
* JavaScript
* CSS (optional for base styling)

---

## 🧠 Project Goal

The goal of this project is to understand:

* DOM traversal
* Dynamic style manipulation
* Utility-first CSS architecture
* Pattern parsing in JavaScript
* Runtime CSS generation

---

## 🏗️ Project Structure

```id="cqww44"
.
├── index.html
├── app.js
└── README.md
```

---

## ⚡ Getting Started

### 1. Clone the repository

```bash id="y93j5x"
git clone https://github.com/your-username/chai-css-engine.git
cd chai-css-engine
```

---

### 2. Open project

Simply open:

```id="m7d6i7"
index.html
```

in your browser.

No build tools or dependencies required.

---

## 🎯 How It Works

### Example

```html id="a9fxzb"
<div class="chai-p-20 chai-m-10 chai-bg-blue chai-text-center chai-fs-24">
  ChaiCSS Engine
</div>
```

The engine converts this into:

```css id="i4j0yb"
padding: 20px;
margin: 10px;
background-color: blue;
text-align: center;
font-size: 24px;
```

and applies the styles dynamically using JavaScript.

---

## 🔍 Core Workflow

1. Traverse DOM after page load
2. Find all classes starting with `chai-`
3. Parse utility patterns
4. Extract dynamic values from class names
5. Generate corresponding styles
6. Apply inline styles dynamically
7. Remove or ignore processed utility classes

---

## 🧪 Supported Utility Classes

### 📦 Spacing Utilities

| Utility      | CSS                    |
| ------------ | ---------------------- |
| `chai-p-20`  | `padding: 20px`        |
| `chai-pt-10` | `padding-top: 10px`    |
| `chai-pb-15` | `padding-bottom: 15px` |
| `chai-pl-5`  | `padding-left: 5px`    |
| `chai-pr-5`  | `padding-right: 5px`   |
| `chai-m-20`  | `margin: 20px`         |
| `chai-mt-10` | `margin-top: 10px`     |
| `chai-mb-15` | `margin-bottom: 15px`  |

---

### 🎨 Colors

| Utility           | CSS                       |
| ----------------- | ------------------------- |
| `chai-bg-red`     | `background-color: red`   |
| `chai-bg-black`   | `background-color: black` |
| `chai-text-white` | `color: white`            |
| `chai-text-blue`  | `color: blue`             |

---

### ✍️ Typography

| Utility            | CSS                  |
| ------------------ | -------------------- |
| `chai-text-center` | `text-align: center` |
| `chai-text-left`   | `text-align: left`   |
| `chai-fs-12`       | `font-size: 12px`    |
| `chai-fs-24`       | `font-size: 24px`    |
| `chai-fw-bold`     | `font-weight: bold`  |

---

### 🔲 Borders & Radius

| Utility           | CSS                       |
| ----------------- | ------------------------- |
| `chai-border-1`   | `border: 1px solid black` |
| `chai-border-2`   | `border: 2px solid black` |
| `chai-rounded-10` | `border-radius: 10px`     |
| `chai-rounded-20` | `border-radius: 20px`     |

---

### 📐 Layout Utilities

| Utility               | CSS                       |
| --------------------- | ------------------------- |
| `chai-flex`           | `display: flex`           |
| `chai-grid`           | `display: grid`           |
| `chai-justify-center` | `justify-content: center` |
| `chai-items-center`   | `align-items: center`     |

---

## 🧠 Example Parsing Logic

### Dynamic Padding

```js id="tcz7d5"
if (className.startsWith("chai-p-")) {
  const value = className.split("-")[2];
  element.style.padding = `${value}px`;
}
```

---

### Dynamic Margin

```js id="84p5q8"
if (className.startsWith("chai-m-")) {
  const value = className.split("-")[2];
  element.style.margin = `${value}px`;
}
```

---

### Dynamic Font Size

```js id="3itp7h"
if (className.startsWith("chai-fs-")) {
  const value = className.split("-")[2];
  element.style.fontSize = `${value}px`;
}
```

---

## 🎨 Example Usage

```html id="quw2i4"
<div
  class="
    chai-bg-black
    chai-text-white
    chai-p-20
    chai-m-10
    chai-rounded-12
    chai-text-center
    chai-fs-24
  "
>
  Utility First CSS Engine
</div>
```

---

## 🚀 Future Improvements

* ⚡ Dynamic stylesheet generation instead of inline styles
* 📱 Responsive utility support
* 🌙 Dark mode utilities
* 🎨 Theme system
* 🧩 Plugin architecture
* 🔥 Tailwind-style breakpoint support
* 📦 Minified production build
* 🧠 Utility caching for performance optimization

---

## 📊 Possible Enhancements

* MutationObserver support for dynamic DOM updates
* CSS variable support
* Custom utility registration
* Config-driven design tokens
* Runtime utility compiler

---

## 🛡️ Challenges Solved

* DOM traversal
* Dynamic utility parsing
* Pattern matching and extraction
* Runtime style application
* Reusable utility engine architecture

---

## 📜 License

MIT License

---

## 👨‍💻 Author

Built as a JavaScript DOM manipulation and utility-first CSS engine project to explore:

* Runtime styling systems
* Utility-first CSS architecture
* Dynamic frontend rendering
* JavaScript parsing logic
* Client-side style generation

---

## ⭐ Learning Outcomes

By building this project, you learn:

* DOM traversal and manipulation
* Parsing structured utility patterns
* Dynamic inline style generation
* Building reusable frontend utilities
* Understanding utility-first CSS systems
* Creating lightweight frontend libraries
* Handling dynamic styling with JavaScript
