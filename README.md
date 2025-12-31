# ♻️ AI Waste Classifier: Organic vs. Recyclable
### *A Deep Learning Project for Smart Waste Management*

![TensorFlow](https://img.shields.io/badge/TensorFlow-2.10.0-FF6F00?style=for-the-badge&logo=tensorflow) ![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python) ![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

## 🌍 The Mission
Proper waste segregation is a critical step in recycling and waste management. This project leverages the power of **Deep Learning** and **Computer Vision** to automate the classification of waste into two distinct categories: **Organic (O)** and **Recyclable (R)**. By accurately identifying waste types, we can streamline recycling processes and contribute to a cleaner planet.

---

## 🧠 Project Overview
This project is contained within a Jupyter Notebook (`Final_Project_DL.ipynb`) that orchestrates the entire machine learning pipeline, from data acquisition to prediction.

### Key Features
* **⚡ Automated Data Pipeline:** Automatically downloads and extracts the dataset (`o-vs-r-split-reduced-1200`) directly within the notebook.
* **🔄 Robust Preprocessing:** Utilizes `ImageDataGenerator` for data augmentation (rotation, shear, zoom, flips) to prevent overfitting and improve model generalization.
* **🏗️ Advanced Architecture:** Built using **TensorFlow/Keras**, leveraging powerful CNN architectures for image classification.
* **📊 Visualization:** Includes matplotlib integration to visualize training data and model performance.

---

## 🛠️ Tech Stack & Dependencies
To run this project, you will need the following libraries:

* **Core:** `numpy`, `os`, `shutil`
* **Deep Learning:** `tensorflow`, `keras`
* **Data Processing:** `sklearn` (scikit-learn)
* **Visualization:** `matplotlib`
* **Utilities:** `requests`, `zipfile`, `tqdm` (for progress bars)

---

## 🚀 Getting Started

### 1. Clone & Setup
Ensure you have Python installed. You can install the required dependencies using pip:

```bash
pip install tensorflow numpy matplotlib scikit-learn tqdm requests
```

### 2. Run the Notebook
Open the project file in your preferred environment (Jupyter Lab, Google Colab, or VS Code):

```bash
jupyter notebook Final_Project_DL.ipynb
```

### 3. Execution Flow
#### 1. The notebook is structured to run sequentially:

#### 2.Environment Setup: Verifies TensorFlow version and imports libraries.

#### 3.Data Acquisition: Downloads the specific Organic vs. Recyclable dataset from the cloud.

#### 4.Data Extraction: Unzips the dataset with a visual progress bar.

#### 5.Preprocessing: Configured to resize images to 150x150 pixels and apply augmentation strategies like rotation and horizontal flipping.

#### 6.Model Training: Follow the notebook cells to train the classifier.

## 📁 Data Structure

#### The project expects (and automatically creates) the following directory structure:

```plaintext
o-vs-r-split/
├── train/    # Training images (Organic & Recyclable)
└── test/     # Testing/Validation images
```
#### Classes (Binary Classification)

O : Organic Waste

R : Recyclable Waste
