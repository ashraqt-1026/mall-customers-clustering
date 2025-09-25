# Mall Customers Clustering

## 📌 Overview
This project applies **K-Means clustering** to the [Mall Customers dataset](https://www.kaggle.com/datasets/shwetabh123/mall-customers), with the goal of segmenting customers into distinct groups based on their demographics and spending habits.  
Customer segmentation is a useful technique for marketing teams to identify **VIPs, budget-conscious customers, or high-spending youth**, and adapt business strategies accordingly.

---

## 📊 Dataset
The dataset contains **200 entries**, with the following features:

- `CustomerID` → Unique customer identifier  
- `Genre` → Gender (Male/Female)  
- `Age` → Customer age  
- `Annual Income (k$)` → Annual income in thousands of dollars  
- `Spending Score (1-100)` → Score assigned by the mall based on spending patterns  

---

## ⚙️ Steps Performed
1. **Data Exploration (EDA)**  
   - Checked dataset shape, null values, and summary statistics.  
   - Plotted distributions of Age, Income, and Spending Score.  

2. **Feature Selection**  
   - Chose key features for clustering:  
     - `Annual Income (k$)`  
     - `Spending Score (1-100)`  
     - Age and Gender also used in interpretation.  

3. **Clustering with K-Means**  
   - Used the **Elbow Method** to determine the optimal number of clusters (`k = 4`).  
   - Applied KMeans and assigned cluster labels to each customer.  

4. **Evaluation & Visualization**  
   - Plotted clusters in 2D (Income vs Spending Score).  
   - Calculated mean values of each feature per cluster for interpretation.  

---

## 📈 Results & Interpretation
Based on the clustering results:

- **Cluster 0** → Older customers, medium income, low spending → **Budget-conscious**  
- **Cluster 1** → Older males, medium income, low spending → **Conservative spenders**  
- **Cluster 2** → Young males, medium income, high spending → **High-spending youth (Extravagant)**  
- **Cluster 3** → Young females, medium income, very high spending → **VIP / High-spenders**  

---

## 🛠️ Tech Stack
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---
