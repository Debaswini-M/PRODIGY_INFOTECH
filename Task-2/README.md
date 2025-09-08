# 🛒 Customer Segmentation using K-Means Clustering

## 📌 Task Description  
**Task 2:** Create a K-means clustering algorithm to group customers of a retail store based on their purchase history.

Dataset: [Kaggle - Customer Segmentation Tutorial](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

---

## ⚙️ Steps Followed

### 1. Importing Libraries
- `pandas`, `numpy` for data handling  
- `matplotlib`, `seaborn` for visualization  
- `scikit-learn` for preprocessing, clustering, and evaluation  

### 2. Data Preparation
- Selected important features: **Age, Annual Income, Spending Score**  
- Scaled features using **StandardScaler**  

### 3. Finding Optimal Clusters
- Used **Elbow Method (WCSS)** to visualize the optimal number of clusters  
- Validated with **Silhouette Score** (best clustering performance at **k=5**)  

### 4. K-Means Clustering
- Applied **KMeans** with `k=5`  
- Assigned cluster labels to each customer  

### 5. Visualization
- **Elbow Method Plot** → shows optimal `k`  
- **Silhouette Scores** → ensured cluster quality  
- **Scatter Plot (Annual Income vs Spending Score)** → customer groups with centroids  
- **Cluster Summary Table** → average Age, Income, and Spending Score per cluster
- **Cluster Profile Heatmap** → summarized differences across clusters   

---

## 📊 Results & Insights

### Cluster Profiling (Means)
| Cluster | Age  | Annual Income (k$) | Spending Score (1–100) | Interpretation |
|---------|------|--------------------|-------------------------|----------------|
| **0** | 46.2 | 26.8 | 18.4 | Older, low income, low spenders |
| **1** | 25.2 | 41.1 | 62.2 | Young, lower-mid income, high spenders |
| **2** | 32.9 | 86.1 | 81.5 | Premium customers (high income & high spending) |
| **3** | 39.9 | 86.1 | 19.4 | Wealthy but low spending (disengaged) |
| **4** | 55.6 | 54.4 | 48.9 | Mature, mid income, moderate spenders |

---

## 📝 Conclusion
- The dataset of mall customers was successfully segmented into **5 meaningful clusters**:  
  - **Cluster 0 → Budget-conscious, low spenders**  
    - Older customers, low income, and low spending.  
    - Likely price-sensitive → can be engaged with discounts or budget-friendly offers.  

  - **Cluster 1 → Young aspirers**  
    - Younger customers with moderate income and high spending scores.  
    - Represent a **growing customer base** → can be targeted with lifestyle products and trend-based campaigns.  

  - **Cluster 2 → Premium/VIP customers**  
    - High income and very high spending score.  
    - These are **loyal, high-value customers** → should be retained with loyalty programs, personalized services, and exclusive deals.  

  - **Cluster 3 → Affluent but disengaged**  
    - High income but very low spending scores.  
    - This segment is **wealthy but not engaged** with the mall → they need reactivation through personalized marketing, premium services, or exclusive events.  

  - **Cluster 4 → Mature mid-range spenders**  
    - Older age group, mid income, and average spending.  
    - Can be targeted with **family-oriented or practical offers**.  

- **Key Takeaways for the Business**:  
  - The **most profitable clusters** are **Cluster 2 (VIPs)** and **Cluster 1 (Young aspirers)** → invest in retention & engagement.  
  - **Cluster 3** shows **lost opportunities** (wealthy but low spending) → they are a potential growth segment if properly targeted.  
  - **Cluster 0** customers are unlikely to contribute much revenue → keep them engaged with basic offers, but don’t over-invest.  
  - Segmentation shows that **one-size-fits-all marketing won’t work**. Instead, tailored strategies can maximize customer satisfaction and mall revenue.   

---

## 🚀 Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 👩🏻‍💻 Author
` Debaswini`

