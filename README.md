# ICPTC: Iranian Commercial Pistachio Tree Cultivars Dataset & Deep Learning Model

This repository contains the dataset and codebase for the **Iranian Commercial Pistachio Tree Cultivars (ICPTC)** project. This project includes both a standardized image dataset of several major pistachio cultivars and an efficient deep learning model for automated cultivar identification.

[![Mendeley Dataset](https://img.shields.io/badge/Mendeley-Dataset-red)](https://data.mendeley.com/datasets/6mmjjkpd5m/1)
[![Dataset Paper](https://img.shields.io/badge/DOI-Data%20in%20Brief-blue)](https://doi.org/10.1016/j.dib.2021.107348)
[![Model Paper](https://img.shields.io/badge/DOI-British%20Food%20Journal-green)](https://doi.org/10.1108/bfj-12-2020-1100)

---

## 📌 Project Overview

Identifying pistachio tree cultivars directly from field images is a highly challenging fine-grained classification task due to subtle visual differences in branch expansion, leaf patterns, shapes, and colors. Accurate recognition supports orchardists in improving crop yields, reducing management costs, and optimizing economic value.

This repository provides:
1. **The ICPTC Dataset:** 526 high-resolution field images captured under uncontrolled real-world conditions (varying angles, distances, and sunlight).
2. **The Model Architecture:** A high-performance, computationally efficient deep learning approach designed specifically to classify pistachio tree cultivars using representative image patches to oversample small datasets.

---

## 📊 Dataset: ICPTC

The ICPTC dataset comprises RGB color images belonging to four primary Iranian pistachio cultivars collected from natural habitats within pistachio orchards in the Chah-Afzal region of Yazd, Iran.

### Cultivars Included
The four major commercial Iranian pistachio tree cultivars featured in this dataset are:
* **Jumbo** (*Kalleh-Ghouchi*)
* **Long** (*Ahmad-Aghaei*)
* **Round** (*Fandoghi / O'hadi*)
* **Super-Long** (*Akbari*)

### Key Specifications
* **Total Images:** 526 RGB images
* **Distribution:** Varies between 109 and 171 images per cultivar class.
* **Imaging Conditions:** Images were captured under real-world, uncontrolled conditions during the spring season (April and May), featuring varying camera-to-target distances, diverse viewpoints, multiple angles, and natural sunlight.
* **Dataset Partitioning:**
  * **Training Set:** 63%
  * **Validation Set:** 17%
  * **Test Set:** 20% *(Note: Test images are completely separated from trees used in the training phase to ensure reliable evaluation).*

---

## 🧠 Model Architecture

The deep learning model addresses the challenge of limited training samples by incorporating an innovative data augmentation and oversampling strategy. 
* **Keypoint Extraction:** Uses ORB (Oriented FAST and Rotated BRIEF) keypoint detection to extract highly distinct image patches.
* **Overfitting Prevention:** Patches are extracted from training images and used to oversample the dataset, ensuring the model avoids overfitting on small image samples.
* **Backbone:** Convolutional layers based on the **ResNet** architecture, fine-tuned specifically for agricultural fine-grained image classification.

---

## 🔗 Data Accessibility

The official dataset can be accessed and cited using the following official Mendeley Data link:

* **Mendeley Data Repository:** [ICPTC: Iranian Commercial Pistachios Tree Cultivars](https://data.mendeley.com/datasets/6mmjjkpd5m/1)

---

## 🚀 Getting Started

### Prerequisites & Installation
Ensure you have Python 3.8+ installed. Clone this repository and install the dependencies:
```bash
git clone [https://github.com/your-username/ICPTC-Pistachio-Identification.git](https://github.com/your-username/ICPTC-Pistachio-Identification.git)
cd ICPTC-Pistachio-Identification
pip install -r requirements.txt
```

### Usage
Extract ORB image patches and train the deep learning model on the dataset using the following script:
```bash
python train.py --dataset_path ./dataset/icptc --epochs 50 --batch_size 32
```

---

## 📄 References & BibTeX

If you use this dataset or model in your academic work, please cite the following papers:

### **Dataset Reference**
> Heidary-Sharifabad, A., Zarchi, M. S., & Zarei, G. (2021). ICPTC: Iranian commercial pistachio tree cultivars standard dataset. *Data in Brief*, *38*, 107348. https://doi.org/10.1016/j.dib.2021.107348

```bibtex
@article{HeidarySharifabad2021ICPTC,
  author    = {Heidary-Sharifabad, Ahmad and Zarchi, Mohsen Sardari and Zarei, Gholamreza},
  title     = {ICPTC: Iranian commercial pistachio tree cultivars standard dataset},
  journal   = {Data in Brief},
  year      = {2021},
  volume    = {38},
  pages     = {107348},
  doi       = {10.1016/j.dib.2021.107348}
}
```

### **Model Reference**
> Heidary-Sharifabad, A., Zarchi, M. S., Emadi, S., & Zarei, G. (2021). An efficient deep learning model for cultivar identification of a pistachio tree. *British Food Journal*, *123*(11), 3592-3609. https://doi.org/10.1108/bfj-12-2020-1100

```bibtex
@article{HeidarySharifabad2021Efficient,
  author    = {Heidary-Sharifabad, Ahmad and Zarchi, Mohsen Sardari and Emadi, Sima and Zarei, Gholamreza},
  title     = {An efficient deep learning model for cultivar identification of a pistachio tree},
  journal   = {British Food Journal},
  year      = {2021},
  volume    = {123},
  number    = {11},
  pages     = {3592--3609},
  doi       = {10.1108/bfj-12-2020-1100}
}
```
