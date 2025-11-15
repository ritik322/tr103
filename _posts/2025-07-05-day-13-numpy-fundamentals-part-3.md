---
title: "Day 13: NumPy Fundamentals (Part 3)"
description: "Advanced NumPy concepts including reshaping, stacking, and multidimensional arrays."
author: ritikmehta
date: 2025-07-05 09:00:00 +0530
categories: [AI Training, NumPy]
tags: [numpy, arrays, multidimensional, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 13: July 5, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I completed my NumPy learning by exploring **multidimensional arrays** and advanced array manipulation techniques. This is crucial for understanding how data flows through neural networks.

### 🧠 Concepts Learned

* **Multidimensional Arrays:**
    * **1D array:** A simple list of numbers `[1, 2, 3]`
    * **2D array (matrix):** Rows and columns (like a spreadsheet)
    ```python
    matrix = np.array([[1, 2, 3],
                       [4, 5, 6]])
    ```
    * **3D array:** Used for images (height × width × color channels)

* **Reshaping Arrays:**
    * **What it does:** Changes the dimensions without changing the data.
    * **Example:**
    ```python
    array = np.array([1, 2, 3, 4, 5, 6])
    reshaped = array.reshape(2, 3)  # 2 rows, 3 columns
    # [[1, 2, 3],
    #  [4, 5, 6]]
    ```
    * **Flatten:** `array.flatten()` → Convert any shape back to 1D

* **Stacking Arrays:**
    * **Vertical stack:** `np.vstack([a, b])` → Stack arrays vertically
    * **Horizontal stack:** `np.hstack([a, b])` → Stack arrays horizontally
    * **Use case:** Combining datasets or features

* **Copying vs Viewing:**
    * **View:** `array_view = array[:]` → Reference to original (changes affect both)
    * **Copy:** `array_copy = array.copy()` → Independent copy

* **Why This Matters for AI:**
    * **Images:** Represented as 3D arrays (height × width × RGB)
    * **Neural networks:** Process data in batches (4D arrays)
    * **Understanding shapes:** Critical for debugging ML models

### ✅ Today's Goal
The goal was to understand how NumPy handles multidimensional data. This completes my NumPy foundation—I now understand why it's called the "backbone" of scientific computing in Python!