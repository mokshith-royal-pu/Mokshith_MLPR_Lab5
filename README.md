# MLPR-Lab-5  
## Face Classification using Hue–Saturation Features and K-Means Clustering

---

## 🎯 Aim
The aim of this experiment is to implement a **distance-based face classification system** using colour features extracted from detected face regions. The task involves clustering faces using **K-Means clustering** and classifying a **template face image** based on its proximity to learned clusters.

---

## 🧪 Methodology
The methodology followed in this lab consists of the following steps:

### 1️⃣ Face Detection
- Face detection is performed using **Haar Cascade Classifier** on grayscale images.
- Bounding boxes are drawn around the detected faces.

### 2️⃣ Feature Extraction
- Detected face regions are converted from **BGR to HSV** colour space.
- Mean **Hue** and **Saturation** values are extracted from each face.
- These values form a **2D feature vector** for every detected face.

### 3️⃣ Clustering using K-Means
- Extracted Hue–Saturation features are clustered using **K-Means clustering**.
- Number of clusters is set to **K = 2**.
- Cluster centroids are computed and visualized.

### 4️⃣ Template Image Classification
The template image undergoes the same processing steps:
- Face detection
- HSV colour conversion
- Mean Hue–Saturation feature extraction  
- The template feature vector is classified using the trained **K-Means model**.

---

## 📊 Visualizations and Results

### 🔹 Face Detection Output
Detected faces are highlighted using bounding boxes.

### 🔹 Hue–Saturation Feature Space
Each detected face is plotted in the **Hue–Saturation feature space** along with cluster centroids.

### 🔹 Clustered Faces with Template Image
The template face is plotted together with clustered faces to visualize its assigned class.

---

## 🔍 Key Findings
- Hue and Saturation are effective **low-dimensional features** for basic face grouping.
- K-Means clustering successfully separates faces into distinct clusters.
- The template image is correctly classified based on its proximity to cluster centroids.
- Visualization in Hue–Saturation space clearly illustrates cluster separation.

---

## ✅ Conclusion
This lab demonstrates how **distance-based learning techniques** can be applied to image-based classification problems using simple colour features. The experiment highlights the importance of:
- Feature extraction  
- Distance metrics  
- Clustering and visualization  

It also reinforces the role of **unsupervised learning** in classification tasks where labeled data is unavailable.

---

## 🛠️ Tools and Libraries Used
- Python  
- OpenCV  
- NumPy  
- Matplotlib  
- Scikit-learn  

---

## 📁 Repository Structure
