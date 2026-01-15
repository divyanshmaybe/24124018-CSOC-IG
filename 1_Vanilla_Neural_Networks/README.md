# Vanilla Neural Networks: Medical Appointment No-Show Prediction

This project implements a custom neural network from scratch to predict medical appointment no-shows using the Kaggle medical appointment dataset.

## Overview

The notebook demonstrates a complete machine learning pipeline:
- Data preprocessing and feature engineering
- Custom neural network implementation with forward and backward propagation
- Handling class imbalance with weighted loss functions
- Model evaluation and threshold tuning

## Dataset

The dataset (`KaggleV2-May-2016.csv`) contains information about medical appointments and whether patients showed up or not. It includes features like:
- Patient demographics (age, gender)
- Appointment scheduling details
- Medical history indicators
- Neighborhood information

**Note**: The dataset is not included in this repository. Download it from [Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments) and place it in this directory.

## Neural Network Architecture

- **Input Layer**: Features after preprocessing and encoding
- **Hidden Layers**: 2 hidden layers with 3 neurons each
- **Output Layer**: Single neuron with sigmoid activation
- **Loss Function**: Binary Cross-Entropy with class weighting
- **Optimization**: Custom gradient descent with learning rate decay

## Key Features

### Data Preprocessing
- Feature selection (removing irrelevant columns)
- Label encoding for target variable
- One-hot encoding for categorical features
- Feature scaling (StandardScaler on age)

### Custom Implementation
- Manual forward propagation
- Manual backward propagation
- Mini-batch gradient descent
- Class-weighted loss for imbalanced dataset

### Evaluation
- Train/test accuracy and F1-score
- Confusion matrix analysis
- Threshold tuning for optimal performance
- Training loss visualization

## Usage

1. Ensure you have the dataset file in this directory
2. Install required packages: `pip install -r ../requirements.txt`
3. Open `ex.ipynb` in Jupyter Lab
4. Run all cells sequentially

## Results

The model achieves reasonable performance on the imbalanced dataset through:
- Class weighting to handle minority class (no-shows)
- Threshold adjustment for better precision/recall balance
- Learning rate scheduling for stable convergence

## Files

- `ex.ipynb`: Main implementation notebook
- `report.pdf`: Detailed project report
- `KaggleV2-May-2016.csv`: Dataset (not included - download separately)

## Dependencies

- numpy
- pandas
- scikit-learn
- matplotlib
- ydata-profiling
- jupyter

## Author

Divyansh Soni (Roll Number: 24124018)
