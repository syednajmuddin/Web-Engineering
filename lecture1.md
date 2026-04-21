# 🛠️ Instructor’s Note on AI & Ethics
> **Declaration:** Portions of this material were generated with the assistance of AI (ChatGPT, OpenAI) and curated by the instructor.  
> Students are advised to consult standard references to validate and deepen their understanding.

---

# Lecture 3: Introduction to HTML & Page Structure

---

## Recap of Previous Lecture

- Difference between Internet (infrastructure) and Web (service on top of it)
- Basic client–server model (Client → Request → Server → Response)
- Difference between static and dynamic content
- Real-world analogy (e.g., ready-made vs custom-made service)
- Role of web browsers and web servers

---

## 1. Basic HTML Document Structure

Every webpage follows a standard structure:

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Page</title>
</head>
<body>
    <h1>Welcome</h1>
    <p>This is my webpage.</p>
</body>
</html>
```

### Explanation:

* `<!DOCTYPE html>` → Defines HTML5 document
* `<html>` → Root element
* `<head>` → Metadata (title, meta info)
* `<body>` → Visible content

---

## 2. Basic Content Tags

Common tags used inside `<body>`:

```html
<h1>Main Heading</h1>
<p>This is a paragraph.</p>
```

---

## 3. How Do We Organize a Webpage?

Now consider a real website:

* Where does the header go?
* Where is navigation placed?
* How do we separate content and footer?

A simple (but not ideal) approach is:

```html
<div class="header">Header</div>
<div class="nav">Navigation</div>
<div class="content">Content</div>
<div class="footer">Footer</div>
```

### Problem:

* Everything is just a `<div>`
* No meaning (semantics)
* Harder to understand and maintain

---

## 4. Semantic HTML (Recommended Approach)

Semantic tags describe the *meaning* of content.

```html
<header>Header</header>
<nav>Navigation</nav>
<main>
    <section>Content</section>
</main>
<footer>Footer</footer>
```

### Why use semantic tags?

* Better readability for developers
* Helps search engines (SEO)
* Improves accessibility (screen readers)

---

## 5. Complete Example Using Semantic Tags

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Website</title>
</head>
<body>

  <header>
    <h1>My Website</h1>
  </header>

  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
  </nav>

  <main>
    <section>
      <h2>Welcome</h2>
      <p>This is the main content.</p>
    </section>
  </main>

  <footer>
    <p>© 2026</p>
  </footer>

</body>
</html>
```

---

## 6. Lists in HTML

### Unordered List

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

### Ordered List

```html
<ol>
  <li>First</li>
  <li>Second</li>
</ol>
```

---

## 7. Links in HTML

```html
<a href="https://example.com">Visit Website</a>
```

---

## 8. Images in HTML

```html
<img src="image.jpg" alt="Description" width="200">
```

---

## 9. In-Class Activity

Create a simple webpage that includes:

* A header
* Navigation links
* A main section with heading and paragraph
* A list
* An image
* A footer

---

## 10. Summary

* HTML provides structure to webpages
* Semantic tags improve clarity and organization
* Lists, links, and images enhance content
