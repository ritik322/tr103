---
title: "Day 3: Python Basics - Data Structures (Part 3)"
description: "Practical application of data structures through looping and manipulation techniques."
author: ritikmehta
date: 2025-06-24 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, data structures, loops, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 3: June 24, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I focused on the practical side: **how to actually work with data structures**. It's not enough to just create them—I need to loop through them, access their values, and manipulate them efficiently.

### 🧠 Concepts Reviewed

* **Looping Through Lists:**
    * **Basic for loop:** `for item in my_list:`
    * **With index:** `for i, item in enumerate(my_list):`
    * **List comprehension:** `[x*2 for x in my_list]` - A faster, cleaner way to create new lists.

* **Working with Dictionaries:**
    * **Looping through keys:** `for key in my_dict:`
    * **Looping through values:** `for value in my_dict.values():`
    * **Looping through both:** `for key, value in my_dict.items():`
    * **Safe access:** Using `.get()` to avoid errors when a key doesn't exist.

* **Nested Structures:**
    * **What they are:** Lists inside dictionaries, dictionaries inside lists, etc.
    * **Example:** A list of contacts where each contact is a dictionary:
    ```python
    contacts = [
        {"name": "Alice", "phone": "123"},
        {"name": "Bob", "phone": "456"}
    ]
    ```

### ✅ Today's Goal
The goal was to become comfortable navigating and manipulating complex data structures. This is essential for Phase 2, especially when working with Pandas DataFrames, which are essentially sophisticated nested structures.