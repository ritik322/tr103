---
title: "Day 11: NumPy Fundamentals (Part 1)"
description: "Introduction to NumPy and understanding arrays - the foundation of numerical computing in Python."
author: ritikmehta
date: 2025-07-03 09:00:00 +0530
categories: [AI Training, NumPy]
tags: [numpy, arrays, phase-2, ai-libraries]
pin: false
math: false
mermaid: false
---

## 📅 Day 11: July 3, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I started **Phase 2** by learning about **NumPy** (Numerical Python). This is one of the most fundamental libraries in AI/ML, and almost every data science library is built on top of it.

### 🧠 Concepts Learned

* **What is NumPy?**
    * **Definition:** A Python library for working with numerical data efficiently.
    * **Core object:** The **array** (similar to a list, but much faster and more powerful).
    * **Why it matters:** All machine learning libraries (TensorFlow, PyTorch, scikit-learn) use NumPy arrays under the hood.

* **NumPy Arrays vs Python Lists:**
    * **Lists:** Flexible but slow for math operations.
    * **Arrays:** Fixed-type (all elements must be the same type), but incredibly fast for calculations.
    * **Speed difference:** NumPy operations can be 100x faster than Python lists!

* **Creating Arrays:**
    * **From a list:** `np.array([1, 2, 3, 4])`
    * **Zeros:** `np.zeros(5)` → `[0. 0. 0. 0. 0.]`
    * **Ones:** `np.ones(3)` → `[1. 1. 1.]`
    * **Range:** `np.arange(0, 10, 2)` → `[0 2 4 6 8]`
    * **Random:** `np.random.rand(5)` → 5 random numbers between 0 and 1

* **Array Properties:**
    * **Shape:** `array.shape` → Dimensions of the array
    * **Size:** `array.size` → Total number of elements
    * **Data type:** `array.dtype` → Type of data (int, float, etc.)

### ✅ Today's Goal
The goal was to understand **why NumPy exists** and what makes it different from regular Python lists. NumPy is the foundation—without it, modern AI/ML wouldn't be possible at this scale.