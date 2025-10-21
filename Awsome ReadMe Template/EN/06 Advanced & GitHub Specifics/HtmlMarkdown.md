# 🌐 HTML in Markdown Guide

This guide explains how to use **HTML tags** within your Markdown documents to add more control and style when standard Markdown falls short. GitHub's Markdown renderer supports most basic HTML tags, which allows you to size images, align text more precisely, and create advanced structures.

## Table of Contents

1.  [Why Use HTML Within Markdown?](#1-why-use-html-within-markdown)
2.  [Basic Text Formatting](#2-basic-text-formatting)
3.  [Advanced Image Control](#3-advanced-image-control)
4.  [Collapsible Sections (Details and Summary)](#4-collapsible-sections-details-and-summary)
5.  [Displaying Keyboard Shortcuts](#5-displaying-keyboard-shortcuts)
6.  [Combining Markdown with HTML](#6-combining-markdown-with-html)
7.  [Best Usage Practices and Limitations](#7-best-usage-practices-and-limitations)

-----

## 1\. Why Use HTML Within Markdown?

Markdown is known for its simplicity and readability. However, sometimes you need more:

  - **Sizing and Alignment:** Centering an image or adjusting its size.
  - **Fine-Tuning Formatting:** Creating underlined text or adding a mandatory line break.
  - **Interactive Elements:** Creating collapsible menus, such as with the `details` tag.
  - **Custom Structures:** More complex structures that standard Markdown doesn't support.

In such cases, you can write HTML code directly inside your Markdown file.

## 2\. Basic Text Formatting

You can use HTML for some basic text styles that are not available in standard Markdown.

### Underlined Text (`<u>`)

```html
This is <u>underlined</u> text.
```

**Result:** This \<u\>underlined\</u\> text.

### Line Break (`<br>`)

In Markdown, you usually need to leave a blank line to start a new paragraph. However, sometimes you want the text to continue immediately on the next line. The `<br>` tag does exactly that.

```markdown
This is the first line.<br>This is the line immediately below it.
```

**Result:**
This is the first line.<br>This is the line immediately below it.

## 3\. Advanced Image Control

This is one of the most common areas where HTML is used. The standard Markdown `![alt](src)` syntax does not allow you to control image size or alignment.

### Image Sizing

You can set the image's `width` and/or `height` properties in pixels using the `<img>` tag.

```html
<img src="./assets/logo.png" alt="Project Logo" width="100">
```

### Image Alignment

You can wrap an image inside a `<p>` or `<div>` tag with the `align` attribute to center or right-justify it.

**Centered Image:**

```html
<p align="center">
  <img src="./assets/logo.png" alt="Project Logo" width="200">
</p>
```

**Right-Justified Image:**

```html
<p align="right">
  <img src="./assets/logo.png" alt="Project Logo" width="100">
</p>
```

## 4\. Collapsible Sections (Details and Summary)

As mentioned in the previous guide, the `<details>` and `<summary>` tags are the best way to add interactive, expandable/collapsible sections to your `README` files.

```html
<details>
  <summary>🚀 Advanced Installation Steps</summary>

  You can add detailed installation steps or code blocks that are normally hidden here.
</details>
```

## 5\. Displaying Keyboard Shortcuts

The `<kbd>` (keyboard) tag is excellent for indicating keyboard shortcuts in your documentation. Browsers usually style this tag with a special font that looks like a key.

```html
Use the <kbd>Ctrl</kbd> + <kbd>S</kbd> key combination to save the file.
```

**Result:**
Use the \<kbd\>Ctrl\</kbd\> + \<kbd\>S\</kbd\> key combination to save the file.

## 6\. Combining Markdown with HTML

The content inside HTML tags can often still be interpreted as Markdown. To do this, you must leave a blank line after the opening and before the closing tags of your HTML block.

```html
<p align="center">
  
  _This text is both centered and **italic and bold**._

  `This is also a code snippet.`

</p>
```

**Result:**

\<p align="center"\>

*This text is both centered and **italic and bold**.*

`This is also a code snippet.`

\</p\>

## 7\. Best Usage Practices and Limitations

  - **Avoid Unnecessary Use:** If you can do something with standard Markdown, prefer it. HTML can reduce readability. Use HTML only where Markdown's capabilities end.
  - **Security Limitations:** GitHub blocks HTML tags and features that could be dangerous for security reasons (e.g., `<script>`, `<iframe>`, `style`). You can only use basic formatting and structural tags.
  - **Compatibility:** Be aware that the HTML you write may not render the same way in different Markdown renderers (e.g., another Git platform or static site generator).
  - **Readability:** Complex HTML structures can make the raw `.md` file difficult to read. Keep your code clean and organized.