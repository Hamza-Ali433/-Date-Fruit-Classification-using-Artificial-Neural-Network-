 Date Fruit Classification using Artificial Neural Network (PyTorch)

## Overview

This project demonstrates a multiclass classification problem using an Artificial Neural Network (ANN) implemented with PyTorch. The objective is to classify different varieties of date fruits based on their physical and texture-related characteristics. The project covers the complete deep learning pipeline, from data preprocessing to model training and evaluation.

---

## Dataset Information

The dataset contains **898 samples** and **34 numerical features** describing the physical properties of date fruits. The target variable consists of **7 different date varieties**.

### Date Classes

- BERHI
- DEGLET
- DOKOL
- IRAQI
- ROTANA
- SAFAVI
- SOGAYI

### Features

The dataset includes measurements such as:

- Area
- Perimeter
- Major Axis
- Minor Axis
- Eccentricity
- Solidity
- Convex Area
- Extent
- Aspect Ratio
- Roundness
- Compactness
- ShapeFactor_1
- ShapeFactor_2
- ShapeFactor_3
- ShapeFactor_4
- MeanRR
- MeanRG
- MeanRB
- StdDevRR
- StdDevRG
- StdDevRB
- SkewRR
- SkewRG
- SkewRB
- KurtosisRR
- KurtosisRG
- KurtosisRB
- EntropyRR
- EntropyRG
- EntropyRB
- ALLdaub4RR
- ALLdaub4RG
- ALLdaub4RB

---

## Project Workflow

- Import required libraries
- Load the dataset
- Explore and understand the data
- Encode class labels
- Split the dataset into training and testing sets
- Standardize feature values
- Convert data into PyTorch tensors
- Create DataLoaders
- Build an Artificial Neural Network
- Train the model
- Evaluate model performance
- Predict unseen samples

---

## Neural Network Architecture

```
Input Layer (34 Features)
        │
        ▼
Linear Layer (64 Neurons)
        │
      ReLU
        │
        ▼
Linear Layer (64 Neurons)
        │
      ReLU
        │
        ▼
Output Layer (7 Classes)
```

---

## Technologies Used

- Python
- PyTorch
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Model Configuration

| Parameter | Value |
|-----------|-------|
| Hidden Layers | 2 |
| Hidden Neurons | 64 |
| Activation Function | ReLU |
| Loss Function | CrossEntropyLoss |
| Optimizer | Adam |
| Epochs | 100 |

---

## Model Performance

**Classification Accuracy**

**94.44%**

The trained ANN successfully classified the seven date fruit varieties with an overall accuracy of approximately **94.44%** on the test dataset.

---

## Project Structure

```
Date-Fruit-Classification-ANN/
│
├── ANN_Classifier.ipynb
├── Date_Fruit_Dataset.csv
├── README.md
└── requirements.txt
```

---

## How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/Date-Fruit-Classification-ANN.git
```

2. Open the project folder

```bash
cd Date-Fruit-Classification-ANN
```

3. Install the required libraries

```bash
pip install -r requirements.txt
```

4. Run the Jupyter Notebook

```bash
jupyter notebook
```

Open **ANN_Classifier.ipynb** and execute all cells.

---

## What I Learned

During this project I gained practical experience with:

- Building neural networks using PyTorch
- Data preprocessing for deep learning
- Feature scaling
- Label encoding
- Creating custom ANN models
- Working with DataLoaders
- Training neural networks using mini-batches
- Using the Adam optimizer
- Evaluating multiclass classification models

---


---

## Conclusion

This project demonstrates how an Artificial Neural Network can effectively solve a multiclass classification problem using PyTorch. By combining proper data preprocessing, feature scaling, and a simple feed-forward neural network, the model achieved an accuracy of **94.44%**. The project served as valuable hands-on practice in implementing deep learning models and understanding the complete workflow from raw data to prediction.
