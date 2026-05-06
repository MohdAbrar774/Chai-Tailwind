# 🎨 ChaiCSS — Lightweight Utility-First CSS Engine

A lightweight utility-first CSS engine built using pure JavaScript that dynamically converts custom utility classes into inline styles at runtime.

Inspired by utility-first CSS frameworks like Tailwind CSS, this project allows developers to write classes such as:

```html id="1dh4v4"
<div class="chai-p-20 chai-bg-red chai-text-center">
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

```id="dzl9vr"
.
├── index.html
├── app.js
└── README.md
```

---

## ⚡ Getting Started

### 1. Clone the repository

```bash id="g1x68u"
git clone https://github.com/your-username/chai-css-engine.git
cd chai-css-engine
```

---

### 2. Open project

Simply open:

```id="nprbn8"
index.html
```

in your browser.

No build tools or dependencies required.

---

## 🎯 How It Works

### Example

```html id="f3wq1y"
<div class="chai-p-20 chai-bg-blue chai-text-center">
  ChaiCSS Engine
</div>
```

The engine converts this into:

```css id="mr18x5"
padding: 20px;
background-color: blue;
text-align: center;
```

and applies the styles dynamically using JavaScript.

---

## 🔍 Core Workflow

1. Traverse DOM after page load
2. Find all classes starting with `chai-`
3. Parse utility patterns
4. Generate corresponding styles
5. Apply inline styles dynamically
6. Remove or ignore processed utility classes

---

## 🧪 Supported Utility Classes

### 📦 Spacing

| Utility     | CSS                |
| ----------- | ------------------ |
| `chai-p-20` | `padding: 20px`    |
| `chai-m-10` | `margin: 10px`     |
| `chai-pt-5` | `padding-top: 5px` |

---

### 🎨 Colors

| Utility           | CSS                     |
| ----------------- | ----------------------- |
| `chai-bg-red`     | `background-color: red` |
| `chai-text-white` | `color: white`          |

---

### ✍️ Typography

| Utility            | CSS                  |
| ------------------ | -------------------- |
| `chai-text-center` | `text-align: center` |
| `chai-fs-24`       | `font-size: 24px`    |
| `chai-fw-bold`     | `font-weight: bold`  |

---

### 🔲 Borders

| Utility           | CSS                       |
| ----------------- | ------------------------- |
| `chai-border-1`   | `border: 1px solid black` |
| `chai-rounded-10` | `border-radius: 10px`     |

---

### 📐 Layout

| Utility               | CSS                       |
| --------------------- | ------------------------- |
| `chai-flex`           | `display: flex`           |
| `chai-justify-center` | `justify-content: center` |
| `chai-items-center`   | `align-items: center`     |

---

## 🧠 Example Parsing Logic

```js id="4vmhzk"
const elements = document.querySelectorAll("*");

elements.forEach((element) => {
  element.classList.forEach((className) => {
    if (className.startsWith("chai-p-")) {
      const value = className.split("-")[2];
      element.style.padding = `${value}px`;
    }
  });
});
```

---

## 🎨 Example Usage

```html id="p8d3l9"
<div
  class="
    chai-bg-black
    chai-text-white
    chai-p-20
    chai-rounded-12
    chai-text-center
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

---

## 📊 Possible Enhancements

* MutationObserver support for dynamic DOM updates
* Utility caching for performance optimization
* Configurable design tokens
* CSS variable support
* Developer debugging tools

---

## 🛡️ Challenges Solved

* DOM traversal
* Pattern matching and parsing
* Dynamic style application
* Utility abstraction
* Reusable engine architecture

---

## 📜 License

MIT License

---

## 👨‍💻 Author

Built as a JavaScript DOM manipulation and utility-first CSS engine project to explore:

* Runtime style systems
* Utility CSS architecture
* Dynamic frontend rendering
* JavaScript parsing logic

---

## ⭐ Learning Outcomes

By building this project, you learn:

* DOM traversal and manipulation
* Parsing structured class patterns
* Dynamic inline style generation
* Building reusable frontend utilities
* Understanding utility-first CSS architecture
* Creating lightweight frontend libraries
