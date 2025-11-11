# ✈️ Customer Segmentation : EastWest Airlines Clustering Project

This project focuses on **unsupervised learning techniques** to segment EastWest Airlines customers based on their flight behavior and loyalty metrics.  
We apply **K-Means, Hierarchical, and DBSCAN clustering** to uncover hidden customer groups that can help the airline design better loyalty programs and marketing strategies.

---

## 🎯 Objective
To perform **customer segmentation** and discover natural groupings in the EastWest Airlines dataset using different clustering techniques.

---

## 🧰 Tools & Libraries
- Python 🐍  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Scipy  

---

## 🧩 Project Workflow

### 1️. Data Loading & Cleaning
- Loaded data from `EastWestAirlines.xlsx`
- Removed irrelevant columns like `ID#`
- Handled missing values using median imputation
- Treated outliers using **IQR method** to improve model stability

### 2️. Feature Scaling
Standardized all numerical features using **StandardScaler** for uniform scaling before clustering.

### 3️. Exploratory Data Analysis (EDA)
- Statistical summary and data overview  
- Correlation heatmap  
- Histograms of customer attributes  
- Detected feature relationships and value ranges  

---

## 🤖 Clustering Techniques Applied

### 🔹 K-Means Clustering
- Used **Elbow Method** to find optimal K (≈5 clusters)
- Evaluated using **Silhouette Score**
- Visualized cluster separation in 2D space  

### 🔹 Hierarchical Clustering
- Applied **Ward linkage** and visualized with a **Dendrogram**
- Defined 5 clusters from dendrogram cut
- Compared silhouette with K-Means results  

### 🔹 DBSCAN (Density-Based)
- Identified dense clusters and noise points  
- Tuned `eps` and `min_samples` for meaningful clusters  
- Compared silhouette performance  

---

## 📈 Evaluation Metrics
| Algorithm | Silhouette Score |
|------------|------------------|
| K-Means | ~0.45 |
| Hierarchical | ~0.42 |
| DBSCAN | Depends on parameters |

*(Replace with your actual output values)*  

---

## 🎨 Visualization Highlights
- Elbow Curve for optimal K  
- Dendrogram for Hierarchical structure  
- Scatter plots of clusters in feature space  
- Heatmap of feature correlations  

---

## 💡 Business Insights
✅ K-Means formed well-separated customer clusters.  
✅ Hierarchical clustering confirmed similar grouping patterns.  
✅ DBSCAN detected dense frequent-flyer segments and noise points.  
✅ Frequent travelers tend to have **higher mileage and loyalty points**.  
✅ Different customer segments can guide **targeted marketing and loyalty rewards**.

---

## 💾 Output Files
- `Clustering_Results_EastWestAirlines.csv` → contains cluster labels for each customer  
- Visuals for K-Means, Hierarchical, and DBSCAN results  

---

## 🚀 Future Enhancements
- Perform **PCA for dimensionality reduction**  
- Use **K-Prototypes** for mixed-type datasets  
- Build an **interactive dashboard** for cluster exploration  

---
