
# ✈️ Delta Fleet Analysis Using PCA and KMeans Clustering

## 📌 Overview

This project analyzes aircraft data from Delta Airlines to identify similarities between different planes using unsupervised learning. Principal Component Analysis (PCA) is used to reduce dimensionality, followed by KMeans clustering to group aircraft into distinct segments based on technical features.

## 📁 Dataset

- **Source**: `delta.csv`
- **Content**: The dataset includes numerical features describing each aircraft's technical specifications, such as speed, fuel capacity, range, and engine type.

## ⚙️ Methodology

### 1. Data Preparation
- Dropped non-numerical or identifier columns that do not contribute to clustering.
- Standardized all numerical features using `StandardScaler`.

### 2. Dimensionality Reduction with PCA
- Performed PCA to reduce the number of features to 4 components.
- PCA was used to compress the dataset while preserving as much variance as possible.

### 3. KMeans Clustering
- Applied KMeans clustering on the PCA-transformed data.
- The **Elbow Method** was used to determine that **3 clusters** provided a reasonable balance of model complexity and fit.
- Clusters were assigned to each record in the transformed PCA space.

## 🛠️ Tools Used

- Python 3.x
- Pandas, NumPy for data handling
- Scikit-learn for PCA and clustering
- Matplotlib and Seaborn

## 👤 Author

Yi Hsiang (Royce) Yen  
MS in Business Analytics, University of Minnesota  
