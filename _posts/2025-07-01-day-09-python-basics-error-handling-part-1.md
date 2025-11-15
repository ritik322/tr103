---
title: "Day 9: Python Basics - Error Handling (Part 1)"
description: "Introduction to exception handling with try-except blocks to prevent program crashes."
author: ritikmehta
date: 2025-07-01 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, error-handling, exceptions, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 9: July 1, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I learned about **Error Handling**—how to prevent your program from crashing when something goes wrong. This is essential for building robust applications.

### 🧠 Concepts Reviewed

* **What are Exceptions?**
    * **Definition:** Errors that occur during program execution (runtime errors).
    * **Examples:** `ZeroDivisionError`, `FileNotFoundError`, `ValueError`, `KeyError`
    * **Problem:** Without handling, these errors crash your program immediately.

* **The `try...except` Block:**
    * **What it does:** Tries to run code, and if an error occurs, handles it gracefully instead of crashing.
    * **Basic syntax:**
    ```python
    try:
        result = 10 / 0
    except ZeroDivisionError:
        print("Cannot divide by zero!")
    ```

* **Catching Multiple Exceptions:**
    * **Multiple except blocks:**
    ```python
    try:
        file = open('missing.txt', 'r')
    except FileNotFoundError:
        print("File not found!")
    except PermissionError:
        print("No permission to read file!")
    ```

* **Generic Exception Handling:**
    * **Catch any error:**
    ```python
    try:
        # risky code
        pass
    except Exception as e:
        print(f"An error occurred: {e}")
    ```

* **Real-World Example (Jarvis):**
    * In my `takeCommand()` function, I use try-except to handle microphone errors:
    ```python
    try:
        query = recognizer.listen(source)
    except Exception as e:
        print("Could not understand audio")
        return "None"
    ```

### ✅ Today's Goal
The goal was to understand how to prevent crashes by anticipating errors. This is crucial for any real-world application where things can go wrong (missing files, network issues, invalid user input, etc.).