# 🛍️ Customer Segmentation using K-Means Clustering

This project applies unsupervised machine learning to segment mall customers. The segmentation is based on two key metrics: **Annual Income (k$)** and **Spending Score (1–100)**. The primary goal is to identify distinct, homogeneous customer groups (clusters) to facilitate better targeted marketing strategies and generate actionable business insights.

---

## ⚙️ Technologies and Libraries Used

* **Python 3.x**
* **Pandas:** For data manipulation and analysis.
* **Matplotlib & Seaborn:** For data visualization.
* **Scikit-learn (sklearn):** For core machine learning tasks.

---

## 📁 Dataset Details

The dataset contains detailed information about mall customers:

| Feature | Description |
| :--- | :--- |
| **Annual Income (k$)** | The customer's annual income in thousands of dollars ($). |
| **Spending Score (1–100)** | A score assigned by the mall based on customer spending behavior. |

> 📂 File used: `Mall_Customers.csv`

---

## 🔧 Steps Performed

1.  **Data Exploration & Cleaning** 🧹
    * Confirmed the absence of missing or null values.
    * Visualized the strong positive linear relationship between Income and Spending Score.

2.  **Feature Preparation** 📏
    * Selected the two numerical features: **Annual Income (k$)** and **Spending Score (1–100)**.
    * Applied **StandardScaler** to normalize the data (Essential for distance-based algorithms like K-Means and DBSCAN).

3.  **Model Selection & Tuning** 📐
    * Used the **Elbow Method** to determine the optimal number of clusters ($k$) for K-Means.
    * Evaluated both the **K-Means** and **DBSCAN** algorithms for clustering.

4.  **Model Training & Evaluation** ⭐
    * Trained the **K-Means** model with the optimal $k$.
    * Used the **Silhouette Score** as a quantitative metric to evaluate the quality of the clusters produced by the models.

5.  **Visualization & Analysis** 🖼️
    * A final 2D scatter plot was generated, visually separating the customers into their respective clusters with the **cluster centroids** highlighted.
    * Characterized the customer segments (e.g., "High Income, Low Spenders").

---

## 📊 Key Visualizations

* 📉 **Elbow Method Plot:** Used to justify the chosen number of clusters ($k$).
* 🎨 **Final Segmentation Plot:** A 2D scatter plot showing the distinct customer segments colored differently.

---

## 📦 Libraries Used

```bash
pandas
matplotlib.pyplot
seaborn
sklearn.preprocessing (StandardScaler)
sklearn.cluster (KMeans, DBSCAN)
sklearn.metrics (silhouette_score)
