# Template Literals in JavaScript

> **Category:** ES6+ Features | **Level:** 🟢 Beginner

---

## 📌 Definition

**Template literals** are strings enclosed in backticks (`` ` ``) that allow embedded expressions, multi-line strings, and string interpolation — introduced in **ES6**.

---

## 🔑 Key Features

### 1. String Interpolation

Embed variables or expressions directly inside a string using `${}`.

```js
const name = "John";
console.log(`Hello, ${name}!`); // Hello, John!
```

---

### 2. Expression Evaluation

Any valid JavaScript expression can go inside `${}`.

```js
const a = 5,
  b = 10;
console.log(`Sum is ${a + b}`); // Sum is 15
console.log(`${age >= 18 ? "Adult" : "Minor"}`);
console.log(`Today is ${new Date().toDateString()}`);
```

---

### 3. Multi-line Strings

No need for `\n` — just press Enter inside backticks.

```js
// ❌ Old way
const msg = "Line 1\nLine 2\nLine 3";

// ✅ Template Literal
const msg = `Line 1
Line 2
Line 3`;
```

---

### 4. Nested Template Literals

```js
const result = `Hello ${isLoggedIn ? `${username}` : "Guest"}`;
```

---

## ⚖️ Old Way vs Template Literals

```js
// ❌ Old way — messy concatenation
"Hello " +
  name +
  ", you are " +
  age +
  " years old."
  // ✅ Template Literal — clean & readable
  `Hello ${name}, you are ${age} years old.`;
```

---

## 🎯 Key Point to Say in Interview

> _"Template literals make string concatenation cleaner and more readable. They support multi-line strings and any valid JavaScript expression inside `${}`."_

---

## 🔗 Related Topics

- [What is JavaScript and its common uses?](./answers/javascript.md)

---

[⬅️ Back to Question List](../README.md)
