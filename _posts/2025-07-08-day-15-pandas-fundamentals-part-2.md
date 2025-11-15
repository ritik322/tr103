---
title: "Day 15: Pandas Fundamentals (Part 2)"
description: "Data selection, filtering, and manipulation in Pandas DataFrames."
author: ritikmehta
date: 2025-07-08 09:00:00 +0530
categories: [AI Training, Pandas]
tags: [pandas, dataframes, data-manipulation, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 15: July 8, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I learned how to **select, filter, and manipulate** data in Pandas. This is where Pandas really shines—making it easy to extract exactly the data you need.

### 🧠 Concepts Learned

* **Selecting Columns:**
    * **Single column:** `df['name']` → Returns a Series (1D)
    * **Multiple columns:** `df[['name', 'age']]` → Returns a DataFrame (2D)

* **Selecting Rows:**
    * **By position (iloc):** `df.iloc[0]` → First row
    * **By label (loc):** `df.loc[0]` → Row with index 0
    * **Range:** `df.iloc[0:3]` → Rows 0, 1, 2

* **Filtering Data (Boolean Indexing):**
    * **Simple filter:**
    ```python
    df[df['age'] > 25]  # Only rows where age > 25
    ```
    * **Multiple conditions:**
    ```python
    df[(df['age'] > 25) & (df['city'] == 'Delhi')]
    ```
    * **Using OR:** Use `|` instead of `&`

* **Adding/Modifying Columns:**
    * **New column:**
    ```python
    df['age_in_months'] = df['age'] * 12
    ```
    * **Modify existing:**
    ```python
    df['age'] = df['age'] + 1  # Everyone gets 1 year older
    ```

* **Dropping Columns/Rows:**
    * **Drop column:** `df.drop('column_name', axis=1)`
    * **Drop row:** `df.drop(0, axis=0)` → Drop row at index 0

* **Handling Missing Data:**
    * **Check for missing:** `df.isnull()` or `df.isna()`
    * **Drop missing:** `df.dropna()`
    * **Fill missing:** `df.fillna(0)` → Replace NaN with 0

### ✅ Today's Goal
The goal was to learn how to extract and clean data from DataFrames. In real AI projects, 80% of the time is spent preparing data—Pandas makes this process manageable.