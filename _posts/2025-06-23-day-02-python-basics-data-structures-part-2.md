---
title: "Day 2: Python Basics - Data Structures (Part 2)"
description: "Review of Python's fundamental data structures: Tuples and Sets, completing the data structures review."
author: ritikmehta
date: 2025-06-23 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, data structures, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 2: June 23, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I continued with data structures by learning about **Tuples** and **Sets**. These are less common than lists and dictionaries, but they have specific use cases that make them important.

### 🧠 Concepts Reviewed

* **Tuples:**
    * **What they are:** An ordered collection like a list, but *immutable* (cannot be changed after creation).
    * **Analogy:** A sealed package. Once you close it, you can't add or remove items.
    * **Code:** `my_tuple = (1, 2, 3, "fixed")`
    * **When to use:** When you want to protect data from being accidentally modified, like coordinates `(x, y)` or RGB colors `(255, 0, 0)`.

* **Sets:**
    * **What they are:** An *unordered* collection with no duplicate values. Super fast for checking if something exists.
    * **Analogy:** A bag of unique marbles. You can't have two identical marbles, and they're not in any specific order.
    * **Code:** `my_set = {1, 2, 3, 3}` → Results in `{1, 2, 3}`
    * **When to use:** When you need to remove duplicates or check membership quickly.

### ✅ Today's Goal
The goal was to understand when to use immutable (tuples) vs mutable (lists) data structures, and when uniqueness matters (sets). This completes my foundational review of Python's core data structures, preparing me for more complex work ahead.