---
title: "Day 23: ML Problem Types"
description: "Understanding the three basic problem types: Regression, Classification, and Clustering."
author: ritikmehta
date: 2025-07-18 09:00:00 +0530
categories: [AI Training, AI Concepts]
tags: [machine-learning, regression, classification, clustering, phase-3, theory]
pin: false
math: false
mermaid: false
---

## 📅 Day 23: July 18, 2025

### 📝 Phase 3: "Something About AI" (Pure Concepts)

Today, I learned about the **3 Basic Problem Types** in machine learning—the fundamental tasks that ML algorithms are designed to solve.

### 🧠 Concepts Learned

* **1. Regression (Supervised Learning):**
    * **Definition:** Predicting a continuous numerical value.
    * **Key characteristic:** The output is a number on a continuous scale.
    * **Question it answers:** "How much?" or "How many?"
    
    * **Examples:**
        - **House price prediction:** Given features (size, location, bedrooms) → Predict price ($250,000)
        - **Temperature forecasting:** Given weather data → Predict tomorrow's temperature (28°C)
        - **Sales forecasting:** Given historical data → Predict next month's sales (₹5,00,000)
        - **Age estimation:** Given a photo → Predict person's age (32 years)
    
    * **Common algorithms:**
        - Linear Regression
        - Decision Trees
        - Neural Networks

---

* **2. Classification (Supervised Learning):**
    * **Definition:** Predicting a category or class.
    * **Key characteristic:** The output is a discrete label from predefined categories.
    * **Question it answers:** "Which category?" or "What type?"
    
    * **Types:**
        - **Binary Classification:** Only 2 categories (Yes/No, True/False)
        - **Multi-class Classification:** 3+ categories
    
    * **Examples:**
        - **Email spam detection:** Classify as "spam" or "not spam" (binary)
        - **Image recognition:** Classify as "cat," "dog," "bird," etc. (multi-class)
        - **Medical diagnosis:** Classify disease as "Type A," "Type B," or "Healthy" (multi-class)
        - **Sentiment analysis:** Classify review as "positive," "negative," or "neutral" (multi-class)
    
    * **Common algorithms:**
        - Logistic Regression
        - Support Vector Machines (SVM)
        - Random Forests
        - Neural Networks

---

* **3. Clustering (Unsupervised Learning):**
    * **Definition:** Grouping similar items together without predefined labels.
    * **Key characteristic:** No "correct answer"—the algorithm discovers natural groupings.
    * **Question it answers:** "What are the natural groups?"
    
    * **Examples:**
        - **Customer segmentation:** Group customers by purchasing behavior (find 3 types of shoppers)
        - **Document organization:** Group news articles by topic automatically
        - **Image compression:** Group similar colors together
        - **Market research:** Find segments in survey data
    
    * **Common algorithms:**
        - K-Means Clustering
        - Hierarchical Clustering
        - DBSCAN

---

* **How to Choose:**
    * **Need to predict a number?** → Use **Regression**
    * **Need to predict a category?** → Use **Classification**
    * **Need to find natural groups?** → Use **Clustering**

### ✅ Today's Goal
The goal was to understand the three fundamental problem types in ML. Every machine learning project falls into one of these categories—knowing which type helps you choose the right approach and algorithm!