---

# 🚦 Road Scene Semantic Segmentation using SAM, CAM, and DANet

## 📌 Project Overview

This project focuses on **semantic segmentation of urban road scenes**, leveraging advanced deep learning architectures to accurately identify and label each pixel in an image into predefined semantic categories (e.g., road, building, car, pedestrian, sky, etc.). The models were trained and evaluated on the **Cityscapes dataset**, a benchmark dataset for pixel-level scene understanding in urban environments.

Our goal was to evaluate and compare the performance of three attention-based architectures:

* **SAM (Spatial Attention Module)**
* **CAM (Channel Attention Module)**
* **DANet (Dual Attention Network)**

---

## 🧠 Models Used

### 1. **SAM**

The Spatial Attention Module enhances the model's focus on “where” to look in the image by capturing spatial dependencies.

### 2. **CAM**

The Channel Attention Module enhances “what” features are important by focusing on inter-channel relationships.

### 3. **DANet**

Combines both spatial and channel attention mechanisms to jointly optimize feature selection, allowing it to model complex and context-rich scenes more effectively.

---

## 🗂️ Dataset

* **Cityscapes**: A large-scale dataset of diverse urban street scenes across 50 cities.
* Contains finely annotated semantic segmentation maps.
* Input image size: Resized to **512 × 256** during training and inference.

---

## 🔧 Key Features

* Implemented and trained attention-based semantic segmentation models using TensorFlow/Keras.
* Used custom preprocessing and augmentation pipelines.
* Compared visual and quantitative results (mIoU) across models.
* Efficient visualization of prediction masks using **Viridis** colormap and **Matplotlib**.

---

## 📊 Results

* Achieved a **mean Intersection over Union (mIoU) of 81.72%**.
* **Figure 5** (see below) illustrates side-by-side comparisons of the semantic output masks from all three models across randomly selected road scenes.
* Table 3 summarizes the performance metrics (mIoU) of each model.

> 🔍 *Attention Networks demonstrated superior ability to capture fine-grained features and model complex spatial dependencies, which is evident both in visual outputs and performance metrics.*

---

## 📁 Project Structure

```
├── models/
│   ├── sam_model.keras
│   ├── cam_model.keras
│   └── danet_model.keras
├── notebooks/
│   ├── SAM.ipynb
│   ├── CAM.ipynb
│   └── DANet.ipynb
├── outputs/
│   ├── semantic_comparison.png
│   ├── DANet_overlays.png
│   ├── overlay_1.png
│   └── overlay_2.png
├── README.md
└── requirements.txt
```

---

## 🖼️ Visualizations

![semantic_comparison_with_original](https://github.com/user-attachments/assets/077bd593-b546-47b6-94fa-b7dfeb5bcf0c)


---

## 📌 Future Work

* Explore multi-scale feature fusion for improved performance.
* Deploy model on edge devices (e.g., Jetson Nano or Raspberry Pi) for real-time road scene understanding.
* Extend the evaluation to additional datasets like BDD100K.

---

## 👨‍💻 Contributors

* *Rohith Vishwa S*
* *Kannan R V*
* *Hari Swaminathan M*
* *Suhaas M* 
* *Dr.T.Bagyammal* – Project Supervision

---
