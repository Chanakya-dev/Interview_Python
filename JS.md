### **Basic JavaScript Concepts**

#### **1. What are the different data types in JavaScript?**
JavaScript has primitive types: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, and `bigint`.

#### **2. Explain the difference between `let`, `const`, and `var`.**
- `var`: Function-scoped, can be redeclared and updated.
- `let`: Block-scoped, can be updated but not redeclared.
- `const`: Block-scoped, cannot be updated or redeclared.

#### **3. What is the difference between `==` and `===`?**
- `==` checks for value equality with type coercion.
- `===` checks for strict equality (value and type).

#### **4. What is a closure in JavaScript?**
A closure is a function that remembers the scope in which it was created.

#### **5. Explain the difference between `null` and `undefined`.**
- `null`: Assigned explicitly to indicate no value.
- `undefined`: Default value when a variable is not assigned.

### **Functions and Scope**

#### **6. What are arrow functions, and how are they different from regular functions?**
Arrow functions have a shorter syntax and do not bind `this`.

#### **7. What is the purpose of the `this` keyword?**
`this` refers to the object that owns the function being executed.

#### **8. What is the difference between function declaration and function expression?**
- **Function Declaration**: Named function that can be hoisted.
- **Function Expression**: Assigned to a variable and not hoisted.

#### **9. What is the difference between synchronous and asynchronous programming?**
- **Synchronous**: Code runs sequentially.
- **Asynchronous**: Code execution does not block the main thread.

#### **10. Explain the Event Loop in JavaScript.**
The Event Loop manages execution of asynchronous code using the call stack, web APIs, and callback queue.

### **Objects and Arrays**

#### **11. How do you clone an object in JavaScript?**
Objects can be cloned using the spread operator or `Object.assign()`.

#### **12. What are JavaScript array methods like `map`, `filter`, and `reduce`?**
- `map()`: Transforms array elements.
- `filter()`: Filters elements based on condition.
- `reduce()`: Aggregates values.

#### **13. What is destructuring in JavaScript?**
Destructuring allows extracting values from objects or arrays.

#### **14. What is the difference between `forEach` and `map`?**
- `forEach` executes a function but does not return a new array.
- `map` returns a new transformed array.

### **Promises and Async/Await**

#### **15. What is a Promise in JavaScript?**
A Promise represents a value that may be available now, later, or never.

#### **16. Explain async and await in JavaScript.**
Async/await simplifies asynchronous code execution.

### **DOM Manipulation and Events**

#### **17. How do you select an element in JavaScript?**
- `document.getElementById('id')`
- `document.querySelector('.class')`

#### **18. What are event listeners in JavaScript?**
Event listeners allow handling user interactions.

#### **19. Explain event delegation in JavaScript.**
Event delegation allows handling events at a parent level instead of multiple child elements.

### **Advanced Concepts**

#### **20. What is debouncing and throttling in JavaScript?**
- **Debouncing**: Delays execution of a function until after a specified time.
- **Throttling**: Ensures a function executes at most once in a specified time interval.

#### **21. What is the difference between localStorage, sessionStorage, and cookies?**
- `localStorage`: Persistent storage.
- `sessionStorage`: Data is cleared after session ends.
- `cookies`: Small data storage sent with HTTP requests.

#### **22. What are modules in JavaScript?**
Modules allow code reusability and separation using `export` and `import`.

#### **23. Explain the concept of Hoisting in JavaScript.**
Hoisting moves function and variable declarations to the top of their scope before execution.

#### **24. What is the difference between deep and shallow copy?**
- **Shallow copy**: Copies references to nested objects.
- **Deep copy**: Creates independent copies of nested objects.

#### **25. What are WeakMap and WeakSet?**
- **WeakMap**: Holds weak references to keys (garbage collected).
- **WeakSet**: Stores weak object references.

#### **26. What is the difference between `apply`, `call`, and `bind`?**
- `call()`: Calls a function with arguments.
- `apply()`: Calls a function with an array of arguments.
- `bind()`: Returns a new function with `this` bound.

#### **27. Explain JavaScript’s prototype and prototypal inheritance.**
Objects inherit properties and methods from their prototype.

#### **28. What are Symbols in JavaScript?**
Symbols create unique identifiers that prevent property name collisions.

#### **29. What is the difference between `setTimeout` and `setInterval`?**
- `setTimeout()`: Runs code once after a delay.
- `setInterval()`: Runs code repeatedly at a specified interval.

#### **30. What is a Generator function in JavaScript?**
Generator functions use `function*` syntax and `yield` for lazy execution.
