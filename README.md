# 🏡 Exploring Airbnb Listings in Lisbon: A Data-Driven Analysis

This project presents a comprehensive analysis of Airbnb listings in Lisbon, using unsupervised machine learning techniques to uncover market patterns. It was completed as part of the *Programming for Data Science 2024* course by Group B7.

---

## 📌 Overview

The primary objective of this project was to analyze Airbnb data in Lisbon to generate insights for **hosts**, **investors**, and **guests**. Using **K-Means clustering**, we identified five distinct rental categories, based on price, room type, location, and rental frequency.

---

## 🎯 Objectives

- Understand pricing and availability trends in the Lisbon Airbnb market.
- Segment the market using **unsupervised learning** (K-Means, DBSCAN, PCA + K-Means).
- Provide actionable insights and strategies for each identified cluster.

---

## 📊 Methodology

1. **Data Collection**  
   - Source: `listings.csv` from Inside Airbnb – Lisbon.
   - Rows: 22,929  
   - Columns: 18 (numerical + categorical)

2. **Preprocessing**
   - Outlier removal (e.g., prices > €2000)
   - Missing value imputation using **KNN Imputer**
   - Feature engineering (`host_info`, normalized variables)

3. **Clustering Techniques Tested**
   - ✅ **K-Means** – final choice for its interpretability and balance
   - 🧪 DBSCAN – strong with outliers, but performed poorly
   - 🔄 K-Means after PCA – dimensionality reduction, but less interpretable

4. **Cluster Evaluation**
   - **Elbow Method**
   - **Silhouette Score**

---

## 🧠 Final Clusters Identified

| Cluster | Label                   | Avg. Price | Key Traits |
|--------:|-------------------------|-----------:|------------|
| 0       | Luxury Rentals          | €652       | High-end homes in elite areas, low frequency |
| 1       | Standard Rentals        | €106       | Most common type, good for families/business |
| 2       | Budget-Friendly Rentals | €96        | Short stays, high reviews/month, high demand |
| 3       | Corporate Housing       | €107       | Longer stays, business travelers, 13-night avg |
| 4       | Extended Stay Rentals   | €134       | ~269-night avg, ideal for expats/relocations |

---

## 📌 Key Technologies

- **Python**
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `plotly`
- **Algorithms**
  - K-Means (main)
  - DBSCAN (tested)
  - PCA + K-Means (tested)
- **Data Preprocessing**
  - `StandardScaler`, `KNNImputer`, outlier handling

---

## 🖼️ Visual Insights

Clusters were visualized by:
- Price distribution
- Room type
- Neighborhood
- Host activity

> Visualizations were created using `matplotlib`, `seaborn`, and `plotly` for better interpretability.

---

## 💡 Recommendations by Cluster

- **Luxury Rentals**: Partner with luxury travel agencies.
- **Standard Rentals**: Promote through local tourism & business platforms.
- **Budget-Friendly**: Encourage guest reviews; advertise on budget platforms.
- **Corporate Housing**: Offer high-speed WiFi, flexible check-in/out; partner with companies.
- **Extended Stay**: Provide long-stay discounts and flexible lease options.

---

## 👥 Team & Contributions

**Group B7**:  
- Baran Can Çelik  
- Carlos Eduardo Nunes Lourenço  
- Priyá Dessai  
- Raysa Rocha  

> Raysa and Priyá focused on the Jupyter notebook; Carlos and Baran on the report. All members contributed to the final presentation.

---

## 🧾 References

- McKinney (2010), *Data Structures for Statistical Computing in Python*
- Pedregosa et al. (2011), *Scikit-learn: Machine Learning in Python*
- Harris et al. (2020), *NumPy*
- Hunter (2007), *Matplotlib*
- Waskom (2021), *Seaborn*
- Plotly Technologies Inc. (2015)
- VanderPlas (2016), *Python Data Science Handbook*

---

## 📜 License

This project was developed as part of an academic assignment. Feel free to explore or adapt the analysis with credit to the authors.

---

## 🙋‍♀️ Questions?

Feel free to reach out or open an issue if you'd like to discuss any part of the analysis!
