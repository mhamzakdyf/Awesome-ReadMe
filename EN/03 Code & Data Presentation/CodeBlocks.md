Elbette, metnin Markdown yapısını bozmadan ve İçindekiler'deki bağlantıları kaldırarak İngilizce'ye çevirisi aşağıdadır:

# 💻 Code Blocks Guide

This guide details how to create **Code Blocks** and **Inline Code**, the most fundamental components of technical `README` files. These tools maximize readability and clarity by separating code snippets, commands, and technical terms from the normal text.

## Table of Contents

1.  [Why is Code Display Important?](#1-why-is-code-display-important)
2.  [Inline Code](#2-inline-code)
3.  [Code Blocks (Fenced Code Blocks)](#3-code-blocks-fenced-code-blocks)
4.  [Syntax Highlighting](#4-syntax-highlighting)
5.  [Best Usage Practices](#5-best-usage-practices)

-----

## 1\. Why is Code Display Important?

In a technical document, separating commands or code from normal text is vital. Code display:

  - **Provides Readability:** Formats the code with a special font and background, separating it from the rest of the text.
  - **Facilitates Copying:** Platforms like GitHub add a one-click copy button to the corner of code blocks.
  - **Preserves Meaning:** Maintains the indentations, spaces, and special characters within the code exactly as they are.
  - **Prevents Errors:** Stops a user from mistyping or incompletely copying a command.

## 2\. Inline Code

Used to denote expressions within a sentence such as a single command, variable name, file path, function name, or a short code snippet.

### Basic Syntax

You simply need to enclose the text within **single backticks** (`` ` ``). This character is usually located below the `Esc` key on the keyboard.

```markdown
Run the `npm install` command for the project to work. The main configuration file is named `.env`. The `getUser()` function retrieves user information.
```

### Result:

Run the `npm install` command for the project to work. The main configuration file is named `.env`. The `getUser()` function retrieves user information.

## 3\. Code Blocks (Fenced Code Blocks)

Used for long code snippets consisting of multiple lines, configuration file examples, or command line outputs.

### Basic Syntax

You must enclose your code between lines of **triple backticks** (`` ` `` \`).

````markdown
```
This is a code block.
All lines and spaces here
are preserved.
```
````

### Result:

```
This is a code block.
All lines and spaces here
are preserved.
```

## 4\. Syntax Highlighting

The most powerful feature of code blocks is the ability to color the code according to the programming language it is written in. This dramatically increases the code's readability.

To do this, you simply specify the name of the language in lowercase immediately after the initial triple backticks.

### JavaScript Example

````markdown
```javascript
function sayHello(name) {
  console.log(`Hello, ${name}!`);
}

sayHello('World');
```
````

**Result:**

```javascript
function sayHello(name) {
  console.log(`Hello, ${name}!`);
}

sayHello('World');
```

### Python Example

````markdown
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5))
```
````

**Result:**

```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)

print(factorial(5))
```

### Command Line Example (`shell` or `bash`)

Using `shell` or `bash` to show terminal commands is a standard practice. This indicates that the lines are runnable commands.

````markdown
```shell
# Clone the project
git clone [https://github.com/user/repo.git](https://github.com/user/repo.git)

# Change to the directory
cd repo

# Install dependencies
npm install
```
````

**Result:**

```shell
# Clone the project
git clone https://github.com/user/repo.git

# Change to the directory
cd repo

# Install dependencies
npm install
```

## 5\. Best Usage Practices

  - **Specify the Correct Language:** Always use the correct language identifier (`javascript`, `python`, `java`, `csharp`, `html`, `css`, etc.) for the readability of your code.
  - **Be Concise:** In code blocks, only show the code snippet necessary to illustrate the topic. Avoid pasting hundreds of lines of code.
  - **Add Context:** Before or after the code block, include a short text explaining what this code does and why it is important. Provide context to the user.
  - **Avoid Specifying Language (If Plaintext):** If you only want to format simple text or a command output, you can use a code block without specifying a language. This is treated as `plaintext`.