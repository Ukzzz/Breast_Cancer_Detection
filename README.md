# 🩺 Breast Cancer Detection using Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-Latest-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

A machine learning project that uses **Logistic Regression** to classify breast cancer tumors as **Malignant** or **Benign** with **96.49% accuracy** using the Wisconsin Breast Cancer Dataset.

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Usage](#-usage)
- [Model Performance](#-model-performance)
- [License](#-license)

---

## 🔍 Overview

Early detection of breast cancer significantly improves survival rates and treatment outcomes. This project leverages machine learning to assist in the classification of breast tumors based on features computed from digitized images of fine needle aspirate (FNA) of breast masses.

### Key Highlights:

- 🎯 **96.49% Accuracy** on test data
- 📊 Comprehensive data preprocessing and feature scaling
- 🔬 Uses 30 computed features from cell nuclei
- ⚡ Fast inference with Logistic Regression

---

## 📊 Dataset

This project uses the **Wisconsin Breast Cancer Dataset** (WBCD), which is publicly available from the UCI Machine Learning Repository.

| Attribute       | Value       |
| --------------- | ----------- |
| Total Samples   | 569         |
| Malignant Cases | 212 (37.3%) |
| Benign Cases    | 357 (62.7%) |
| Features        | 30          |

---

## 📁 Project Structure

```
Breast Cancer Detection/
│
├── data/
│   └── breast_cancer.csv          # Dataset file
│
├── notebooks/
│   └── Breast_Cancer_Detection.ipynb  # Main Jupyter notebook
│
├── docs/
│   ├── MODEL_CARD.md              # Model documentation
│   └── DATA_DICTIONARY.md         # Feature descriptions
│
├── .gitignore
├── requirements.txt
├── LICENSE
├── CONTRIBUTING.md
└── README.md
```

---

## 🚀 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/breast-cancer-detection.git
   cd breast-cancer-detection
   ```

2. **Create a virtual environment** (recommended)

   ```bash
   python -m venv venv
   venv\Scripts\activate   # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 💻 Usage

```bash
jupyter notebook notebooks/Breast_Cancer_Detection.ipynb
```

---

## 📈 Model Performance

| Class        | Precision | Recall | F1-Score   |
| ------------ | --------- | ------ | ---------- |
| Benign       | 0.96      | 0.99   | 0.97       |
| Malignant    | 0.97      | 0.93   | 0.95       |
| **Accuracy** |           |        | **96.49%** |

---

## 🛠️ Technologies Used

- Python
- NumPy & Pandas
- Matplotlib & Seaborn
- Scikit-learn

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- UCI Machine Learning Repository for the Wisconsin Breast Cancer Dataset
- Dr. William H. Wolberg (University of Wisconsin Hospitals)

---

<p align="center">Made with ❤️ for advancing healthcare AI</p>
