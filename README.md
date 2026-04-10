# Hybrid E-commerce Intelligence System with A* Search and Contextual Bandit Orchestration

## Description
intelligent e-commerce recommendation system that uses A* search to efficiently navigate product categories and find relevant items. It combines unsupervised clustering (K-Means), collaborative filtering (KNN), and a Random Forest classifier for purchase prediction, while a Contextual Bandit (simplified reinforcement learning) dynamically decides which recommendation strategy to show each user for maximum engagement.

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
