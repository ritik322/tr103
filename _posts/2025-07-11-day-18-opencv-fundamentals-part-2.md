---
title: "Day 18: OpenCV Fundamentals (Part 2)"
description: "Image manipulation, drawing shapes, and working with video in OpenCV."
author: ritikmehta
date: 2025-07-11 09:00:00 +0530
categories: [AI Training, OpenCV]
tags: [opencv, computer-vision, video, phase-2]
pin: false
math: false
mermaid: false
---

## 📅 Day 18: July 11, 2025

### 📝 Phase 2: The "AI" Libraries (Knowledge)

Today, I completed my OpenCV learning by exploring **image manipulation** and **video processing**. This marks the end of the AI Libraries phase!

### 🧠 Concepts Learned

* **Basic Image Operations:**
    * **Resize:**
    ```python
    resized = cv2.resize(img, (width, height))
    ```
    * **Crop:** Simple array slicing:
    ```python
    cropped = img[100:300, 200:400]  # [rows, columns]
    ```
    * **Rotate:**
    ```python
    (h, w) = img.shape[:2]
    center = (w // 2, h // 2)
    M = cv2.getRotationMatrix2D(center, 45, 1.0)  # 45 degrees
    rotated = cv2.warpAffine(img, M, (w, h))
    ```

* **Drawing on Images:**
    * **Line:**
    ```python
    cv2.line(img, (0, 0), (100, 100), (255, 0, 0), 2)
    ```
    * **Rectangle:**
    ```python
    cv2.rectangle(img, (50, 50), (200, 200), (0, 255, 0), 3)
    ```
    * **Circle:**
    ```python
    cv2.circle(img, (150, 150), 50, (0, 0, 255), -1)  # -1 = filled
    ```
    * **Text:**
    ```python
    cv2.putText(img, 'Hello', (50, 100), cv2.FONT_HERSHEY_SIMPLEX, 1, (255, 255, 255), 2)
    ```

* **Working with Video:**
    * **Read video:**
    ```python
    cap = cv2.VideoCapture('video.mp4')
    while True:
        ret, frame = cap.read()
        if not ret:
            break
        cv2.imshow('Video', frame)
        if cv2.waitKey(1) & 0xFF == ord('q'):
            break
    cap.release()
    ```
    * **Use webcam:** `cv2.VideoCapture(0)` → 0 is the default camera

* **Saving Video:**
    * **Create writer:**
    ```python
    fourcc = cv2.VideoWriter_fourcc(*'XVID')
    out = cv2.VideoWriter('output.avi', fourcc, 20.0, (640, 480))
    ```

* **Why This Matters for AI:**
    * **Preprocessing:** Resizing, cropping images before feeding to AI models.
    * **Data augmentation:** Rotating, flipping images to create more training data.
    * **Visualization:** Drawing bounding boxes on detected objects.
    * **Real-time applications:** Processing webcam feeds for face detection, gesture recognition.

### ✅ Phase 2 Complete!
Today marks the completion of **Phase 2: The "AI" Libraries**. I've learned:
- **NumPy:** Fast numerical arrays
- **Pandas:** Data manipulation and analysis
- **OpenCV:** Image and video processing

Tomorrow, I move to **Phase 3: "Something About AI"** where I'll learn the theory and concepts behind artificial intelligence!