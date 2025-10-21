# ⚖️ Licensing Guide (`LICENSE`)

This guide explains why the **LICENSE** file, the most fundamental legal document of an open-source project, is so important, what popular license types mean, and how to add a license to your project.

## Table of Contents

1.  [What is a License and Why Must It Be Included?](#1-what-is-a-license-and-why-must-it-be-included)
2.  [What Happens If There Is No License?](#2-what-happens-if-there-is-no-license)
3.  [Popular Open Source Licenses](#3-popular-open-source-licenses)
4.  [Which License Should I Choose?](#4-which-license-should-i-choose)
5.  [How to Add a License to the Project?](#5-how-to-add-a-license-to-the-project)

-----

## 1\. What is a License and Why Must It Be Included?

A software license is a legal document that informs others what they can and cannot do with your code, as the person publishing the source code of your project. A license provides clear rules to users on:

  - **Usage:** Can they use your code in their own projects?
  - **Modification:** Can they modify your code?
  - **Distribution:** Can they distribute original or modified versions of your code to others?
  - **Commercial Use:** Can they use your code within a commercial product?
  - **Liability:** Who is responsible if your code contains a bug.

In short, a license provides legal protection for your project and clearly defines the rights of both you and your users.

## 2\. What Happens If There Is No License?

**This is the most critical point:** If your project does not have a `LICENSE` file, default copyright laws apply. This means:

> **You retain all rights to your code, and no one has permission to use, copy, modify, or distribute your code.**

In other words, if you don't add a license, your project is not "open source." People can see your code, but they cannot legally use it. Therefore, choosing an open-source license is **mandatory** if you want others to use and contribute to your project.

## 3\. Popular Open Source Licenses

Licenses are generally divided into "permissive" and "copyleft." Here are simple explanations of the three most popular licenses:

### a. MIT License (Highly Permissive)

This is one of the simplest and most popular licenses.

  - **What can they do?:** They can do almost anything with your code (use, copy, modify, merge, publish, distribute, sublicense, and/or sell).
  - **What is the Only Condition?:** They must include your original copyright notice and the license text everywhere they use your code.
  - **Feature:** They can take your code and use it in a closed-source (commercial) project.

**Who uses it?** Projects like React, Angular, .NET, Node.js.

### b. Apache 2.0 License (Permissive and Patent Protected)

Similar to MIT, it is permissive but more detailed and provides additional protections.

  - **What can they do?:** They can do almost everything, similar to MIT.
  - **What are the Conditions?:**
    1.  They must include the original copyright and license text.
    2.  They must clearly indicate if they made a significant change to the code.
    3.  **Patent Rights:** This license grants users a license to use the patent rights of the contributors, which means additional legal protection for companies.

**Who uses it?** Large projects like Android, Swift, Kubernetes, TensorFlow.

### c. GNU GPLv3 License (Strong Copyleft)

This license reflects the "Free Software" philosophy in the strongest way.

  - **What can they do?:** They can use, modify, and distribute the code.
  - **What is the Most Important Condition?:** If they modify your code, create new software, and distribute that software, they **must also open source the source code of the new software under the same GPLv3 license.** This is called "copyleft" or "viral license."
  - **Feature:** This license guarantees that your code and all derived works will always remain open source.

**Who uses it?** Projects like Linux Kernel (GPLv2), Git, GIMP, WordPress.

## 4\. Which License Should I Choose?

  - If you say, **"People can do whatever they want with my code, as long as they credit me,"** → **MIT License**
  - If you say, **"People can do whatever they want with my code, but I also want patent protection for big companies,"** → **Apache 2.0 License**
  - If you say, **"Everyone who uses my code must also open source their own project. Freedom multiplies when shared,"** → **GNU GPLv3 License**

If you need help, GitHub's **[choosealicense.com](https://choosealicense.com/)** website will help you choose the right license step-by-step.

## 5\. How to Add a License to the Project?

GitHub has made this process very easy:

1.  Go to your project's main page.
2.  Click on the **`Add file`** button and select the **`Create new file`** option.
3.  Type `LICENSE` or `LICENSE.md` in capital letters in the file name field.
4.  A **`Choose a license template`** button will appear on the right side of the file name field. Click this button.
5.  On the page that opens, select the desired license (MIT, Apache 2.0, GPLv3, etc.) from the list on the left.
6.  GitHub will automatically fill out the license text for you. You usually only need to check the `[year]` and `[fullname]` fields.
7.  Click the **`Review and submit`** button and then `commit` the changes.

That's it! Your project now has a legal framework and is officially open source.