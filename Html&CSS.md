## **1. HTML Basics**
### **1. What is HTML, and why is it used?**  
HTML (**HyperText Markup Language**) is the standard markup language used to structure content on the web. It defines the elements and structure of a webpage.  

### **2. What are HTML elements and tags?**  
- **HTML Elements:** The building blocks of a webpage (`<p>Paragraph</p>`).  
- **HTML Tags:** The keywords that define elements (`<h1>`, `<div>`, `<span>`).  

### **3. What is the difference between HTML and XHTML?**  
- **HTML:** More flexible, does not enforce strict rules.  
- **XHTML:** Stricter, follows XML rules (proper nesting, lowercase tags, closing tags required).  

### **4. What is the difference between block-level and inline elements?**  
- **Block-Level:** Takes full width, starts on a new line (`<div>`, `<p>`, `<h1>`).  
- **Inline:** Stays within a line (`<span>`, `<a>`, `<strong>`).  

### **5. What are semantic HTML elements?**  
Semantic elements describe their meaning (`<article>`, `<section>`, `<header>`, `<footer>`), improving accessibility and SEO.  

---

## **2. HTML Forms & Attributes**
### **6. What is the difference between `id` and `class` attributes?**  
- **id:** Unique, used for a single element (`id="header"`).  
- **class:** Reusable, applies to multiple elements (`class="button"`).  

### **7. What are the different types of input fields in HTML forms?**  
Examples include:  
- **Text (`<input type="text">`)**  
- **Email (`<input type="email">`)**  
- **Password (`<input type="password">`)**  
- **Checkbox (`<input type="checkbox">`)**  
- **Radio (`<input type="radio">`)**  
- **File Upload (`<input type="file">`)**  

### **8. What is the difference between GET and POST methods in forms?**  
- **GET:** Sends data in the URL, less secure, limited data size.  
- **POST:** Sends data in the request body, secure, allows large data.  

### **9. What is the `action` and `method` attribute in forms?**  
- **action:** Specifies the URL to send form data (`action="submit.php"`).  
- **method:** Defines how data is sent (`GET` or `POST`).  

### **10. What is the purpose of the `label` element in forms?**  
It improves accessibility by associating text with input fields (`<label for="email">Email:</label>`).  

---

## **3. HTML5 Features**
### **11. What are the new elements introduced in HTML5?**  
HTML5 introduced elements like `<article>`, `<section>`, `<nav>`, `<video>`, `<audio>`, `<canvas>`, `<progress>`, and `<details>`.  

### **12. What is the difference between `<b>` and `<strong>`?**  
- **`<b>` (Bold):** Used for styling (not semantically meaningful).  
- **`<strong>`:** Indicates importance (SEO and accessibility friendly).  

### **13. What is the difference between `<i>` and `<em>`?**  
- **`<i>` (Italic):** Used for styling text.  
- **`<em>`:** Emphasizes text (better for SEO).  

### **14. What is the difference between `<iframe>` and `<embed>`?**  
- **`<iframe>`:** Embeds another webpage.  
- **`<embed>`:** Embeds media files (videos, PDFs, etc.).  

### **15. What is the `data-*` attribute in HTML5?**  
It allows embedding custom data into elements (`<div data-user="123">`), useful for JavaScript interactions.  

---

## **4. CSS Basics**
### **16. What is CSS, and why is it used?**  
CSS (**Cascading Style Sheets**) is used to style HTML elements, controlling layout, colors, fonts, and responsiveness.  

### **17. What are the different ways to apply CSS to a webpage?**  
- **Inline CSS:** Directly in an element (`style="color: red;"`).  
- **Internal CSS:** Inside `<style>` tags within `<head>`.  
- **External CSS:** Using an external `.css` file (`<link rel="stylesheet" href="styles.css">`).  

### **18. What is the difference between relative, absolute, and fixed positioning in CSS?**  
- **Relative:** Positions relative to its normal position.  
- **Absolute:** Positions relative to the nearest positioned ancestor.  
- **Fixed:** Stays fixed relative to the viewport.  

### **19. What are pseudo-classes and pseudo-elements?**  
- **Pseudo-classes:** Define special states (`:hover`, `:focus`, `:nth-child(2)`).  
- **Pseudo-elements:** Style specific parts (`::before`, `::after`).  

### **20. What is the difference between `em`, `rem`, and `px`?**  
- **px:** Fixed pixel size.  
- **em:** Relative to the parent element's font size.  
- **rem:** Relative to the root element's font size.  

---

## **5. CSS Layout and Flexbox**
### **21. What is the difference between `inline`, `block`, and `inline-block`?**  
- **inline:** Cannot set width/height (`<span>`).  
- **block:** Takes full width (`<div>`).  
- **inline-block:** Inline but allows setting width/height.  

### **22. What is the difference between Flexbox and Grid?**  
- **Flexbox:** One-dimensional (row or column).  
- **Grid:** Two-dimensional (rows and columns).  

### **23. How does the `z-index` property work?**  
`z-index` controls the stacking order of elements (higher values appear on top).  

### **24. What is the difference between `max-width`, `min-width`, and `width`?**  
- **width:** Sets a fixed width.  
- **max-width:** Limits maximum width.  
- **min-width:** Ensures a minimum width.  

### **25. What is the difference between `visibility: hidden;` and `display: none;`?**  
- **`visibility: hidden;`** Hides the element but keeps space.  
- **`display: none;`** Removes the element from the layout.  

---

## **6. CSS Advanced**
### **26. What are media queries in CSS?**  
They enable responsive design based on screen size.  
```css
@media (max-width: 600px) {
  body { background-color: lightblue; }
}
```  

### **27. What is the difference between `absolute` and `relative` units in CSS?**  
- **Absolute:** Fixed sizes (`px`, `pt`, `cm`).  
- **Relative:** Flexible sizes (`em`, `rem`, `%`).  

### **28. What is the difference between `position: sticky;` and `position: fixed;`?**  
- **Sticky:** Sticks within a parent container when scrolling.  
- **Fixed:** Remains in place relative to the viewport.  

### **29. What is a CSS preprocessor?**  
A CSS preprocessor (e.g., **SASS, LESS**) extends CSS with features like variables, mixins, and functions.  

### **30. What is the difference between `nth-child()` and `nth-of-type()`?**  
- **`nth-child(n)`** Targets any nth child.  
- **`nth-of-type(n)`** Targets the nth child of a specific type.  
