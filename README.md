# Drug_discovery_GenAI






# Ligand Activity Classification and Molecular Generation

This repository contains a complete machine learning pipeline for predicting ligand activity against the AChE protein using XGBoost and generating novel molecular structures using a Variational Autoencoder (VAE). It includes data preprocessing, model training, molecule generation, visualization, and evaluation.

---

## 🧠 Project Goals

- **Classify ligands** as active or inactive based on molecular descriptors.
- **Generate new ligands** using a VAE trained on SMILES representations.
- **Evaluate** the generated ligands based on chemical similarity and visual distribution (PCA).

---

## 📁 Directory Structure

Drug_discovery_project/
├── AChE_dataset/
│   ├── AChE_ligands_csv.csv              # Raw dataset with ligand data
│   └── dataset_with_descriptors.csv      # Descriptor-enhanced dataset
│
├── classification model_XGBOOST/
│   ├── classification task.ipynb         # Notebook for classification task
│   └── xgboost_AChE_model_classification.pkl  # Trained model
│
├── VAE model for generation/
│   ├── VAE smile generation.ipynb        # Notebook for molecule generation
│   ├── simple_smiles_vae.pt              # Trained VAE model
│   └── vae_training_loss.png             # VAE training loss visualization
│
├── generated_active_smiles.csv           # Output of generated molecules
├── Tanimoto similarity.png               # Chemical similarity comparison
├── PCA analysis for generated and original active smiles.png  # PCA visual
└── report.pdf                            # Final project report


---

## 📊 Models Used

### 🔹 XGBoost Classifier

- **Goal:** Predict ligand activity.
- **Input:** Molecular descriptors.
- **Output:** Binary classification (active/inactive).
- **Performance Metrics:** Accuracy, precision, recall (see notebook for results).

### 🔹 Variational Autoencoder (VAE)

- **Goal:** Generate novel SMILES strings similar to actives.
- **Input:** SMILES of active ligands.
- **Output:** New SMILES strings.
- **Evaluation:** Tanimoto similarity + PCA visualization.

---

## 🔧 Installation & Requirements

Ensure the following Python libraries are installed:

bash
pip install numpy pandas scikit-learn xgboost rdkit-pypi matplotlib seaborn torch


---

## ▶️ How to Run


1. Open and run the notebooks:
   - classification model_XGBOOST/classification task.ipynb
   - VAE model for generation/VAE smile generation.ipynb

---

## 📌 Visual Results

### PCA Distribution
![PCA](PCA%20analysis%20for%20generated%20and%20original%20active%20smiles.png)

### Tanimoto Similarity
![Tanimoto](Tanimoto%20similarity.png)

---

## 🧬 Key Technologies

- **Languages:** Python
- **Libraries:** XGBoost, PyTorch, RDKit, Scikit-learn, Matplotlib
- **ML Concepts:** Supervised classification, autoencoders, chemical similarity

---

## 📄 Report

A complete explanation of the methods and outcomes can be found in the [project report](report.pdf).

---

## 🤝 Acknowledgements

This project was developed as part of a machine learning initiative focused on ligand-based drug modeling and generative chemistry.  rewrite in huamna form 

Ligand Activity Classification and Molecular Generation
This project focuses on predicting whether ligands are active against the AChE protein and generating new molecular structures using deep learning techniques. The workflow combines machine learning for activity prediction with a Variational Autoencoder (VAE) for molecular generation. It also includes visualization and evaluation of the generated compounds.

🧠 Project Overview
The main objectives of this project are:

To classify ligands as active or inactive using molecular descriptors.

To generate new ligand structures from SMILES representations using a VAE model.

To evaluate generated molecules using similarity analysis and PCA visualization.

📁 Project Structure
Drug_discovery_project/
├── AChE_dataset/
│   ├── AChE_ligands_csv.csv
│   └── dataset_with_descriptors.csv
│
├── classification model_XGBOOST/
│   ├── classification task.ipynb
│   └── xgboost_AChE_model_classification.pkl
│
├── VAE model for generation/
│   ├── VAE smile generation.ipynb
│   ├── simple_smiles_vae.pt
│   └── vae_training_loss.png
│
├── generated_active_smiles.csv
├── Tanimoto similarity.png
├── PCA analysis for generated and original active smiles.png
└── report.pdf
📊 Models and Methods
XGBoost Classification Model
The XGBoost model is used to predict ligand activity based on molecular descriptors.

Input: Molecular descriptor features

Output: Active or inactive ligand prediction

Purpose: Identify compounds with potential biological activity against AChE

The model performance is evaluated using standard classification metrics such as accuracy, precision, and recall.

Variational Autoencoder (VAE)
A Variational Autoencoder was trained on active ligand SMILES strings to generate new molecular structures.

Input: SMILES representations of active ligands

Output: Newly generated SMILES strings

Purpose: Explore and create novel compounds similar to known active molecules

The generated molecules were analyzed using:

Tanimoto similarity for chemical similarity comparison

PCA visualization to compare the distribution of original and generated molecules

🔧 Installation
Install the required Python libraries before running the project:

pip install numpy pandas scikit-learn xgboost rdkit-pypi matplotlib seaborn torch
▶️ Running the Project
Run the following notebooks step by step:

Classification model notebook:

classification model_XGBOOST/classification task.ipynb
Molecular generation notebook:

VAE model for generation/VAE smile generation.ipynb
📌 Results and Visualizations
PCA Analysis
The PCA plot compares the distribution of generated molecules with the original active ligands.

Tanimoto Similarity
Tanimoto similarity analysis measures how chemically similar the generated molecules are to known active compounds.

🧬 Technologies Used
Programming Language: Python

Machine Learning: XGBoost, Scikit-learn

Deep Learning: PyTorch

Cheminformatics: RDKit

Visualization: Matplotlib, Seaborn

📄 Project Report
A detailed explanation of the methodology, experiments, and results is available in the project report included in this repository.

🤝 Acknowledgements
This project was developed as part of a machine learning and drug discovery study focused on ligand activity prediction and generative molecular modeling.



Voice
