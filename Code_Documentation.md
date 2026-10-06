# Code Documentation - PHP Class Assignment 1

**Organization:** [Bincom-Academy-PHP-Assignments](https://github.com/Bincom-Academy-PHP-Assignments)  
**Student Name:** Shuraihu Usman  
**Role:** PHP / Backend Intern & Trainee  
**Academy:** Bincom Academy  
**Project Name:** PHP Class Assignment 1 - HTML & CSS Overview  
**GitHub Repository:** [https://github.com/Bincom-Academy-PHP-Assignments/PHP-Class-Assignment-1](https://github.com/Bincom-Academy-PHP-Assignments/PHP-Class-Assignment-1)  

---

## 1. Project Overview & Learning Objectives

This project fulfills the requirements of **Lesson 1** at Bincom Academy. It applies foundational web technologies to build a clean, accessible, one-page personal portfolio site using **HTML5** and **CSS3** (without backend PHP processing yet).

### Topics Covered in Lesson 1:
- **Setup Local Server:** Configuring XAMPP / WAMP and understanding web root directories (`htdocs` / `www`).
- **Setup Development Environment:** Configuring text editors (VS Code / Sublime Text) and browser developer tools.
- **Introduction to HTML & CSS:** Semantic tags, page hierarchy, and styling rules.
- **CSS Box Model:** Practical application of content, padding, and margin with flat aesthetics (zero borders and zero shadows).
- **Running & Testing:** Executing web pages in the browser and testing responsive structures.

---

## 2. GitHub Repository Information

- **Organization:** [https://github.com/Bincom-Academy-PHP-Assignments](https://github.com/Bincom-Academy-PHP-Assignments)
- **Repository URL:** [https://github.com/Bincom-Academy-PHP-Assignments/PHP-Class-Assignment-1](https://github.com/Bincom-Academy-PHP-Assignments/PHP-Class-Assignment-1)
- **Visibility:** Public
- **Clone Command:**
  ```bash
  git clone https://github.com/Bincom-Academy-PHP-Assignments/PHP-Class-Assignment-1.git
  ```

---

## 3. Directory Structure

```text
PHP-Class-Assignment-1/
├── index.html              # Core HTML5 semantic webpage structure
├── style.css               # Clean, flat CSS styling (no borders, no shadows)
├── ui_output_full.png      # Full-page screenshot of the rendered UI output
├── Code_Documentation.docx # Official technical report in Microsoft Word format
├── Code_Documentation.md   # Complete technical assignment documentation in Markdown
└── README.md               # Quick-start instructions and lesson overview
```

---

## 4. Key Code Implementations & Explanations

### A. HTML5 Structure (`index.html`)

The HTML markup emphasizes clean semantic landmarks, structured content sections, and accessible forms:

#### 1. Header & Navigation
```html
<header>
  <div class="container">
    <h1>Shuraihu Usman</h1>
    <p>PHP / Backend Intern &bull; Bincom Academy Trainee</p>
    <nav>
      <ul>
        <li><a href="#about">About Me</a></li>
        <li><a href="#learning">What I'm Learning</a></li>
        <li><a href="#hobbies">Hobbies &amp; Interests</a></li>
        <li><a href="#contact">Contact Me</a></li>
      </ul>
    </nav>
  </div>
</header>
```
*Explanation:* Uses `<header>` and `<nav>` with anchor links (`#about`, etc.) to provide smooth on-page navigation.

#### 2. Lists & Semantic Sections
```html
<section id="learning">
  <h2>What I Am Learning</h2>
  <p>My journey started with the fundamentals of web architecture...</p>
  <ul>
    <li><strong>HTML5:</strong> Semantic page structuring, forms, headings, lists, and links.</li>
    <li><strong>CSS3:</strong> Box model spacing (margins and padding), styling colors, typography...</li>
    <li><strong>Development Tools:</strong> Code editors and browser developer tools for testing.</li>
    <li><strong>Server Foundations:</strong> Configuring local servers like XAMPP and WAMP...</li>
  </ul>
</section>
```
*Explanation:* Demonstrates both unordered (`<ul>`) and ordered (`<ol>`) lists to present organized content.

#### 3. Interactive Contact Form
```html
<section id="contact">
  <h2>Get In Touch</h2>
  <form action="#" method="get">
    <div class="form-group">
      <label for="fullname">Your Name:</label>
      <input type="text" id="fullname" name="fullname" placeholder="Enter your full name" required>
    </div>
    <div class="form-group">
      <label for="email">Your Email:</label>
      <input type="email" id="email" name="email" placeholder="Enter your email address" required>
    </div>
    <div class="form-group">
      <label for="subject">Subject:</label>
      <select id="subject" name="subject">
        <option value="general">General Inquiry</option>
        <option value="networking">Networking &amp; Collaboration</option>
        <option value="feedback">Website Feedback</option>
      </select>
    </div>
    <div class="form-group">
      <label for="message">Message:</label>
      <textarea id="message" name="message" placeholder="Type your message here..." required></textarea>
    </div>
    <button type="submit">Send Message</button>
  </form>
</section>
```
*Explanation:* Implements semantic input elements (`<input type="text">`, `<input type="email">`, `<select>`, `<textarea>`) with associated `<label>` tags for accessibility.

---

### B. CSS Styling & Box Model (`style.css`)

The stylesheet strictly enforces a **flat, minimalist approach** without any decorative borders or box-shadows, highlighting the core **CSS Box Model** (Content, Padding, and Margin):

#### 1. Universal Reset & Layout Container
```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  width: 85%;
  max-width: 900px;
  margin: 0 auto;
  padding: 20px 0;
}
```
*Explanation:* `box-sizing: border-box` ensures that padding is calculated within element dimensions, preventing unexpected layout overflow. `margin: 0 auto` centers the content container.

#### 2. Section Spacing via Box Model Margins & Padding
```css
section {
  background-color: #ffffff;
  margin-bottom: 25px;
  padding: 30px;
}
```
*Explanation:* `margin-bottom: 25px` establishes clear separation between adjacent sections, while `padding: 30px` creates generous interior breathing room around content.

#### 3. Flat Form Controls (No Borders, No Shadows)
```css
input[type="text"],
input[type="email"],
select,
textarea {
  width: 100%;
  padding: 12px;
  background-color: #f9fafb;
  font-family: inherit;
  font-size: 14px;
  border: none;
  outline: none;
}

input[type="text"]:focus,
input[type="email"]:focus,
select:focus,
textarea:focus {
  background-color: #e5e7eb;
}
```
*Explanation:* Sets `border: none` and relies on subtle background-color shifts (`#f9fafb` to `#e5e7eb`) on `:focus` to signal interactivity cleanly.

---

## 5. UI Output Screenshot

The rendered web page output is shown below:

![Full Page UI Output](ui_output_full.png)

---

## 6. How to Run & Verify

1. **Direct Browser Execution:**
   - Double-click `index.html` or open via browser (`file:///.../index.html`).
2. **Local Server (XAMPP / WAMP):**
   - Copy the folder into `C:\xampp\htdocs\PHP-Class-Assignment-1\`.
   - Start Apache and navigate to `http://localhost/PHP-Class-Assignment-1/index.html`.
3. **Validation:**
   - Open Developer Tools in browser (`F12`) to inspect the DOM tree and verify the CSS Box Model metrics.
