---
title: "Day 17: OpenCV Fundamentals (Part 1)"
description: "Introduction to OpenCV - reading, displaying, and basic manipulation of images and videos."
author: ritikmehta
date: 2025-07-10 09:00:00 +0530
categories: [AI Training, OpenCV]
tags: [opencv, computer-vision, images, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 17: July 10, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I started learning **OpenCV** (Open Computer Vision)—the most popular library for working with images and videos in Python. This is essential for any AI project involving visual data.

### 🧠 Concepts Learned

* **What is OpenCV?**
    * **Definition:** A library for computer vision tasks—processing images and videos.
    * **Use cases:** Face detection, object tracking, image filtering, video analysis.
    * **Why it matters:** Most AI vision applications (self-driving cars, facial recognition) use OpenCV.

* **Images as Arrays:**
    * **Key insight:** Images are just NumPy arrays!
    * **Grayscale image:** 2D array (height × width)
    * **Color image (RGB):** 3D array (height × width × 3 channels)
    * **Each pixel:** A number representing color intensity (0-255)

* **Reading and Displaying Images:**
    * **Read image:**
    ```python
    import cv2
    img = cv2.imread('photo.jpg')
    ```
    * **Display image:**
    ```python
    cv2.imshow('My Image', img)
    cv2.waitKey(0)  # Wait for key press
    cv2.destroyAllWindows()
    ```

* **Image Properties:**
    * **Shape:** `img.shape` → (height, width, channels)
    * **Size:** `img.size` → Total number of pixels
    * **Data type:** `img.dtype` → Usually uint8 (0-255)

* **Color Spaces:**
    * **BGR vs RGB:** OpenCV uses BGR (Blue-Green-Red) by default, not RGB!
    * **Convert to RGB:**
    ```python
    img_rgb = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
    ```
    * **Convert to Grayscale:**
    ```python
    gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
    ```

* **Saving Images:**
    * **Write to file:**
    ```python
    cv2.imwrite('output.jpg', img)
    ```

### ✅ Today's Goal
The goal was to understand what OpenCV is and how images are represented in Python. Images are just arrays of numbers—this simple concept is the foundation of all computer vision!