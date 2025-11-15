---
title: "Day 5: Python Basics - Functions (Part 2)"
description: "Advanced function concepts including default parameters, *args, **kwargs, and lambda functions."
author: ritikmehta
date: 2025-06-26 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, functions, advanced, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 5: June 26, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I dove deeper into **Functions** by learning more advanced concepts. These techniques make functions more flexible and powerful.

### 🧠 Concepts Reviewed

* **Default Parameters:**
    * **What they are:** Parameters with pre-set values that are used if no argument is provided.
    * **Example:**
    ```python
    def greet(name="Guest"):
        return f"Hello, {name}!"
    
    greet()  # Returns "Hello, Guest!"
    greet("Ritik")  # Returns "Hello, Ritik!"
    ```

* **Variable-Length Arguments (*args):**
    * **What it is:** Allows a function to accept any number of positional arguments.
    * **Example:**
    ```python
    def add_numbers(*args):
        return sum(args)
    
    add_numbers(1, 2, 3, 4)  # Returns 10
    ```

* **Keyword Arguments (**kwargs):**
    * **What it is:** Allows a function to accept any number of keyword arguments as a dictionary.
    * **Example:**
    ```python
    def display_info(**kwargs):
        for key, value in kwargs.items():
            print(f"{key}: {value}")
    
    display_info(name="Ritik", age=20, city="Sangrur")
    ```

* **Lambda Functions:**
    * **What they are:** Small, anonymous functions written in one line.
    * **Syntax:** `lambda arguments: expression`
    * **Example:** `square = lambda x: x**2`
    * **When to use:** For simple operations, especially when passing functions as arguments.

### ✅ Today's Goal
The goal was to understand advanced function techniques that make code more flexible and concise. These concepts are everywhere in Python libraries, including the AI/ML libraries I'll be learning in Phase 2.