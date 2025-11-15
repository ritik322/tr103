---
title: "Day 10: Python Basics - Error Handling (Part 2)"
description: "Advanced error handling with else, finally, and raising custom exceptions."
author: ritikmehta
date: 2025-07-02 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, error-handling, exceptions, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 10: July 2, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I completed my error handling review by learning advanced techniques: `else`, `finally`, and how to raise your own exceptions. This marks the **end of Phase 1**!

### 🧠 Concepts Reviewed

* **The `else` Clause:**
    * **What it does:** Runs only if no exception occurred in the `try` block.
    * **Example:**
    ```python
    try:
        number = int(input("Enter a number: "))
    except ValueError:
        print("That's not a valid number!")
    else:
        print(f"You entered: {number}")
    ```

* **The `finally` Clause:**
    * **What it does:** Always executes, whether an exception occurred or not.
    * **Use case:** Cleanup operations like closing files or database connections.
    * **Example:**
    ```python
    try:
        file = open('data.txt', 'r')
        content = file.read()
    except FileNotFoundError:
        print("File not found!")
    finally:
        file.close()  # Always closes the file
    ```

* **Raising Exceptions:**
    * **What it means:** Intentionally triggering an exception when something is wrong.
    * **Syntax:** `raise ExceptionType("Error message")`
    * **Example:**
    ```python
    def divide(a, b):
        if b == 0:
            raise ValueError("Cannot divide by zero!")
        return a / b
    ```

* **Custom Exceptions:**
    * **What they are:** Your own exception types for specific error cases.
    * **Example:**
    ```python
    class InvalidAgeError(Exception):
        pass
    
    age = -5
    if age < 0:
        raise InvalidAgeError("Age cannot be negative!")
    ```

### ✅ Phase 1 Complete!
Today marks the completion of **Phase 1: Python Basics Review**. I've covered:
- Data structures (lists, dicts, tuples, sets)
- Functions and modules
- File handling
- Error handling

I'm now 100% confident in my Python fundamentals. Tomorrow, I move to **Phase 2: The "AI" Libraries** where I'll learn about NumPy, Pandas, and OpenCV!