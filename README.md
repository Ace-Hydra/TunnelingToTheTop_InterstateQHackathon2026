# Tunneling to the Top

A quantum machine learning project submitted to the 2026 Interstate Quantum Hackathon. The project explores whether quantum classifiers can outperform a classical baseline for orbital debris classification using a compact feature set derived from satellite object data.

## Team

- Molly O'Donnell
- Alexander Dorozynski
- Siam Arafat Saad
- Bibek Shrestha

## Overview

This repository contains a Jupyter notebook that:

- loads and preprocesses orbital debris data,
- trains several quantum and classical machine learning models,
- compares their validation and test accuracy,
- visualizes the performance of the different approaches.

The primary notebook is:

- `QuantumHackathon_TunnelingToTheTop.ipynb`

Additional project artifacts include:

- `InterstateQHackathon_TunnelingToTheTop_Report.pdf` — project report
- `SpaceDebris_PartOne.csv.csv` — dataset fragment
- `SpaceDebris_PartTwo.csv.csv` — dataset fragment

## Problem Statement

The task is to classify space objects using features such as:

- inclination,
- eccentricity,
- mean motion,
- B* coefficient,
- object type label.

The notebook compares a quantum support vector classifier (QSVC), a variational quantum classifier (VQC), and a classical SVM to assess whether quantum machine learning offers a practical advantage for this classification problem.

## Methods

The workflow implemented in the notebook includes:

1. Data upload and preprocessing
2. Train/validation/test splitting with stratification
3. Min-max scaling for quantum feature encoding
4. Feature map creation using a ZZ feature map
5. Training of:
   - QSVC using Qiskit quantum kernels
   - VQC using RealAmplitudes and SPSA optimization
   - classical SVM baseline
6. Performance comparison and plotting

## Technologies Used

- Python
- Jupyter Notebook
- Qiskit
- qiskit-machine-learning
- qiskit-algorithms
- scikit-learn
- pandas
- NumPy
- Matplotlib

## Repository Structure

```text
.
├── QuantumHackathon_TunnelingToTheTop.ipynb
├── InterstateQHackathon_TunnelingToTheTop_Report.pdf
├── SpaceDebris_PartOne.csv.csv
├── SpaceDebris_PartTwo.csv.csv
└── README.md
