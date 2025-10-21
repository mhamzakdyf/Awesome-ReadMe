# ✅ Task Lists in Markdown

This guide explains all the details of creating interactive task lists using GitHub Flavored Markdown (GFM). Task lists are an excellent tool for tracking tasks to be done (To-Do List), the progress of a project, or whether a set of requirements has been completed.

## Table of Contents

1.  [What is a Task List?](#1-what-is-a-task-list)
2.  [Basic Syntax Rules](#2-basic-syntax-rules)
3.  [Practical Use Cases](#3-practical-use-cases)

-----

## 1\. What is a Task List?

A task list is a special Markdown list where each item has a clickable checkbox. On GitHub, these lists are more than static text; you can update the status of tasks by checking the boxes directly via the `README` file, `Issue`, or `Pull Request` description.

## 2\. Basic Syntax Rules

Creating a task list is very simple. It is sufficient to add `[ ]` (incomplete) or `[x]` (complete) at the beginning of each item in a standard unordered list (starting with `-`, `*`, or `+`).

### Incomplete Task

Leave a space between the square brackets for an empty checkbox.

```markdown
- [ ] Bu görev henüz tamamlanmadı.
* [ ] Bu da tamamlanmadı.
```

**Result:**

  - [ ] This task is not completed yet.
  - [ ] This one is not completed either.

### Completed Task

Write a lowercase `x` between the square brackets for a completed task.

```markdown
- [x] Bu görev tamamlandı.
* [x] Bu görev de başarıyla bitti.
```

**Result:**

  - [x] This task has been completed.
  - [x] This task was also successfully finished.

## 3\. Practical Use Cases

  - **Project Roadmap:** In your `README.md` file, you can present the features planned for future versions of the project as a task list.
  - **Pull Request (PR) Templates:** When a PR is opened, you can add the steps a developer must complete (running tests, updating documentation, etc.) to the template as a task list. This increases code quality.
  - **Issue Tracking:** When a bug or feature request (`Issue`) is created, you can specify the steps required for a solution as a task list.
  - **Personal Notes:** You can easily keep your own `TODO` list in a Markdown file.