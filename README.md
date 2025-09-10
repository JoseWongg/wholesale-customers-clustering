
# Wholesale Customers Clustering (Python)

Unsupervised customer segmentation on the **Wholesale Customers** dataset (UCI) to discover purchasing patterns and actionable groups.  
Two algorithms are compared: **K‑Means** and **Hierarchical Agglomerative Clustering (HAC)**. Includes EDA, preprocessing, dimensionality reduction, evaluation, and business recommendations.

---

## Repository Structure
```
wholesale-customers-clustering/
├── notebooks/
│   └── wholesale_customers_clustering.ipynb   # Jupyter notebook (code + outputs)
├── data/
│   └── Wholesale customers data.csv           # Dataset
├── docs/
│   └── report.pdf                             # Analysis report (PDF)
├── LICENSE
└── README.md
```

---

## Dataset & License
**Name:** Wholesale Customers — UCI Machine Learning Repository  
**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)  
**Source:** https://archive.ics.uci.edu/dataset/292/wholesale+customers  
**Citation:**  
Cardoso, M. (2013). *Wholesale customers* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5030X

Main variables (annual spend): `Fresh`, `Milk`, `Grocery`, `Frozen`, `Detergents_Paper`, `Delicatessen`  
Categoricals: `Channel` (1=Horeca, 2=Retail), `Region` (1=Lisbon, 2=Oporto, 3=Other)

---

## What’s Inside
- **EDA:** structure, distributions, skewness, correlations; channel/region makeup.
- **Preprocessing:** outlier capping (IQR), log transform of skewed variables, **Z‑score scaling**.
- **Clustering:**  
  - **K‑Means** (K selected via elbow + silhouette).  
  - **HAC** (Ward linkage; dendrogram‑guided cluster count).  
- **Dimensionality reduction:** **PCA** to visualise clusters in 2D and inspect component loadings.
- **Evaluation:** silhouette score, cluster profiles (means/modes), comparative discussion.
- **Business impact:** targeted promos, inventory planning, segment‑specific actions.
- **Ethics:** avoid discriminatory targeting; respect data‑use constraints even with anonymised data.

---

## How to Use
### Quick View
Open `notebooks/wholesale_customers_clustering.ipynb` directly on GitHub to read the analysis.

### Run Locally
1) Clone the repo:
```bash
git clone https://github.com/JoseWongg/wholesale-customers-clustering.git
cd wholesale-customers-clustering
```
2) Open the notebook:
```bash
jupyter notebook notebooks/wholesale_customers_clustering.ipynb
```

---

## Authorship & Contact
Developed by **Jose Wong**  
j.wong@mail.com  
https://www.linkedin.com/in/jose-wongg  
https://github.com/JoseWongg

---

## License
MIT — see the [LICENSE](LICENSE) file. 
