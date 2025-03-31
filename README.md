# Assignment 4 – Federated Learning Algorithm Implementation

This repository contains the notebook for **Assignment 4**, focusing on implementing and analyzing Federated Learning (FL) algorithms. It builds upon the previous assignment and aims to simulate real-world FL scenarios with decentralized data from multiple nodes (weather stations).

## 📁 Files

- `Assignment_4_FLAlgorithm.ipynb`: Main Jupyter notebook implementing FL algorithms, data processing, and result analysis.
- `FMI_data_2025.csv`: Dataset used for training and evaluation (assumed to be in the same directory).

## 📊 Dataset Overview

The dataset includes weather station data with the following features:

- `Name`: Identifier for the station (acts as a node)
- `Latitude`, `Longitude`: Geographic coordinates
- `Tmax`, `Tmin`: Maximum and minimum temperatures over the past 5 days (input features)
- `y_Tmax`: Maximum temperature on day 6 (target label)
- `y_Tmin`: Minimum temperature on day 6 (optional target)

Each row represents a 6-day temperature sequence for one station. The learning task is to predict `y_Tmax` using the past 5 days' `Tmax` and `Tmin`.

## 🧠 Objective

The primary goal of this notebook is to:

- Simulate a Federated Learning setup
- Train local models on client (station) data
- Aggregate local updates using techniques like Federated Averaging (FedAvg)
- Compare FL performance to centralized training

## ⚙️ Technologies Used

- Python  
- Jupyter Notebook  
- NumPy & Pandas  
- PyTorch or TensorFlow (depending on your code)
- NetworkX (for graph-based relationships)
- Custom implementation of FL aggregation

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# 2. Install dependencies
pip install -r requirements.txt

# 3. Start Jupyter Notebook
jupyter notebook

# 4. Open and run the notebook
# File: Assignment_4_FLAlgorithm.ipynb
