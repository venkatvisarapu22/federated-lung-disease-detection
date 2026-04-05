# 🏥 Federated Multimodal Lung Disease Detection

## 📌 Overview

This project predicts lung disease using a **multimodal deep learning model** trained with **Federated Learning (FL)**.

It combines:

* Chest X-ray images (CNN)
* Clinical data (Age, Gender)

without sharing sensitive patient data across hospitals.

---

## 📊 Dataset Information

This project is based on:

* MIMIC-IV Clinical Database
* MIMIC-CXR Dataset

⚠️ **Important Notice:**
The original datasets are NOT included due to access restrictions.

To use full dataset:

1. Complete PhysioNet credentialed access course
2. Request access
3. Download dataset from:
   https://physionet.org/

---

## 📂 Included Data

This repository contains:

* Processed subset (600 patients)
* Hospital-wise split datasets

---

## 🧠 Model Architecture

* CNN → Extract image features
* Fully Connected → Clinical features
* Fusion Layer → Combine both
* Sigmoid → Binary classification

---

## 🌐 Federated Learning

* 3 hospitals simulated
* Algorithm: Federated Averaging (FedAvg)
* Training rounds: 10

---

## 📈 Results

* Accuracy: ~80%
* F1 Score: ~0.78
* ROC AUC: ~0.88

---

## 📊 Evaluation

* Confusion Matrix
* ROC Curve
* Precision, Recall, F1 Score

---

## 💾 Pretrained Model

Download model from Google Drive:

👉 [PASTE YOUR DRIVE LINK HERE]

After downloading:

1. Place file inside project folder
2. Rename as:

```
federated_lung_model.pth
```

---

## 🚀 How to Run

### Step 1: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 2: Run notebook

```bash
jupyter notebook
```

### Step 3: Execute all cells

---

## 🔮 Future Work

* Add clinical text using BERT
* Add genomic data
* Improve dataset size

---
## ⚡ Quick Run (Using Pretrained Model)

If you do not want to retrain the model:

1. Download the pretrained model from Google Drive
2. Place it in the project root directory
3. Rename it as:

```
federated_lung_model.pth
```

4. Open the notebook and run the cells sequentially 

The notebook is designed to:

* Automatically load the saved model
* Skip training if the model file is found
* Directly show evaluation results

This allows quick testing without long training time.
