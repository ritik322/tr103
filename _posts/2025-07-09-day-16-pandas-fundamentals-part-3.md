---
title: "Day 16: Pandas Fundamentals (Part 3)"
description: "Grouping, aggregation, and data analysis techniques in Pandas."
author: ritikmehta
date: 2025-07-09 09:00:00 +0530
categories: [AI Training, Pandas]
tags: [pandas, groupby, aggregation, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 16: July 9, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I completed my Pandas learning by exploring **grouping and aggregation**—powerful techniques for analyzing data by categories.

### 🧠 Concepts Learned

* **GroupBy Operations:**
    * **What it does:** Groups data by a category and performs calculations on each group.
    * **Example:**
    ```python
    # Average age by city
    df.groupby('city')['age'].mean()
    ```
    * **Analogy:** Like creating a pivot table in Excel.

* **Aggregation Functions:**
    * **Common functions:** `sum()`, `mean()`, `count()`, `max()`, `min()`, `std()`
    * **Multiple aggregations:**
    ```python
    df.groupby('city').agg({
        'age': ['mean', 'max'],
        'salary': 'sum'
    })
    ```

* **Sorting Data:**
    * **By column:** `df.sort_values('age')` → Ascending order
    * **Descending:** `df.sort_values('age', ascending=False)`
    * **Multiple columns:** `df.sort_values(['city', 'age'])`

* **Merging DataFrames:**
    * **Concatenate:** `pd.concat([df1, df2])` → Stack DataFrames
    * **Merge (like SQL JOIN):**
    ```python
    pd.merge(df1, df2, on='id')
    ```

* **Apply Custom Functions:**
    * **Apply to column:**
    ```python
    df['age'].apply(lambda x: x * 2)
    ```
    * **Apply to entire row:**
    ```python
    df.apply(lambda row: row['age'] + row['bonus'], axis=1)
    ```

* **Why This Matters for AI:**
    * **Feature engineering:** Creating new features from existing data.
    * **Data exploration:** Understanding patterns before building models.
    * **Data cleaning:** Preparing data in the right format for ML algorithms.

### ✅ Today's Goal
The goal was to understand advanced Pandas operations. I now know how to load, clean, filter, group, and analyze data—everything needed to prepare datasets for machine learning!