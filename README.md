# 🛍️ Customer Segmentation Using K-Means + PCA

Unsupervised machine learning project that segments customers into meaningful
groups based on their purchasing behavior — using K-Means Clustering and PCA visualization.

---

## 📌 Problem Statement

Retail businesses have thousands of customers but treat them all the same.
This project solves that by automatically grouping customers based on their Age, Annual Income, and Spending Score 
— so businesses can target each group with the right strategy.

---

## 🔬 Techniques Used

- K-Means Clustering
- Elbow Method (to find optimal number of clusters)
- Silhouette Score Analysis
- Principal Component Analysis (PCA) for 2D visualization
- StandardScaler for feature normalization
- Business Interpretation of each cluster

---

## 📂 Project Structure

```
├── Customer_Segmentation_Project.ipynb   # Main notebook
├── Mall_Customers.csv                    # Dataset (download separately)
├── customer_segments_output.csv          # Output: full data with cluster labels
├── cluster_profiles.csv                  # Output: average profile per cluster
├── scatter_raw.png                       # EDA scatter plot
├── distributions.png                     # Feature distribution plots
├── elbow_silhouette.png                  # Elbow + silhouette curves
├── clusters_pca.png                      # Final 2D cluster visualization
├── cluster_comparison.png                # Bar chart comparison by feature
└── README.md                             # Project documentation
```

---

## 📊 Dataset

**Mall Customer Segmentation Dataset**  
Source: [Kaggle — vjchoudhary7](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

Download `Mall_Customers.csv` and place it in the same folder as the notebook.

> **No dataset?** No problem. The notebook includes a built-in synthetic dataset generator — just run it and it works automatically without any download.

**Features used:**
| Feature | Description |
|---------|-------------|
| Age | Customer age in years |
| Annual Income (k$) | Yearly income in thousands |
| Spending Score (1–100) | Mall-assigned score based on spending behavior |

---

## ⚙️ How to Run

**1. Clone this repository**
```bash
git clone https://github.com/your-username/customer-segmentation.git
cd customer-segmentation
```

**2. Install required libraries**
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

**3. Open the notebook**
```bash
jupyter notebook Customer_Segmentation_Project.ipynb
```

**4. Run all cells from top to bottom**

---

## 🧠 Project Steps

| Step | Description |
|------|-------------|
| 1 | Import libraries |
| 2 | Load dataset (real CSV or synthetic fallback) |
| 3 | Exploratory Data Analysis — distributions and scatter plots |
| 4 | Handle missing and infinite values |
| 5 | Feature scaling with StandardScaler |
| 6 | Find optimal K using Elbow Method + Silhouette Score |
| 7 | Apply K-Means clustering |
| 8 | Dimensionality reduction with PCA (2 components) |
| 9 | Visualize clusters in 2D PCA space |
| 10 | Cluster analysis and business interpretation |
| 11 | Save results to CSV and PNG files |

---

## 💡 Business Interpretation

Each cluster gets a real-world label based on its average Income and Spending Score:

| Cluster | Profile | Recommended Strategy |
|---------|---------|----------------------|
| 💎 High Value | High income + high spending | Target with premium products and exclusive offers |
| 💼 Cautious Affluent | High income + low spending | Build trust, loyalty programs, personalized outreach |
| 🎯 Young Spenders | Low/mid income + high spending | Affordable deals, EMI options, trend-based marketing |
| 😐 Average | Mid income + mid spending | General campaigns, seasonal discounts |
| 💤 Low Engagement | Low income + low spending | Re-engagement campaigns, budget-friendly offers |

---

## 📈 Sample Outputs

- **Elbow Curve** — shows the optimal number of clusters (K)
- **Silhouette Score Chart** — validates cluster quality
- **2D PCA Scatter Plot** — visual separation of customer groups
- **Cluster Profile Bar Charts** — comparison of Age, Income, Spending per cluster
- **CSV Export** — full dataset with cluster labels for further use

---

## 🛠️ Requirements

```
Python >= 3.7
numpy
pandas
matplotlib
scikit-learn
jupyter
```

Install all at once:
```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

---

## 👤 Author

**Ali Ahmad**  
Founder & CEO — Genvorex AI  
AI Engineer | GenAI & Agentic Systems | RAG | Workflow Automation  


## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Built as part of AI/ML learning journey — Genvorex AI*
