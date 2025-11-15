---
title: "Day 24: Core ML Vocabulary"
description: "Understanding the essential terms: Model, Features, and Labels - the ingredients of machine learning."
author: ritikmehta
date: 2025-07-21 09:00:00 +0530
categories: [AI Training, AI Concepts]
tags: [machine-learning, model, features, labels, phase-3, theory]
pin: false
math: false
mermaid: false
---

## 📅 Day 24: July 21, 2025

### 📝 Phase 3: "Something About AI" (Pure Concepts)

Today, I learned the **Core ML Vocabulary**—the essential terms that every AI practitioner uses. Understanding these "ingredients" is crucial for discussing any machine learning project.

### 🧠 Concepts Learned

* **1. Model:**
    * **Definition:** The "brain" or system that is created after training. It's what has "learned" the patterns from data.
    * **Analogy:** Like a trained employee who has learned to do a job. After training, they can perform the task independently.
    * **Technical view:** A mathematical function that maps inputs to outputs.
    * **In practice:** Often saved as a file (`.pkl`, `.h5`, `.pt`) that can be loaded and used.
    
    * **Example:**
        - You train a model on 10,000 house sale records
        - The model learns the relationship between features and prices
        - Save the model as `house_price_model.pkl`
        - Now you can use it to predict prices for new houses
    
    * **Types of models:**
        - Linear Regression Model
        - Neural Network Model
        - Decision Tree Model
        - etc.

---

* **2. Features:**
    * **Definition:** The inputs or "clues" you give to the model. The information the model uses to make predictions.
    * **Analogy:** Like the questions a doctor asks before diagnosis (symptoms = features).
    * **Also called:** Input variables, independent variables, predictors, attributes.
    
    * **Examples:**
        - **House price prediction:**
            - Features: Number of bedrooms, square feet, location, age of house, number of bathrooms
        - **Email spam detection:**
            - Features: Number of suspicious words, sender domain, email length, presence of links
        - **Medical diagnosis:**
            - Features: Age, blood pressure, cholesterol level, symptoms
        - **Image recognition:**
            - Features: Pixel values (or extracted features like edges, shapes)
    
    * **Feature engineering:**
        - The process of selecting and creating useful features
        - One of the most important skills in ML
        - Example: Creating a new feature "price per square foot" from "price" and "square feet"

---

* **3. Label:**
    * **Definition:** The answer or "output" you are trying to predict. The target variable.
    * **Analogy:** Like the correct answer on a test answer key.
    * **Also called:** Output variable, target variable, dependent variable, response.
    * **Important note:** Only used in **Supervised Learning** (Unsupervised Learning has no labels!)
    
    * **Examples:**
        - **House price prediction:**
            - Label: The actual price ($450,000)
        - **Email spam detection:**
            - Label: "Spam" or "Not Spam"
        - **Medical diagnosis:**
            - Label: The disease name or "Healthy"
        - **Student performance:**
            - Label: Final exam score or Pass/Fail
    
    * **Training vs. Testing:**
        - **During training:** Model sees both features AND labels (learns the relationship)
        - **During prediction:** Model only sees features (predicts the label)

---

* **Putting It All Together:**
    ```
    Features (Input)  →  [MODEL]  →  Label (Output)
    
    Example:
    [Bedrooms=3,         →  [House Price]  →  $350,000
     SqFt=1500,              Model
     Location=Suburb]
    ```

### ✅ Today's Goal
The goal was to master the three fundamental ML terms: **Model**, **Features**, and **Labels**. These words appear in every ML conversation—now I can speak the language of AI!