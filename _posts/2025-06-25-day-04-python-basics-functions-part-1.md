---
title: "Day 4: Python Basics - Functions (Part 1)"
description: "Understanding how to write and use functions in Python, the building blocks of organized code."
author: ritikmehta
date: 2025-06-25 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, functions, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 4: June 25, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I moved into **Functions**—one of the most important concepts in programming. Functions allow you to write reusable pieces of code that make your programs cleaner and more organized.

### 🧠 Concepts Reviewed

* **What is a Function?**
    * **Definition:** A block of code that performs a specific task and can be called multiple times.
    * **Analogy:** Like a recipe. You write it once, then use it whenever you need it.
    * **Basic syntax:**
    ```python
    def greet(name):
        return f"Hello, {name}!"
    ```

* **Parameters and Arguments:**
    * **Parameters:** Variables listed in the function definition (e.g., `name` in the example above).
    * **Arguments:** The actual values you pass when calling the function (e.g., `greet("Ritik")`).

* **Return Values:**
    * **What they are:** The output that a function gives back using the `return` keyword.
    * **Example:** `result = add(5, 3)` → The function returns `8`, which is stored in `result`.

* **Functions Without Return:**
    * Some functions perform actions but don't return anything (they return `None` by default).
    * **Example:** A function that prints to the console or saves to a file.

### ✅ Today's Goal
The goal was to understand how to create clean, reusable code through functions. This is the foundation for organizing larger projects like my Jarvis assistant, where each feature (like speech recognition or opening apps) can be its own function.