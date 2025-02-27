# Part A: Decentralization TD3 Workshop

This directory contains the implementation for a Data Redundancy and Distributed Computing Workshop, demonstrating decentralized prediction systems using multiple machine learning models.

## Objectives
- Understand distributed and decentralized computing principles.
- Build and integrate multiple predictive models.
- Implement a consensus mechanism with weighting and slashing for reliability.

## Files
- **`model1.py`**: Logistic Regression model running on port 5001.
- **`model2.py`**: Decision Tree model running on port 5002.
- **`model3.py`**: K-Nearest Neighbors (KNN) model running on port 5003.
- **`consensus.py`**: Combines predictions from all models, applies weighting and slashing, and updates `model_db.json`.
- **`model_db.json`**: JSON database tracking model weights, balances, and URLs.

## Setup
1. **Install Dependencies**: 
   ```bash
   pip install scikit-learn flask pyngrok requests numpy
