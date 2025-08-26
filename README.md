# Mall-Customer-Segmentation
# Customer Segmentation using Clustering

## Project Overview
# This project applies unsupervised machine learning to segment mall customers.
# Algorithms used: K-Means, Hierarchical Clustering, DBSCAN.
# Goal: Group customers based on Age, Income, and SpendingScore for business insights.

---

## Dataset
# Features:
# - Age: Customer's age
# - Income: Annual income
# - SpendingScore: Score (1–100) representing spending habits
# Total Customers: 200

---

## Algorithms Used

###K-Means
# - Found optimal clusters using Elbow Method & Silhouette Score
# - Final clusters = 5
# - Best interpretability among all methods

##Hierarchical Clustering
# - Used Ward linkage with Euclidean distance
# - Visualized clusters with dendrogram
# - Similar to K-Means results

### 3️⃣ DBSCAN
# - Density-based clustering
# - Handles noise/outliers (labeled as -1)
# - Fewer stable clusters compared to K-Means

---

## 📈 K-Means Cluster Profiles
# Cluster | Avg Age | Avg Income | Avg SpendingScore | Count | Label
#   0     |   46.2  |    26.7    |        18.3       |  20   | Low-income Conservative Spenders
#   1     |   25.2  |    41.1    |        62.2       |  54   | Young High Spenders
#   2     |   32.9  |    86.1    |        81.5       |  40   | Affluent Big Spenders
#   3     |   39.9  |    86.1    |        19.4       |  39   | Wealthy Conservative Spenders
#   4     |   55.6  |    54.4    |        48.9       |  47   | Older Average Spenders

---

## Evaluation
# - Silhouette Score → Checked cluster quality
# - Adjusted Rand Index (ARI) → Compared K-Means & Hierarchical
# - DBSCAN → Detected noise & outliers

---

## How to Run
```bash
# Step 1: Clone repository
git clone https://github.com/kumar-kiran-24/customer-segmentation.git
cd customer-segmentation

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Run analysis
jupyter notebook  # OR python clustering.py
