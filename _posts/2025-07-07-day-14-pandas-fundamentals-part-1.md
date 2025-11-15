---
title: "Day 14: Pandas Fundamentals (Part 1)"
description: "Introduction to Pandas and DataFrames - the spreadsheet of Python for data analysis."
author: ritikmehta
date: 2025-07-07 09:00:00 +0530
categories: [AI Training, Pandas]
tags: [pandas, dataframes, data-analysis, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 14: July 7, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I started learning **Pandas**—the most important library for working with structured data in Python. If NumPy is for numerical arrays, Pandas is for "spreadsheets in code."

### 🧠 Concepts Learned

* **What is Pandas?**
    * **Definition:** A library for data manipulation and analysis.
    * **Core object:** The **DataFrame** (think Excel spreadsheet, but in Python).
    * **Why it matters:** Almost all real-world AI projects start with cleaning and preparing data using Pandas.

* **DataFrames vs NumPy Arrays:**
    * **NumPy:** Fast for numerical operations, but no column names.
    * **Pandas:** Built on NumPy, but adds labels, column names, and powerful data tools.

* **Creating DataFrames:**
    * **From dictionary:**
    ```python
    data = {
        'name': ['Alice', 'Bob', 'Charlie'],
        'age': [25, 30, 35],
        'city': ['Delhi', 'Mumbai', 'Bangalore']
    }
    df = pd.DataFrame(data)
    ```
    * **From CSV file:** `df = pd.read_csv('data.csv')`
    * **From Excel:** `df = pd.read_excel('data.xlsx')`

* **Viewing Data:**
    * **First rows:** `df.head()` → Shows first 5 rows
    * **Last rows:** `df.tail()` → Shows last 5 rows
    * **Info:** `df.info()` → Data types and memory usage
    * **Statistics:** `df.describe()` → Summary statistics (mean, max, min, etc.)

* **Basic DataFrame Properties:**
    * **Shape:** `df.shape` → (rows, columns)
    * **Columns:** `df.columns` → List of column names
    * **Data types:** `df.dtypes` → Type of each column

### ✅ Today's Goal
The goal was to understand what Pandas is and why it's essential for data work. DataFrames are the standard format for data in machine learning—before you can train a model, you need to load and explore your data with Pandas.