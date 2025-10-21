Elbette, metnin Markdown yapısını bozmadan ve İçindekiler'deki bağlantıları kaldırarak İngilizce'ye çevirisi aşağıdadır:

# 📊 Tables Guide

This guide details how to create and format **Markdown tables**, which are used to present data in a structured and organized manner. Tables are an excellent tool for situations like comparing features, listing API parameters, or showcasing configuration options.

## Table of Contents

1.  [Why Are Tables Useful?](#1-why-are-tables-useful)
2.  [Creating a Basic Table (Syntax)](#2-creating-a-basic-table-syntax)
3.  [Column Alignment](#3-column-alignment)
4.  [Formatting within Tables](#4-formatting-within-tables)
5.  [Best Usage Practices](#5-best-usage-practices)

-----

## 1\. Why Are Tables Useful?

Tables come into play where lists or normal texts are insufficient. Their main benefits include:

  - **Comparison:** Allows easy side-by-side comparison of features of different items.
  - **Structured Data:** Ideal for presenting "key-value" pairs such as parameters, options, and definitions.
  - **Readability:** Separates information into rows and columns, making it easy to scan and understand.
  - **Professional Look:** Adds an organized and professional feel to technical documentation.

## 2\. Creating a Basic Table (Syntax)

The basic logic of creating a table in Markdown is quite simple and consists of three main components:

1.  **Header Row:** Contains the column titles. Cells are separated by vertical bars (`|`).
2.  **Delimiter Row:** Separates the headers from the rest of the table. At least three hyphens (`---`) are used for each column.
3.  **Content Rows:** Contains the table data. Cells are again separated by `|`.

### Basic Example

```markdown
| Header 1 | Header 2 | Header 3 |
|---|---|---|
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| Row 3, Column 1 | Row 3, Column 2 | Row 3, Column 3 |
```

### Result:

| Header 1 | Header 2 | Header 3 |
|---|---|---|
| Row 1, Column 1 | Row 1, Column 2 | Row 1, Column 3 |
| Row 2, Column 1 | Row 2, Column 2 | Row 2, Column 3 |
| Row 3, Column 1 | Row 3, Column 2 | Row 3, Column 3 |

-----

## 3\. Column Alignment

You can add colons (`:`) to the delimiter row to align the text in the table columns to the left, right, or center.

  - **Left Align (Default):** `:---`
  - **Center:** `:---:`
  - **Right Align:** `---:`

### Alignment Example

```markdown
| Command | Description | Required? |
|:---|:---:|---:|
| `git clone` | Copies the project to your computer. | Yes |
| `npm install` | Installs the necessary packages. | Yes |
| `npm test` | Runs the tests. | No |
```

### Result:

| Command | Description | Required? |
|:---|:---:|---:|
| `git clone` | Copies the project to your computer. | Yes |
| `npm install` | Installs the necessary packages. | Yes |
| `npm test` | Runs the tests. | No |

-----

## 4\. Formatting within Tables

You can include other Markdown elements inside table cells. This makes your tables richer and more informative.

  - Inline code (`` ` ``)
  - Links (`[]()`)
  - Bold or italic text (`**bold**`, `*italic*`)
  - Strikethrough text (`~~strikethrough~~`)

### Formatting Example

```markdown
| Parameter | Type | Description |
|---|---|---|
| `userId` | *string* | The **unique** ID of the user whose information will be retrieved. |
| `isActive` | *boolean* | Used to list only active users. |
| `apiKey` | `string` | ~~No longer used.~~ Use a token instead. |
| `docs` | [Link](https://...) | Related documentation page. |
```

### Result:

| Parameter | Type | Description |
|---|---|---|
| `userId` | *string* | The **unique** ID of the user whose information will be retrieved. |
| `isActive` | *boolean* | Used to list only active users. |
| `apiKey` | `string` | \~\~No longer used.\~\~ Use a token instead. |
| `docs` | [Link](https://www.google.com/search?q=https://...) | Related documentation page. |

-----

## 5\. Best Usage Practices

  - **Make Raw Code Readable:** To make the table look neat even when editing the Markdown file, aligning the vertical bars (`|`) below each other is a good practice. This doesn't affect the rendered result but increases the readability of the source code.
  - **Keep Tables Simple:** Wide tables with too many columns might not look good on mobile devices. Keep your tables narrow and focused if possible.
  - **Empty Cells:** If you want to leave a cell empty, just leave the space between the vertical bars (`|`) blank.
  - **Avoid Unnecessary Use:** There is no need to turn something that can be explained with a simple list into a table. Use tables only for structural data.