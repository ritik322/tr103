---
title: "Day 12: NumPy Fundamentals (Part 2)"
description: "Array operations, indexing, slicing, and mathematical operations with NumPy."
author: ritikmehta
date: 2025-07-04 09:00:00 +0530
categories: [AI Training, NumPy]
tags: [numpy, arrays, operations, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 12: July 4, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I continued with **NumPy** by learning how to actually work with arrays—indexing, slicing, and performing mathematical operations efficiently.

### 🧠 Concepts Learned

* **Array Indexing:**
    * **Single element:** `array[2]` → Access the element at index 2
    * **Negative indexing:** `array[-1]` → Last element
    * **2D arrays:** `array[row, column]` → Access specific position

* **Array Slicing:**
    * **Basic slice:** `array[1:4]` → Elements from index 1 to 3
    * **Step size:** `array[::2]` → Every second element
    * **2D slicing:** `array[0:2, 1:3]` → Rows 0-1, columns 1-2

* **Mathematical Operations:**
    * **Element-wise operations:**
    ```python
    a = np.array([1, 2, 3])
    b = np.array([4, 5, 6])
    a + b  # [5, 7, 9]
    a * b  # [4, 10, 18]
    ```
    * **Scalar operations:**
    ```python
    a * 2   # [2, 4, 6]
    a ** 2  # [1, 4, 9]
    ```

* **Useful Functions:**
    * **Sum:** `np.sum(array)` → Total of all elements
    * **Mean:** `np.mean(array)` → Average
    * **Max/Min:** `np.max(array)`, `np.min(array)`
    * **Standard deviation:** `np.std(array)`

* **Broadcasting:**
    * **What it is:** NumPy's ability to perform operations on arrays of different shapes.
    * **Example:** Adding a scalar to an array automatically "broadcasts" the scalar to every element.

### ✅ Today's Goal
The goal was to understand how to manipulate and perform calculations on NumPy arrays. These operations are the building blocks of all data processing in machine learning.