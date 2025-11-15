---
title: "Day 7: Python Basics - File Handling (Part 1)"
description: "Learning how to read from and write to text files in Python, essential for data persistence."
author: ritikmehta
date: 2025-06-28 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, file-handling, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 7: June 28, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I started learning about **File Handling**—how to read from and write to files. This is crucial because most real-world programs need to save and load data from files.

### 🧠 Concepts Reviewed

* **Why File Handling Matters:**
    * Programs need to store data permanently (beyond the program's runtime).
    * **Example in Jarvis:** My `Remember.txt` file stores information that Jarvis needs to remember between sessions.

* **Opening Files:**
    * **Syntax:** `file = open('filename.txt', 'mode')`
    * **Modes:**
        * `'r'` → Read (default)
        * `'w'` → Write (overwrites existing content)
        * `'a'` → Append (adds to existing content)
        * `'r+'` → Read and write

* **Reading from Files:**
    * **Read entire file:** `content = file.read()`
    * **Read line by line:** `line = file.readline()`
    * **Read all lines as list:** `lines = file.readlines()`
    * **Example:**
    ```python
    file = open('data.txt', 'r')
    content = file.read()
    print(content)
    file.close()
    ```

* **Writing to Files:**
    * **Write text:** `file.write("Hello, World!")`
    * **Example:**
    ```python
    file = open('output.txt', 'w')
    file.write("This is a test.")
    file.close()
    ```

* **Closing Files:**
    * **Important:** Always close files with `file.close()` to free up system resources.

### ✅ Today's Goal
The goal was to understand the basics of file I/O operations. Tomorrow, I'll learn the safer `with` statement and how to handle file errors properly.