
# 🧠 Intelligent Data Analysis: PCA on Housing Dataset

This repository contains a Principal Component Analysis (PCA) assignment conducted on a housing dataset. The goal of this analysis is to explore and understand data patterns by reducing dimensionality, identifying principal components, and visualizing relationships between variables such as **price** and **area per bedroom**.

## 📁 Contents

- `IDA - PCA Assignment.ipynb`: Jupyter notebook with code and analysis
- `README.md`: Overview of the project

## 🏠 Dataset Description

The dataset used is the [Housing dataset from Kaggle](https://www.kaggle.com/code/gauravduttakiit/housing-price-prediction-with-pca/notebook), consisting of 545 entries and 16 attributes, including:

- **price**: House price
- **bedrooms**, **bathrooms**, **area**, **stories**
- Several binary (flag) features like `airconditioning`, `mainroad`, `basement`, etc.
- Derived attributes: `areaperbedroom` and `bbratio`

## 🔧 Preprocessing

- **Outliers handled** using the Winsorization method
- **Standardization** applied to all features (mean = 0, variance = 1)
- Ensured no missing values

## 🏷️ Feature Labeling

Two features were chosen for labeling:

- **Price**:
  - Categorized into: `Low`, `Medium`, `High`
  - Binned using specific price ranges
- **Areaperbedroom**:
  - Categorized into: `Very Low`, `Low`, `Medium`, `High`
  - Labeled using quartiles

These labels are visualized post-PCA to analyze how well principal components separate the data categories.

## 📊 Data Analysis & Visualizations

- **Explained Variance**:
  - Price: PC1 explains ~18.47%, PC2 ~13.43%
  - Areaperbedroom: PC1 explains ~22.43%, PC2 ~10.92%
- **Cumulative Variance**:
  - ~90% of variance is captured within the first 9–10 principal components
- **Correlation**:
  - Loadings plotted to show how each feature correlates with PCs
- **VIF Analysis**:
  - Identified multicollinearity using Variance Inflation Factor

## 📈 Visual Insights

- 2D PCA projections show effective grouping of labeled categories
- Histograms reveal skewed price distribution and symmetric areaperbedroom distribution
- Eigenvalue spectra and cumulative plots guide how many PCs to retain

## 🧠 Conclusion

This project demonstrates effective dimensionality reduction using PCA and offers insights into relationships between variables in housing data. It helps identify key features influencing price and spaciousness while handling outliers and collinearity effectively.

## 🛠️ Technologies Used

- Python
- Pandas, NumPy, Matplotlib, Seaborn
- Scikit-learn (PCA, StandardScaler)
- Scipy (Winsorization)

## 📌 Author

**Gokul Prasath Radhakrishnan**  
