# 📄 Templates Guide (Issue & PR Templates)

This guide explains how to create **Templates** that are used to standardize bug reports (Issues) and code contributions (Pull Requests) submitted to your project. These templates guide contributors to provide the correct information and make project maintenance much more efficient.

## Table of Contents

1.  [What are Templates and Why are They So Important?](#1-what-are-templates-and-why-are-they-so-important)
2.  [How Do They Work? The Role of the `.github` Folder](#2-how-do-they-work-the-role-of-the-github-folder)
3.  [Creating Issue Templates](#3-creating-issue-templates)
4.  [Creating a Pull Request Template](#4-creating-a-pull-request-template)
5.  [Best Usage Practices](#5-best-usage-practices)

-----

## 1\. What are Templates and Why are They So Important?

Issue and Pull Request (PR) templates are pre-prepared Markdown texts that are automatically loaded into the description box when a user starts creating a new issue or PR.

**Main benefits:**

  - **Complete Information:** Encourages users to provide all the essential information needed to understand the problem (version, operating system, steps, etc.). Prevents insufficient reports like "It's not working."
  - **Standardization:** Ensures that all reports and contributions arrive in the same format, making them easier to review and manage.
  - **Time Efficiency:** Saves project maintainers the time spent asking the same basic questions repeatedly.
  - **Process Guidance:** A PR template offers a checklist that reminds contributors of important steps, such as whether they ran tests or updated the documentation.

## 2\. How Do They Work? The Role of the `.github` Folder

GitHub looks for a special folder named `.github` in a project's root directory. When you place files or subfolders with specific names inside this folder, GitHub automatically detects them and activates the corresponding features. Issue and PR templates also live inside this folder.

## 3\. Creating Issue Templates

It is best practice to allow users to choose different templates for different purposes (bug reporting, feature suggesting).

### Folder Structure

Create the following structure in your project's root directory:

```
.github/
└── ISSUE_TEMPLATE/
    ├── bug_report.md
    ├── feature_request.md
    └── config.yml
```

### a. Bug Report Template (`bug_report.md`)

This template asks for all the necessary information to reproduce a bug.

```markdown
---
name: 🐞 Bug Report
about: Use this to report a bug you have found in the project.
title: "[BUG] Write a short and descriptive title"
labels: 'bug'
assignees: ''

---

**Description of the Bug**
Provide a clear and concise explanation of what the bug is.

**Steps to Reproduce**
Explain step-by-step how the bug can be reproduced:
1. Go to the '...' page.
2. Click on the '...' button.
3. Scroll down and see '...'.
4. The bug appears here.

**Expected Behavior**
Clearly state what you expected to happen normally.

**Screenshots**
If possible, include screenshots to help us understand the bug.

**Technical Environment (Please fill out this information):**
 - Operating System: [e.g., Windows 10, macOS Sonoma]
 - Browser (if applicable): [e.g., Chrome, Firefox]
 - Project Version: [e.g., v1.2.3]

**Additional Context**
Is there any other context you would like to add about the problem?
```

### b. Feature Request Template (`feature_request.md`)

This template is used for proposing a new idea or enhancement.

```markdown
---
name: ✨ Feature Request
about: Suggest a new idea or enhancement for the project.
title: "[SUGGESTION] Write a short and descriptive title"
labels: 'enhancement'
assignees: ''

---

**Is your suggestion related to a problem? Please describe.**
For example: Provide an explanation like "I constantly have to perform action X, and it takes too long. I wish feature Y existed..."

**Proposed Solution**
Clearly explain the feature or enhancement you think will solve this problem.

**Alternatives Considered**
Have you thought about any other solutions or features that could solve this problem?

**Additional Context**
Is there any other context, screenshots, or examples you would like to add about your suggestion?
```

### c. Configuration File (`config.yml`)

This file determines which options the user will see when they click the "New issue" button.

```yaml
blank_issues_enabled: false
contact_links:
  - name: 💬 Community Discussions
    url: https://github.com/user/project/discussions
    about: Please use the Discussions section for general questions other than feature proposals or bug reports.
```

## 4\. Creating a Pull Request Template

The PR template helps ensure that contributors perform the necessary checks.

### File Location and Name

Create the following file in your project's root directory: `.github/PULL_REQUEST_TEMPLATE.md`

### Example `PULL_REQUEST_TEMPLATE.md`

```markdown
## 🎯 What is this PR about?
- 
- 
- 

## 🔗 Related Issue
Closes #

## 📸 Screenshots (If Any)
## Checklist:
- [ ] My code adheres to the project's coding standards.
- [ ] I have written and run the necessary tests for my changes.
- [ ] I have updated the relevant documentation.
- [ ] My changes do not create any new warnings.
```

## 5\. Best Usage Practices

  - **Be Clear and Simple:** Ensure the language in your templates is easy to understand and follow.
  - **Specify Required and Optional Fields:** Clarify which information users absolutely must provide.
  - **Provide Direction:** Use `config.yml` to direct users to "Discussions" or other communication channels for general questions.
  - **Keep It Updated:** Don't forget to update your templates as your project's process changes.