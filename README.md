# Internship Assignment – JavaScript (var, let, const)

## Topic: JavaScript Variables (var, let, const)

---

## SECTION A: Technical Questions

### 1. What is the difference between `var`, `let`, and `const`?

| Feature | var | let | const |
|------|-----|-----|------|
| Scope | Function scope | Block scope | Block scope |
| Redeclaration | Allowed | Not allowed | Not allowed |
| Reinitialization | Allowed | Allowed | Not allowed |
| Hoisting | Yes (initialized as undefined) | Yes (temporal dead zone) | Yes (temporal dead zone) |

---

### 2. Which keyword allows redeclaration and why?

**`var`** allows redeclaration because it is function-scoped and does not follow strict block scoping rules.

---

### 3. Which keyword allows reinitialization?

Both **`var`** and **`let`** allow reinitialization.

---

### 4. Which keyword does not allow redeclaration and reinitialization?

**`const`** does not allow redeclaration or reinitialization.

---

### 5. Why should `const` be used for fixed values?

Because `const` prevents reassignment, ensuring the value remains unchanged throughout the program.

---

### 6. What error occurs when redeclaring a `let` variable?

**SyntaxError: Identifier has already been declared**

---

### 7. What error occurs when reassigning a `const` variable?

**TypeError: Assignment to constant variable**

---

### 8. Which keyword is preferred in modern JavaScript and why?

**`let` and `const`** are preferred because they provide block scope and prevent bugs caused by hoisting and redeclaration.

---

### 9. Can `const` be declared without initialization? Explain.

No. `const` must be initialized at the time of declaration, otherwise it throws a syntax error.

---

### 10. When should `var` be avoided?

`var` should be avoided in modern JavaScript because it can cause unexpected behavior due to function scope and hoisting.

---

## SECTION B: Code-Based Questions

### 11. Predict the output:

```javascript
var a = 10;
a = 20;
var a = 30;
console.log(a);
````

**Output:**

```text
30
```

---

### 12. Predict the output:

```javascript
let b = 5;
b = 15;
console.log(b);
```

**Output:**

```text
15
```

---

### 13. Identify the error:

```javascript
let x = 10;
let x = 20;
```

**Error:**
SyntaxError – redeclaration of `let` variable is not allowed.

---

### 14. Identify the error:

```javascript
const y = 50;
y = 100;
```

**Error:**
TypeError – reassignment to a constant variable.

---

### 15. Write a program using `var` to show redeclaration.

```javascript
var name = "Harish";
var name = "Babu";
console.log(name);
```

**Output:**

```text
Babu
```

---

### 16. Write a program using `let` to show reinitialization.

```javascript
let count = 1;
count = 2;
console.log(count);
```

**Output:**

```text
2
```

---

### 17. Write a program using `const` and explain why value cannot change.

```javascript
const PI = 3.14;
console.log(PI);
```

**Explanation:**
The value cannot be changed because `const` variables cannot be reassigned.

---

### 18. Convert `var` to `let` where applicable.

```javascript
let age = 25;
age = 26;
```

---

### 19. Convert `var` to `const` where applicable.

```javascript
const country = "India";
```

---

### 20. Write your own example for `var`, `let`, and `const`.

```javascript
var city = "Chennai";

let score = 90;
score = 95;

const college = "ABC Engineering College";

console.log(city, score, college);
```

---

## End of Assignment

```



