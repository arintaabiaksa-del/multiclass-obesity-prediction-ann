# Obesity Levels Classification: ANN vs. Dropout Regularization

This repository contains a comprehensive deep learning project focused on predicting obesity levels based on eating habits and physical conditions. The core of this study is an experimental comparison between a **Baseline ANN** and an **ANN with Dropout Regularization**.

## 📊 Project Overview
The dataset categorizes individuals into 7 different obesity levels. This project explores how deep learning architectures can handle multi-class tabular data and evaluates whether common regularization techniques like Dropout actually improve performance on high-confidence datasets.

## 🧠 Model Architecture
Two models were developed and compared:
1. **Baseline Model:** A Multi-Layer Perceptron (MLP) with dense layers and ReLU activation.
2. **Dropout Model:** The same architecture with added Dropout layers to prevent potential overfitting.



[Image of Artificial Neural Network architecture]


## 🛠️ Tech Stack
- **Framework:** `TensorFlow` / `Keras`
- **Scikit-Learn Integration:** `SciKeras` (for model wrapping and evaluation)
- **Data Processing:** `Pandas`, `NumPy`, `Scikit-Learn` (StandardScaler, LabelEncoder)
- **Environment:** Google Colab

## 📉 Key Findings & Comparison
The experiment yielded a surprising but scientifically significant result:

| Metric | Baseline ANN | ANN + Dropout |
| :--- | :---: | :---: |
| **Accuracy** | **98.33%** | 93.54% |
| **Loss** | **0.0589** | 0.3635 |

### Analysis:
- **Baseline Superiority:** The baseline model achieved near-perfect accuracy, indicating it generalized extremely well without needing regularization.
- **Underfitting via Dropout:** Adding Dropout layers led to a decrease in accuracy. This suggests that the baseline model was not overfitting, and the penalty from Dropout removed too much essential information, causing slight underfitting.

## 🖼️ Visualizations
*(Upload your training history plots to the 'images' folder to display them here)*

### Confusion Matrix
![Confusion Matrix](images/confusion_matrix.png)

### Training vs Validation Loss
![Loss Plot](images/loss_plot.png)

## 📂 Project Structure
- `Klasifikasi_2025.ipynb`: The main notebook containing data preprocessing, model training, and evaluation.
- `dataset/`: (Optional) Folder for the obesity dataset CSV.
- `images/`: Folder for evaluation plots and architecture diagrams.

## 📜 Conclusion
This project demonstrates that **"more complex is not always better."** In cases where the data is clean and the baseline model generalizes perfectly, excessive regularization like Dropout can hinder performance.

---
*Developed for Data Science & Deep Learning Portfolio.*
