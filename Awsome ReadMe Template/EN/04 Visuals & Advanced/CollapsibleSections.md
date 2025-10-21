# 📖 Collapsible Sections Guide

This guide explains how to create **collapsible** sections in your `README` files using the HTML `<details>` and `<summary>` tags to keep them cleaner and more organized. This technique is perfect for hiding secondary information such as long code blocks, configuration file examples, or frequently asked questions by default.

## Table of Contents

1.  [What is a Collapsible Section and Why is it Used?](#1-what-is-a-collapsible-section-and-why-is-it-used)
2.  [Basic Syntax](#2-basic-syntax)
3.  [Nested Collapsible Sections](#3-nested-collapsible-sections)
4.  [Using Markdown as Content](#4-using-markdown-as-content)
5.  [Practical Use Cases](#5-practical-use-cases)
6.  [Best Usage Practices](#6-best-usage-practices)

-----

## 1\. What is a Collapsible Section and Why is it Used?

A collapsible section is an interactive area whose content the user can show or hide by clicking. GitHub allows the use of basic HTML tags within Markdown files, and `<details>` is one of these powerful features.

**Main benefits:**

  - **Clean and Focused Interface:** Makes the `README` file look shorter and less intimidating at first glance. Users only click to see the details they are interested in.
  - **Organization:** Separates long or technically dense information (error outputs, lengthy code examples, etc.) from the main flow.
  - **Enhanced Documentation:** Provides an ideal structure for sections like Frequently Asked Questions (FAQ).

## 2\. Basic Syntax

Two HTML tags are used to create a collapsible section:

  - `<details>`: The main tag that wraps all the content to be hidden.
  - `<summary>`: Contains the title text that is always visible and toggles the content open or closed when clicked.

### Basic Example

```html
<details>
  <summary>Click here to view the details.</summary>

  This section is hidden by default. It becomes visible when the title is clicked.
  You can add as much text or other content as you like here.
</details>
```

### Result:

\<details\>
\<summary\>Click here to view the details.\</summary\>

This section is hidden by default. It becomes visible when the title is clicked.
You can add as much text or other content as you like here.

\</details\>

-----

## 3\. Nested Collapsible Sections

You can nest `<details>` tags to create more complex and hierarchical structures.

### Nested Example

```html
<details>
  <summary>Main Topic</summary>

  This is the explanation for the main topic.

  <details>
    <summary>Sub Topic 1</summary>

    These are the details for the sub topic.
  </details>

  <details>
    <summary>Sub Topic 2</summary>
    
    These are the details for the second sub topic.
  </details>
</details>
```

### Result:

\<details\>
\<summary\>Main Topic\</summary\>

This is the explanation for the main topic.

\<details\>
\<summary\>Sub Topic 1\</summary\>

```
These are the details for the sub topic.
```

\</details\>

\<details\>
\<summary\>Sub Topic 2\</summary\>

```
These are the details for the second sub topic.
```

\</details\>
\</details\>

-----

## 4\. Using Markdown as Content

One of the most powerful features of the `<details>` tag is that you can write normal Markdown syntax inside it. All Markdown elements such as code blocks, lists, images, and tables work seamlessly.

**Important Note:** For Markdown to be rendered correctly, you must **leave a blank line** after the `<summary>` tag and before the `</details>` tag.

### Example with Markdown

````html
<details>
  <summary>🚀 Show Installation Commands</summary>

  Below are the basic commands required for project setup:

  ```shell
  # 1. Clone the repository
  git clone [https://github.com/user/project.git](https://github.com/user/project.git)

  # 2. Go to the directory
  cd project

  # 3. Install dependencies
  npm install
  ```

  For more information, please see the `INSTALL.md` file.

</details>
````

### Result:

\<details\>
\<summary\>🚀 Show Installation Commands\</summary\>

Below are the basic commands required for project setup:

```shell
# 1. Clone the repository
git clone https://github.com/user/project.git

# 2. Go to the directory
cd project

# 3. Install dependencies
npm install
```

For more information, please see the `INSTALL.md` file.

\</details\>

-----

## 5\. Practical Use Cases

  - **Frequently Asked Questions (FAQ):** Each question can be a `<summary>`, and each answer can be placed inside `<details>`.
  - **Long Code Blocks:** Hiding long code or configuration file examples that the user does not need to see at first glance.
  - **Error Logs:** In an "Issue" report, putting long error logs inside a collapsible section to make the report more readable.
  - **Release Notes:** Presenting the details of each release within a separate collapsible section.

-----

## 6\. Best Usage Practices

  - **The Space Rule:** Remember to leave a blank line after the `<summary>` tag and before the `</details>` tag for Markdown to work correctly.
  - **Descriptive Titles:** The `<summary>` text should clearly explain what the hidden content is about. Use a more specific title like "View Configuration File Example" instead of a generic phrase like "Details."
  - **Don't Hide Critical Information:** Avoid hiding information vital to the project's setup or basic usage by default. This feature is better suited for secondary or optional information.