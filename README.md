# Unsupervised Exploration of Electric School Bus Adoption

This project explores the adoption of **Electric School Buses (ESBs)** across school districts in the United States using **unsupervised machine learning techniques**.

Electric school buses are designed to reduce students’ exposure to diesel emissions and lower greenhouse gas emissions from school transportation. While adoption is increasing nationwide, it still represents a small portion of the total school bus fleet.

The objective of this project is to **discover patterns in ESB adoption across school districts** by analyzing socio-economic, environmental, and adoption-related variables.

This work was completed as part of a **Machine Learning course project** focused on unsupervised data analysis.

---

# Project Objective

The central question of this project is:

**Can we identify meaningful groups of school districts based on their socio-economic characteristics, environmental exposure, and electric school bus adoption patterns?**

To answer this question, the project applies **unsupervised learning methods** to:

- Identify clusters of districts with similar adoption profiles
- Detect districts with unusual adoption patterns
- Explore relationships between demographic indicators and ESB adoption

---

# Dataset

The dataset used in this project is the **Electric School Bus Adoption Dataset**, compiled by the **World Resources Institute (WRI)**.

It contains data describing the transition to electric school buses across thousands of U.S. school districts.

## Key information included

The dataset contains:

### District-level socio-economic indicators
- Poverty rate
- Median household income
- Racial and ethnic composition
- District size
- Urban / suburban / rural classification

### Environmental indicators
- Air pollution levels (PM2.5)
- Ozone exposure
- Asthma prevalence

### Electric school bus adoption metrics
- Number of electric buses committed
- Number delivered or operating
- Bus manufacturers
- Funding sources

### Adoption timeline information
Each electric bus moves through four stages:

- Awarded
- Ordered
- Delivered
- Operating

These stages allow analysis of the **deployment timeline of electric buses**.

---

# Methodology

The analysis follows a typical unsupervised learning pipeline.

---

# 1 Data Preprocessing

Several preprocessing steps were applied:

- Removal of irrelevant variables
- Selection of key socio-economic and environmental variables
- Handling missing values using median imputation
- Feature scaling using standardization

To reduce redundancy:

- Highly correlated variables were removed based on a **correlation threshold**

This produced a cleaned dataset suitable for clustering.

---

# 2 Dimensionality Reduction

High-dimensional data was projected into a lower dimensional space using:

- **Kernel PCA**
- **UMAP**
- **t-SNE**

Among these techniques, **UMAP produced the clearest separation between observations**, and was therefore used for visualization and clustering.

---

# 3 Clustering

Clustering was performed using a **Gaussian Mixture Model (GMM)** applied to the UMAP embedding.

The goal was to identify groups of districts with similar socio-economic and adoption characteristics.

The optimal number of clusters was evaluated using:

- Silhouette score
- Log-likelihood analysis

The analysis identified **three major clusters of districts**.

---

# 4 Cluster Interpretation

The clusters represent different profiles of districts in terms of ESB adoption and socio-economic context.

### Cluster 1 – Transitional districts

Characteristics:

- Moderate ESB adoption
- Slightly below average income
- Higher asthma prevalence
- Mixed demographic composition

Interpretation:

These districts appear to be **in transition toward electrification but still face environmental and socio-economic challenges**.

---

### Cluster 2 – Socio-economically disadvantaged districts

Characteristics:

- High poverty levels
- High proportion of students eligible for free meals
- Very low ESB adoption
- Smaller district sizes

Interpretation:

These districts appear **underrepresented in ESB adoption**, potentially due to financial or infrastructure barriers.

---

### Cluster 3 – Wealthier districts with favorable conditions

Characteristics:

- Higher household income
- Lower poverty rates
- Lower pollution exposure
- Moderate ESB adoption

Interpretation:

These districts appear **better positioned to adopt electric buses earlier**.

---

# 5 Outlier Detection

Outliers were identified using:

- Low cluster membership probabilities from the **Gaussian Mixture Model**
- Low likelihood scores

These outliers may correspond to:

- Districts with unusually large fleets
- Extremely small districts
- Districts with atypical adoption patterns

Further investigation is required to determine whether these cases represent **data irregularities or interesting real-world phenomena**.

---

# Key Insights

The analysis suggests that **electric school bus adoption is uneven across districts**.

Districts that face the **highest environmental and socio-economic challenges are not always the first to adopt electric buses**.

This raises questions about:

- funding accessibility
- infrastructure barriers
- policy design for equitable electrification.

---

# Limitations and Future Improvements

One limitation of this project is the **limited use of the temporal information available in the dataset**.

The dataset includes multiple stages in the adoption process (awarded, ordered, delivered, operating), but the current analysis focuses primarily on static indicators.

A potential improvement would be to **incorporate temporal features**, such as:

- time between funding award and bus delivery
- deployment delays
- adoption speed across districts

These features could provide deeper insights into **deployment efficiency and bottlenecks in the electrification process**.

Future work could also explore:

- anomaly detection using **Isolation Forest**
- **association rule mining** between funding sources and district characteristics
- geographic analysis of adoption patterns.

---

# Technologies Used

Python

Libraries used in this project include:

- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib
- umap-learn

Machine learning methods:

- Dimensionality reduction (PCA, UMAP, t-SNE)
- Gaussian Mixture Models
- Unsupervised clustering
- Exploratory data analysis

---


---

# Author

Machine Learning project focused on **unsupervised data exploration and clustering analysis of electric school bus adoption patterns**.


