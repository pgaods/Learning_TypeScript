# HTML Tags Tutorial: A Beginner's Guide

## Overview

HTML (HyperText Markup Language) provides a set of tags that define the structure and content of web pages. This tutorial covers the most commonly used HTML tags, organized by category to help you understand when and how to use each one.

## Learning Objectives

By the end of this tutorial, you will:

- understand the purpose of structural and layout tags
- learn how to format text with semantic and visual tags
- know how to create lists and tables
- be able to embed links and media in your pages

---

## 1. Structural & Layout Tags

Layout tags define the overall structure of your web page. They help organize content into logical sections.

### Block-level vs. Inline Elements

**Block-level elements** take up the full width available and create line breaks before and after.
**Inline elements** only take up as much width as necessary and stay on the same line.

### Key Tags

| Tag | Purpose | Type |
| --- | --- | --- |
| `<div>` | Generic container for grouping content | Block |
| `<span>` | Generic container for small pieces of content | Inline |
| `<section>` | Defines a thematic grouping of content | Block |
| `<article>` | Self-contained content (blog post, news article) | Block |
| `<header>` | Introductory content or navigation | Block |
| `<footer>` | Footer content for a section or page | Block |
| `<nav>` | Navigation links section | Block |
| `<main>` | Main content of the page | Block |

### Example

```html
<header>
  <h1>My Website</h1>
  <nav>
    <a href="/">Home</a>
    <a href="/about">About</a>
  </nav>
</header>

<main>
  <article>
    <h2>Welcome</h2>
    <p>This is my first blog post.</p>
  </article>
</main>

<footer>
  <p>&copy; 2024 My Website</p>
</footer>
```

### Key Differences Between `<div>` and `<span>`

The main difference between `<div>` and `<span>`:

- `<div>` is **block-level** — takes full width and creates line breaks
- `<span>` is **inline** — takes only needed width and stays on the same line

---

## 2. Text Formatting Tags

Use these tags to structure and format your text content.

### Headings

```html
<h1>Main Heading (Largest)</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
<!-- ... through h6 for smallest -->
```

**Best Practice:** Use only one `<h1>` per page for SEO.

### Paragraphs and Text Formatting

Let's see the details using a table:

| Tag | Purpose | Example |
| --- | --- | --- |
| `<p>` | Paragraph text | `<p>This is a paragraph.</p>` |
| `<strong>` | Important text (bold + semantic) | `<strong>Warning:</strong> This is important!` |
| `<em>` | Emphasized text (italic + semantic) | `<em>This is emphasized.</em>` |
| `<b>` | Bold text (visual only) | `<b>Bold text</b>` |
| `<i>` | Italic text (visual only) | `<i>Italic text</i>` |
| `<br>` | Line break | `Line 1<br>Line 2` |

### When to Use Strong vs. Bold / Em vs. Italic

- Use `<strong>` and `<em>` when the emphasis has semantic meaning (screen readers recognize it)
- Use `<b>` and `<i>` for visual formatting without semantic meaning

---

## 3. Lists

Lists organize information in an easy-to-read format.

### Unordered Lists (Bulleted)

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

### Ordered Lists (Numbered)

```html
<ol>
  <li>First step</li>
  <li>Second step</li>
  <li>Third step</li>
</ol>
```

**Remember:** Every list item must be wrapped in `<li>` tags.

---

## 4. Links & Media

These tags allow you to connect to other pages and embed multimedia content.

### Links

```html
<a href="https://example.com">Click here to visit example.com</a>
<a href="/about">Go to About page</a>
```

**Note:** Use relative paths (`/about`) for internal pages and absolute URLs (`https://`) for external links.

### Images

```html
<img src="image.jpg" alt="Description of image">
```

**Important:** Always include `alt` text for accessibility!

### Media

```html
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support the audio tag.
</audio>
```

---

## 5. Tables

Tables display data in rows and columns.

### Basic Table Structure

```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>John</td>
    <td>25</td>
  </tr>
  <tr>
    <td>Sarah</td>
    <td>28</td>
  </tr>
</table>
```

### Components

| Tag | Purpose |
| --- | --- |
| `<table>` | Container for the entire table |
| `<tr>` | Table row |
| `<th>` | Table header cell (bold, centered) |
| `<td>` | Table data cell |

**Tip:** Use `<th>` for headers and `<td>` for data to improve accessibility.

---

## Quick Reference Cheat Sheet

| Task | Tag |
| --- | --- |
| Create a section | `<section>` |
| Add a heading | `<h1>` - `<h6>` |
| Make text bold | `<strong>` or `<b>` |
| Make text italic | `<em>` or `<i>` |
| Create a bullet list | `<ul><li>Item</li></ul>` |
| Create a numbered list | `<ol><li>Item</li></ol>` |
| Add a link | `<a href="url">Text</a>` |
| Add an image | `<img src="file.jpg" alt="description">` |
| Create a table | `<table><tr><th>Header</th></tr><tr><td>Data</td></tr></table>` |

---

## Key Takeaways

1. **Semantic HTML** — Use tags like `<header>`, `<nav>`, `<article>` for meaningful structure
2. **Block vs. Inline** — Understand how `<div>` and `<span>` differ
3. **Accessibility** — Always include `alt` text for images and use semantic tags
4. **Proper Nesting** — Ensure all tags are properly opened and closed
5. **Consistency** — Choose `<strong>`/`<em>` OR `<b>`/`<i>` and stick with it for consistency
