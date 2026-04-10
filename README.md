# Hybrid E-commerce Intelligence System with A* Search and Contextual Bandit Orchestration

**Course Name:** AL2002 Artificial Intelligence/Machine Learning

## Project Description
This project builds an intelligent e-commerce recommendation system that combines A* search for efficient product navigation with unsupervised clustering, supervised Random Forest prediction, and a Contextual Bandit (simplified RL) to dynamically choose between KNN collaborative filtering and ML-based recommendations. The system segments users via K-Means, predicts purchase probabilities, and optimizes click-through rates without using deep learning or neural networks.

## Project Components

| Component | Technology / Algorithm | Purpose |
|-----------|----------------------|---------|
| Informed Search | A* Algorithm | Find optimal product path from category to target item using heuristic based on purchase probability |
| User Segmentation | K-Means Clustering | Group users into personas (e.g., bargain hunters, impulse buyers) |
| Collaborative Filtering | K-Nearest Neighbors (KNN) | Generate "users who liked this also liked" recommendations |
| Purchase Prediction | Random Forest Classifier | Predict probability of user buying a specific product |
| Strategy Orchestration | Contextual Bandit (LinUCB) | Decide whether to show KNN or Random Forest recommendations to maximize engagement |
| Data Processing | Pandas, NumPy | Clean and transform RetailRocket e-commerce dataset |
| Evaluation | Scikit-learn, Matplotlib | Measure silhouette score, F1-score, cumulative regret, and CTR |

## Dataset
- **Source:** RetailRocket Dataset (Kaggle)
- **Size:** ~2.5 million e-commerce events (views, carts, purchases)
- **Features:** User ID, Item ID, Event type, Timestamp, Price, Category
