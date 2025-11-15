---
title: "Day 6: Python Basics - Modules and Imports"
description: "Understanding how to use and import Python modules to leverage existing code and libraries."
author: ritikmehta
date: 2025-06-27 09:00:00 +0530
categories: [AI Training, Python]
tags: [python, basics, modules, imports, phase-1]
pin: false
math: false
mermaid: false
---

## 📅 Day 6: June 27, 2025

### 📝 Phase 1: Python Basics (Review)

Today, I focused on **Modules and Imports**—the mechanism that allows Python programmers to use code written by others. This is how I can use powerful libraries without writing everything from scratch.

### 🧠 Concepts Reviewed

* **What is a Module?**
    * **Definition:** A Python file (`.py`) that contains functions, classes, or variables that can be used in other programs.
    * **Analogy:** Like a toolbox. You don't need to build every tool yourself—you just import the toolbox and use what you need.

* **Importing Modules:**
    * **Basic import:** `import math` → Access functions like `math.sqrt(16)`
    * **Import specific items:** `from math import sqrt` → Use directly: `sqrt(16)`
    * **Import with alias:** `import numpy as np` → Shorter name: `np.array([1,2,3])`
    * **Import everything (not recommended):** `from math import *`

* **Standard Library vs External Libraries:**
    * **Standard Library:** Built-in modules that come with Python (e.g., `math`, `random`, `datetime`).
    * **External Libraries:** Must be installed using `pip` (e.g., `pip install pyttsx3`).

* **Creating Your Own Module:**
    * **What it is:** Simply save functions in a `.py` file and import it.
    * **Example:** Save `my_functions.py` with a function, then use `import my_functions`.

### ✅ Today's Goal
The goal was to understand how Python's ecosystem works. In my Jarvis project, I use `import pyttsx3`, `import speech_recognition`, etc. Now I understand what's happening behind the scenes—I'm accessing pre-written code that others have created and shared.