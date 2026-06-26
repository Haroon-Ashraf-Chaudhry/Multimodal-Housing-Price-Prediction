<div align="center">

# 🏠 Multimodal Housing Price Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

A machine learning project that predicts housing prices by fusing **structured tabular data** (numerical/categorical features) with **unstructured visual data** (property images) through a multimodal deep learning architecture — going beyond traditional single-modality approaches for more accurate and context-aware price estimation.

</div>

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Project Architecture](#-project-architecture)
- [Tech Stack](#-tech-stack)
- [Dataset](#-dataset)
- [Installation](#-installation)
- [Usage](#-usage)
- [Results](#-results)
- [Project Structure](#-project-structure)
- [License](#-license)

---

## 🔍 Overview

Traditional housing price prediction models rely solely on structured features such as square footage, number of bedrooms, and location. This project pushes the boundary by incorporating **property images** alongside tabular features to form a **multimodal prediction pipeline**.

The model learns both low-level visual patterns (e.g., property condition, architectural style) and high-level numerical relationships, combining them through a fusion layer to produce more accurate price predictions.

---

## ✨ Key Features

- **Multimodal Fusion**: Combines image-based and tabular feature representations in a unified model
- **CNN-based Visual Encoder**: Extracts meaningful visual embeddings from property images using a convolutional neural network
- **Tabular Feature Engineering**: Handles missing values, categorical encoding, and numerical scaling
- **End-to-End Training**: Joint optimization across both modalities
- **Evaluation Metrics**: Reports MAE, RMSE, and R² for model performance assessment
- **Reproducible Notebook**: Fully documented Jupyter Notebook for step-by-step reproducibility

---

## 🏗️ Project Architecture

```
Property Images  ──►  CNN Encoder  ──►  Image Embeddings  ──┐
                                                             ├──► Fusion Layer ──► Price Prediction
Tabular Features ──►  MLP Branch   ──►  Tabular Embeddings ─┘
```

1. **Image Branch**: A CNN (e.g., ResNet or custom architecture) processes property photos and outputs a fixed-size feature vector.
2. **Tabular Branch**: A multi-layer perceptron processes structured features (bedrooms, bathrooms, area, location, etc.).
3. **Fusion Layer**: Concatenates both embeddings and passes them through fully connected layers to predict the final price.

---

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Language | Python 3.8+ |
| Deep Learning | TensorFlow / PyTorch |
| Data Processing | Pandas, NumPy |
| Image Processing | Pillow, OpenCV |
| Visualization | Matplotlib, Seaborn |
| Environment | Jupyter Notebook |

---

## 📊 Dataset

The project uses a housing dataset comprising:

- **Structured features**: property size, number of rooms, floor level, location attributes, age of property, etc.
- **Unstructured features**: exterior and interior images of the properties

> **Note**: Ensure the dataset is placed in the appropriate directory before running the notebook. See the notebook for exact path configuration.

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Haroon-Ashraf-Chaudhry/Multimodal-Housing-Price-Prediction.git
cd Multimodal-Housing-Price-Prediction
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn pillow torch torchvision jupyter
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook Multimodal_Housing_Price_Prediction.ipynb
```

---

## 🚀 Usage

Open the notebook and execute the cells sequentially:

1. **Data Loading & EDA** — Load and explore both tabular and image data
2. **Preprocessing** — Clean, encode, and normalize tabular features; resize and normalize images
3. **Model Building** — Define CNN encoder, tabular MLP, and fusion network
4. **Training** — Train the multimodal model with appropriate loss and optimizer
5. **Evaluation** — Assess model performance using MAE, RMSE, and R²
6. **Inference** — Run predictions on new property inputs

---

## 📈 Results

The multimodal model demonstrates improved predictive accuracy compared to unimodal baselines:

| Model | MAE | RMSE | R² |
|---|---|---|---|
| Tabular-Only (MLP) | — | — | — |
| Image-Only (CNN) | — | — | — |
| **Multimodal Fusion** | **—** | **—** | **—** |

> Specific metric values are reported inside the notebook upon execution.

---

## 📁 Project Structure

```
Multimodal-Housing-Price-Prediction/
│
├── Multimodal_Housing_Price_Prediction.ipynb   # Main project notebook
├── README.md                                   # Project documentation
└── LICENSE                                     # MIT License
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**Haroon Ashraf Chaudhry**

[![GitHub](https://img.shields.io/badge/GitHub-Haroon--Ashraf--Chaudhry-181717?style=flat-square&logo=github)](https://github.com/Haroon-Ashraf-Chaudhry)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin)](https://linkedin.com/in/haroon-ashraf-chaudhry)

---

<div align="center">

⭐ **If you find this repository useful, please consider giving it a star!** ⭐

</div>
