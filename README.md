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

📌 Tasks Overview

✅ Task 1 — `slugify(title)`

Converts a string into a URL-friendly slug by converting to lowercase and replacing spaces with hyphens.
js
function slugify(title) {
  return title.toLowerCase().replace(/\s+/g, "-");
}
Examples:

js
slugify("Arrays for beginners"); // "arrays-for-beginners"
slugify("How to become a JUNIOR developer in TWO WEEKS"); // "how-to-become-a-junior-developer-in-two-weeks"

✅ Task 2 — makeArray(firstArray, secondArray, maxLength)
Merges two arrays and returns a new array truncated to maxLength if needed.

js
function makeArray(firstArray, secondArray, maxLength) {
  const twoArray = firstArray.concat(secondArray);
  if (twoArray.length > maxLength) {
    return twoArray.slice(0, maxLength);
  }
  return twoArray;
}
Examples:

js
Копировать
Редактировать
makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3); // ["Mango", "Poly", "Ajax"]
makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0); // []

✅ Task 3 — filterArray(numbers, value)
Returns a new array containing only the elements from numbers greater than value.

js
function filterArray(numbers, value) {
  let countNumber = [];
  for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] > value) {
      countNumber.push(numbers[i]);
    }
  }
  return countNumber;
}
Examples:

js
filterArray([1, 2, 3, 4, 5], 3); // [4, 5]
filterArray([12, 24, 8, 41, 76], 38); // [41, 76]
🧠 What You'll Practice
String methods: toLowerCase(), replace()

Array methods: concat(), slice()

Looping through arrays with for

Conditional filtering of arrays

Writing reusable functions

