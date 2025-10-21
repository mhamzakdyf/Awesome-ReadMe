# 🔗 Links Guide

This guide details how to create **links** that make your Markdown documents interactive and connect different sources of information. Links are the primary way to direct users to external websites, different sections of the document, or other files in your repository.

## Table of Contents

1.  [What is a Link and Why is it Important?](#1-what-is-a-link-and-why-is-it-important)
2.  [External Links](#2-external-links)
3.  [Internal (Anchor) Links](#3-internal-anchor-links)
4.  [Relative Links](#4-relative-links)
5.  [Advanced Link Techniques](#5-advanced-link-techniques)
6.  [Best Usage Practices](#6-best-usage-practices)

-----

## 1\. What is a Link and Why is it Important?

A link (or hyper link) is a piece of text or an image that, when clicked, takes you to another destination. In `README` files, links are used for the following purposes:

  - **Citations/References:** Linking to the website of a library, tool, or article being used.
  - **Navigation:** Allowing users to easily navigate between different sections of the document (like a Table of Contents).
  - **Related Files:** Directing users to other important files in the project (`CONTRIBUTING.md`, `LICENSE`, etc.).
  - **Interaction:** Linking to demo sites, contact addresses, or social media profiles.

## 2\. External Links

External links direct you to a website outside of the current document.

### Basic Syntax

The structure `[Display Text](URL)` is used to create a link.

  - `[Display Text]`: This is the text the user will see and click on.
  - `(URL)`: This is the web address that will be visited when clicked.

<!-- end list -->

```markdown
Our project uses the [Google](https://www.google.com) search engine.
For more information, you can visit the [Markdown Guide](https://www.markdownguide.org).
```

### Result:

Our project uses the [Google](https://www.google.com) search engine.
For more information, you can visit the [Markdown Guide](https://www.markdownguide.org).

### Adding a Title

If you want a small description box (tooltip) to appear when hovering over the link, you can add a title in quotes after the URL.

```markdown
[GitHub](https://github.com "Goes to GitHub's homepage")
```

**Result:** [GitHub](https://github.com "Goes to GitHub's homepage") (Hover your mouse over it)

-----

## 3\. Internal (Anchor) Links

Internal links (anchor links) direct the user to a different heading within the same document. They are vital for facilitating navigation in long documents, especially when creating a **Table of Contents**.

### Syntax

The structure `[Display Text](#link-version-of-the-target-heading)` is used. The `#` sign indicates that the link is within the same page.

GitHub automatically generates a link version from your headings. The rules are:

1.  All letters are converted to lowercase.
2.  Spaces are replaced with hyphens (`-`).
3.  Emojis and special characters (`?`, `!`, `.` etc.) are removed.

**Example:**
To link to the heading `## 5. Advanced Link Techniques`:

```markdown
[Go to advanced techniques](#5-advanced-link-techniques)
```

**Result:** [Go to advanced techniques](#5-advanced-link-techniques)

-----

## 4\. Relative Links

Relative links are used to link to other files within your project (repository). This keeps your project self-contained and ensures the links work regardless of where your project is copied.

### Link to a File in the Same Directory

```markdown
Please read the [`CONTRIBUTING.md`](./CONTRIBUTING.md) file for contribution rules.
```

### Link to a File in a Different Directory

```markdown
Installation instructions are located in the [`docs/INSTALL.md`](./docs/INSTALL.md) file.
```

-----

## 5\. Advanced Link Techniques

### Image Links

To make an image a clickable link, simply nest a standard image definition (`![Alt Text](image-url)`) inside a link definition.

```markdown
[![Google Logo](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)](https://google.com)
```

**Result:** (You can click on the image below)

[](https://www.google.com/search?q=%5Bhttps://google.com%5D\(https://google.com\))

### Email Links (Mailto Links)

`mailto:` is used to create a link that opens the user's default email application.

```markdown
For questions, [email us](mailto:example@mail.com).
```

**Result:** For questions, [email us](mailto:example@mail.com).

-----

## 6\. Best Usage Practices

  - **Be Descriptive:** The link text should clearly indicate where the link goes. Avoid vague phrases like "Click here."
      - **Bad:** For details, click \<u\>here\</u\>.
      - **Good:** For details, read \<u\>our installation guide\</u\>.
  - **Short and Clear:** Keep links as short and understandable as possible.
  - **Check:** Before publishing your document, ensure all links are working correctly. Broken links create an unprofessional impression.