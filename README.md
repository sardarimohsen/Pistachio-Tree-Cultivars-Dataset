
# ICPTC: Iranian Commercial Pistachio Tree Cultivars Dataset

This repository contains the **Iranian Commercial Pistachio Tree Cultivars (ICPTC)** dataset and the implementation of the deep learning model described in our research papers. 

[![Paper 1](https://img.shields.io/badge/Paper-ICPTC%20Dataset-blue)](INSERT_LINK_HERE)
[![Paper 2](https://img.shields.io/badge/Paper-Deep%20Learning%20Model-green)](INSERT_LINK_HERE)

## 📌 Overview
Pistachio cultivation is a vital agricultural sector in Iran. Accurate cultivar identification is crucial for orchard management and economic optimization. This project provides a standardized image dataset of four major commercial Iranian pistachio cultivars and an efficient deep learning architecture for automated identification.



### Cultivars Included:
1.  **Akbari** (Super Long)
2.  **Ahmad Aghaei** (Long)
3.  **Fandoghi** (Round)
4.  **Kalleh-Ghouchi** (Jumbo)

---

## 📊 Dataset: ICPTC
The **ICPTC** dataset consists of high-resolution images captured under field conditions, reflecting real-world challenges such as varying lighting and backgrounds.

*   **Total Images:** [Insert Number, e.g., 4,000+]
*   **Format:** JPG/PNG
*   **Classes:** 4 (Akbari, Ahmad Aghaei, Fandoghi, Kalleh-Ghouchi)
*   **Data Split:** [e.g., 70% Training, 15% Validation, 15% Testing]

---

## 🧠 Model Architecture
Our "Efficient Deep Learning Model" focuses on high accuracy with reduced computational overhead, making it suitable for deployment in agricultural monitoring systems.



### Key Features:
*   **Backbone:** [e.g., Modified MobileNetV2 / ResNet]
*   **Input Size:** [e.g., 224x224]
*   **Optimization:** [e.g., Adam Optimizer with Cross-Entropy Loss]

---

## 🚀 Getting Started

### Prerequisites
*   Python 3.8+
*   PyTorch / TensorFlow (Select the one you used)
*   OpenCV, Pandas, Matplotlib

### Installation
```bash
git clone [https://github.com/your-username/ICPTC-Pistachio-Identification.git](https://github.com/your-username/ICPTC-Pistachio-Identification.git)
cd ICPTC-Pistachio-Identification
pip install -r requirements.txt
```

### Training
To train the model on the ICPTC dataset:
```bash
python train.py --data ./dataset --epochs 50 --batch_size 32
```

---

## 📝 Citation
If you use this dataset or code in your research, please cite the following papers:

**For the Dataset:**
> *Authors (Year). ICPTC: Iranian commercial pistachio tree cultivars standard dataset. Journal Name/Conference.*

**For the Model:**
> *Authors (Year). An efficient deep learning model for cultivar identification of a pistachio tree. Journal Name/Conference.*

---

## 📧 Contact
For questions regarding the dataset or model implementation, please contact:
*   **Name:** [Your Name]
*   **Email:** [Your Email]
*   **Institution:** [Your University/Research Center]
```
