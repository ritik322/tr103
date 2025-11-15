---
title: "Day 8: Python Basics - File Handling (Part 2)"
description: "Advanced file handling with context managers and best practices for safe file operations."
author: ritikmehta
date: 2025-06-30 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, file-handling, context-manager, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 8: June 30, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I learned the **proper way** to handle files using context managers and best practices. This makes file operations safer and prevents common errors.

### 🧠 Concepts Reviewed

* **The `with` Statement (Context Manager):**
    * **What it is:** A better way to open files that automatically closes them, even if an error occurs.
    * **Syntax:**
    ```python
    with open('file.txt', 'r') as file:
        content = file.read()
        print(content)
    # File is automatically closed here
    ```
    * **Why it's better:** No need to manually call `file.close()`, and it handles errors gracefully.

* **Working with Multiple Files:**
    * **Example:** Reading from one file and writing to another:
    ```python
    with open('input.txt', 'r') as infile:
        with open('output.txt', 'w') as outfile:
            content = infile.read()
            outfile.write(content.upper())
    ```

* **File Paths:**
    * **Relative paths:** `'data.txt'` (in the same folder)
    * **Absolute paths:** `'C:/Users/Ritik/data.txt'` (full path)
    * **Cross-platform:** Use `os.path.join()` for compatibility between Windows/Mac/Linux

* **Checking if Files Exist:**
    * **Using `os` module:**
    ```python
    import os
    if os.path.exists('file.txt'):
        print("File exists!")
    ```

* **Appending to Files:**
    * **Mode `'a'`:** Adds content to the end without erasing existing data.
    ```python
    with open('log.txt', 'a') as file:
        file.write("New log entry\n")
    ```

### ✅ Today's Goal
The goal was to master safe and efficient file handling. This is directly applicable to my Jarvis project, where I read and write to `Remember.txt` to store user information across sessions.