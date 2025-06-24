# JavaScript Practice – Arrays and Strings

This project contains three beginner-friendly JavaScript tasks focused on string manipulation and array operations. These tasks help practice common methods like `toLowerCase()`, `replace()`, `concat()`, `slice()`, and loops.

---

## 📁 Project Structure

project/
└── index.html


All JavaScript code can be included inline or linked externally.

---

## 🚀 How to Run

1. Clone or download the repository.  
2. Open `index.html` in your browser.  
3. Open the browser **Console** (F12 or right-click → Inspect → Console tab) to see the output of the functions.

---

## 📌 Tasks Overview

Task 1 — `slugify(title)`

Converts a string into a URL-friendly slug by converting to lowercase and replacing spaces with hyphens.

function slugify(title) {
  return title.toLowerCase().replace(/\s+/g, "-");
}
