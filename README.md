# CSOC-IG: Machine Learning Projects

This repository contains machine learning projects developed as part of the CSOC-IG coursework. It includes implementations of neural networks and reinforcement learning algorithms.

## Projects

### 1. Vanilla Neural Networks
**Location:** `1_Vanilla_Neural_Networks/`

This project implements a custom neural network from scratch for predicting medical appointment no-shows using the Kaggle medical appointment dataset.

**Key Features:**
- Custom neural network implementation with forward and backward propagation
- Class imbalance handling using weighted loss functions
- Data preprocessing and feature engineering
- Model evaluation with accuracy, F1-score, and confusion matrix

**Files:**
- `ex.ipynb`: Main implementation notebook
- `KaggleV2-May-2016.csv`: Dataset (not included in repo - download from Kaggle)
- `report.pdf`: Project report

### 2. Reinforcement Learning
**Location:** `2_Reinforcement_Learning/`

This project explores various reinforcement learning algorithms on custom environments.

**Week 2 Projects:**

#### Frozen Lake Environment
**Location:** `2_Reinforcement_Learning/Week2/FrozenLake/`

- Custom Frozen Lake environments with different grid sizes
- Implementation of Monte Carlo, SARSA, Q-Learning algorithms
- Model-based methods: Policy Iteration and Value Iteration
- Performance comparison across different algorithms

**Files:**
- `task.ipynb`: Comprehensive RL algorithms implementation
- `rl2.ipynb`: Value and Policy Iteration on custom 8x8 Frozen Lake
- `reinforcement_learning_report.pdf`: Detailed report
- `task_1_and_2_derivation_and_proofs.pdf`: Mathematical derivations

#### Cliff Walking Environment
**Location:** `2_Reinforcement_Learning/Week2/CliffWalking/`

- Custom Cliff Walking environment implementation
- SARSA, Q-Learning, and Double Q-Learning algorithms
- Performance analysis and comparison

**Files:**
- `bonus_task.ipynb`: RL algorithms on Cliff Walking

## Installation

1. Clone the repository:
```bash
git clone https://github.com/divyanshmaybe/24124018-CSOC-IG.git
cd 24124018-CSOC-IG
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## Usage

Each project is contained in its own directory with Jupyter notebooks. Open the notebooks in Jupyter Lab or VS Code to run the code interactively.

For the neural networks project, you'll need to download the dataset from Kaggle and place it in the `1_Vanilla_Neural_Networks/` directory.

## Dependencies

- numpy
- pandas
- scikit-learn
- matplotlib
- gymnasium
- ydata-profiling

## License

This project is part of academic coursework.

## Author

Divyansh Maybe
Roll Number: 24124018
