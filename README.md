# Thesis
The User Based E-Recommender System for small businesses
# 📦 eRecomm: Hybrid Recommender System using UCI Online Retail Dataset

This repository contains a hybrid recommender system framework built using the UCI Online Retail dataset. The system integrates **Association Rule Mining**, **Graph-Based Collaborative Filtering**, and **Q-Learning Reinforcement Learning** into a unified architecture named **RGR Model** (Rules, Graphs, Reinforcement).

## 🚀 Features

- Load and preprocess UCI Online Retail dataset (`.csv` / `.xlsx`)
- Detailed data cleaning and quality reporting
- Transaction basket creation & user-item matrix generation
- Association Rule Mining using `mlxtend`
- Graph-based collaborative filtering using NetworkX
- Reinforcement learning with a Q-table architecture
- Visual performance tracking (precision, recall, F1-score, coverage)
- Model saving/loading using `pickle`
- Extensive plotting and analytics

## 🧠 Architecture

**RGR Hybrid Recommendation Model** includes:

1. **Association Rules** (`Apriori`)  
2. **Graph-Based Filtering** (`networkx` bipartite graphs)  
3. **Reinforcement Learning** (`Q-Learning` with exploration/exploitation)  

Combines predictions from all three with configurable weights to produce top-N recommendations.

## 📂 Project Structure

```bash
.
├── erecomm_UCI_2.py     # Core functions: preprocessing, association rules, graphs, Q-learning
├── erecomm_UCI_3.py     # RGRModelTrainer class: encapsulated training/testing routines
├── data/                # Place your input dataset (Online Retail) here
├── models/              # Saved models via pickle
└── README.md            # Project documentation
