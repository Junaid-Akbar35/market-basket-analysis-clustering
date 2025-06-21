

# 🛒 Market Basket Analysis and Customer Segmentation with Multi-Model Clustering

## 📖 Overview

This project performs **Market Basket Analysis** combined with **Multi-Model Clustering** on the **Online Retail Dataset**.
We uncover **frequent product purchase patterns** using **Apriori Algorithm**, segment customers with **clustering algorithms (KMeans, DBSCAN, Agglomerative, Gaussian Mixture, MeanShift)**, and provide **actionable business insights**.

---

## 📂 Dataset

* **Dataset Source**: [Kaggle - Online Retail Dataset by Ulrik Thyge Pedersen](https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset)
* **Size**: \~500,000 transactions
* **Country Used for Analysis**: United Kingdom
* **Time Period**: 2010 - 2011
* **Features Used**:

  * `InvoiceNo`
  * `Description`
  * `Quantity`
  * `InvoiceDate`
  * `UnitPrice`
  * `CustomerID`

---

## ⚙️ Techniques Used

| Technique                 | Purpose                                      |
| ------------------------- | -------------------------------------------- |
| **Apriori Algorithm**     | Discover **frequent product combinations**   |
| **Association Rules**     | Extract **support, confidence, lift**        |
| **PCA, t-SNE**            | Dimensionality reduction for clustering      |
| **Clustering Algorithms** | Segment customer behavior                    |
| → KMeans                  | Partitioning clustering                      |
| → Agglomerative           | Hierarchical clustering                      |
| → Gaussian Mixture        | Probabilistic soft clustering                |
| → DBSCAN                  | Density-based clustering + outlier detection |
| → MeanShift               | Density peak clustering                      |

---

## 📊 Model Results Summary

| Model            | Silhouette Score | Verdict                                 |
| ---------------- | ---------------- | --------------------------------------- |
| ✅ **DBSCAN**     | **0.79**         | ⭐ **Best clustering performance**       |
| KMeans           | 0.42             | ✔ Decent → interpretable segmentation   |
| Agglomerative    | 0.26             | ❗ Weak → overlapping clusters           |
| Gaussian Mixture | -0.06            | ❌ Poor → unclear separation             |
| MeanShift        | 0.29             | ✔ Reasonable → still inferior to DBSCAN |

---

## 📑 Final Insights

### 📦 **Insights from Association Rules**

* **Frequent Product Groups**:

  * **HOME DECORATION**
  * **SEASONAL GIFTS**
  * **RIBBON REELS**
* **Business Recommendation** → Create **product bundles** and run **cross-sell promotions**.

### 👥 **Insights from Clustering**

| Cluster Type          | Business Insight                                     |
| --------------------- | ---------------------------------------------------- |
| **Core Customers**    | Loyalty programs, personalized discounts             |
| **Gift Buyers**       | Seasonal offers, holiday marketing                   |
| **Infrequent Buyers** | Reactivation campaigns, special offers               |
| **Outliers**          | Investigate → Wholesale customers or potential fraud |

---

## 🚀 Business Actions

1. 🎯 **Targeted Marketing** based on clusters.
2. 🎁 **Product Bundling** → Increase average cart value.
3. 🛡️ **Outlier Review** → Improve data quality and detect wholesale activity.

---

## 📁 Project Structure

```
market-basket-clustering/
├── Market_Basket_Clustering_OnlineRetail.ipynb
├── README.md
├── data/
│   └── Online Retail.csv
└── requirements.txt
```

---

## 💻 Installation

```bash
git clone https://github.com/your-username/market-basket-clustering.git
cd market-basket-clustering
pip install -r requirements.txt
```

---

## ✅ Requirements

```
pandas
numpy
matplotlib
seaborn
scikit-learn
mlxtend
```

---

## 🤝 Contributing

Pull requests, feature requests, and suggestions are welcome.
Please open an issue to discuss before making any major changes.

---

## 📄 License

Licensed under the **MIT License**.

---

