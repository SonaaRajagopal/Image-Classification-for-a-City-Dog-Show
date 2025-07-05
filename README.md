# 🐶 Image Classification for a City Dog Show

![Python](https://img.shields.io/badge/Python-3.8-blue?logo=python)
![PyTorch](https://img.shields.io/badge/PyTorch-Framework-EE4C2C?logo=pytorch&logoColor=white)
![Model](https://img.shields.io/badge/Models-AlexNet%20%7C%20ResNet%20%7C%20VGG-green)
![Task](https://img.shields.io/badge/Task-Image%20Classification-orange)



## 📜 Overview

Puppyland, a fictionary city is hosting a **citywide dog show**, and I’ve volunteered to help the organizing committee with contestant registration.

Every participant must submit:

- 🐕 An image of their dog  
- 📄 Biographical information

But some people might try to sneak in **non-dog pets** 🐱🦝! So I built a Python-based image classifier to ensure **only dogs** are accepted.



## 🧠 Objective

Build an **image classification system** that can:

- ✅ Detect whether an image is a dog or not
- 🏆 Compare the performance of different CNN architectures to find the best fit for this task



## 🔍 Models Compared

This project implements and compares the performance of three popular CNN architectures:

## 🧪 Results

| Architecture | Accuracy     | Model Size | Speed  |
|--------------|--------------|------------|--------|
| AlexNet      | ✅ Moderate  | 🟢 Small   | ⚡ Fast |
| VGG          | ✅ High      | 🔴 Large   | 🐢 Slow |
| ResNet       | 🏆 Best      | 🟡 Medium  | ⚡ Fast |

📌 **ResNet** performed best overall in terms of accuracy and generalization.


Each model is fine-tuned for the binary task: **dog vs. not-dog**.



## 🗂️ Dataset

- 📸 **Dog images** from registered participants
- ❌ Includes **some non-dog images** to simulate invalid registrations
- 🧹 Preprocessed using standard transforms: resize, normalization, augmentation



## 🛠️ Tech Stack

| Tool        | Description                      |
|-------------|----------------------------------|
| ![Python](https://img.shields.io/badge/Python-3.8-blue?logo=python) | Programming language |
| ![PyTorch](https://img.shields.io/badge/PyTorch-Framework-EE4C2C?logo=pytorch&logoColor=white) | Deep learning framework |
| ![TorchVision](https://img.shields.io/badge/TorchVision-Image%20Utils-purple) | Model zoo & transforms |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-Plotting-yellow) | Accuracy/loss visualization |
| ![Pandas](https://img.shields.io/badge/Pandas-DataFrame-darkblue) | Data handling & logging |




## 🚀 Features

- 🔍 Accurate binary classification: **dog vs. not-dog**
- 📊 Model performance comparison: VGG vs. ResNet vs. AlexNet
- 📈 Plots for training/validation accuracy and loss
- 💾 Save and load best-performing models
- 💬 Summary report with metrics: accuracy, precision, recall



## 🧪 Results

| Architecture | Accuracy | Model Size | Speed |
|--|-||-|
| AlexNet      | ✅ Moderate | 🟢 Small     | ⚡ Fast |
| VGG          | ✅ High     | 🔴 Large     | 🐢 Slow |
| ResNet       | 🏆 Best     | 🟡 Medium    | ⚡ Fast |

📌 **ResNet** performed best overall in terms of accuracy and generalization.



## 📦 Usage

```bash
# Train a selected model
python train.py --model resnet

# Test with a new image
python classify.py --image dog.jpg --model resnet

# Compare all models
python compare_models.py
