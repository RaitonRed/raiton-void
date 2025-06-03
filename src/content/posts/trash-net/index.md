---
title: TrashNet Project
published: 2025-06-03
description: 'Ever wondered how machines can help save the planet? In this project, I built an AI model that classifies trash just by looking at a photo. Using deep learning and Python, this system can tell if an item is plastic, paper, metal, and more. Fast, accurate, and eco-friendly!'
image: './cover.png'
tags: ["Machine Learning", "Projects"]
category: 'Projects'
draft: false 
lang: 'en'
---

# ♻️ TrashNet: Smart Waste Classification with Deep Learning

Have you ever wondered if a machine could recognize waste types just by looking at them?  
Well... I built one! 💡

## 🧠 What is TrashNet?

**TrashNet** is a deep learning-based image classification system that can automatically identify different types of waste, such as:

- 🧻 Paper  
- 🥤 Plastic  
- 🪞 Glass  
- 🥫 Metal  
- 📦 Cardboard  
- 🚮 General Trash

It uses **Convolutional Neural Networks (CNNs)** powered by **TensorFlow** and trained on a labeled image dataset to classify waste into the correct category.

---

## 🔧 Technologies Used

- `Python 3`
- `TensorFlow / Keras`
- `OpenCV`
- `Scikit-learn`
- `NumPy & Matplotlib`
- `Jupyter Notebook`

---

## 📦 Dataset

The dataset is organized into folders for each waste class and contains hundreds of labeled images.  
All images are resized to `128x128` pixels and normalized for training.

Structure:

```
    dataset/
    ├── cardboard/
    ├── glass/
    ├── metal/
    ├── paper/
    ├── plastic/
    └── trash/
```

---

## 🧼 Preprocessing

Images are:
- Resized to a fixed shape
- Normalized between 0 and 1
- Labeled using folder names
- Split into train and test sets (80/20)
- Saved in a `processed_data.pkl` file for fast reuse

```python
img = cv2.imread(img_path)
img = cv2.resize(img, (128, 128))
img = img / 255.0
```

---

## 📊 Results (Coming Soon!)
I’ll publish model performance, confusion matrix, and sample predictions in the next update — stay tuned! 🚀
If you'd like to contribute or suggest improvements, feel free to open a pull request or issue.

---

## 📺 Full Video + Code Coming Soon

I'm working on a full YouTube video tutorial explaining how I built this project step-by-step — from data loading to model evaluation.

Follow me to stay updated!

---

🌍 Let’s make AI work for the planet.

---

## GitHub Repository

::github{repo="RaitonRed/TrashNet"}