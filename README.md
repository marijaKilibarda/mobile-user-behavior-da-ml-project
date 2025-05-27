# 📱 Mobile App Usage Behavior – EDA & Unsupervised Machine Learning

This project analyzes a subset of the **"Worldwide Mobile App User Behavior Dataset"** from **Harvard Dataverse**, comprising over **10,000 survey responses** from users in **15 countries**. The analysis focuses on understanding user behavior related to **how people find, download, and abandon mobile apps**. 

It's performed:
- Deep **Exploratory Data Analysis (EDA)**
- **Unsupervised Learning** via **DBSCAN** and **Gaussian Mixture Models (GMM)**
- An interactive **data storytelling presentation**

---

## 📊 Project Overview

The original dataset surveyed **10,208 people** across **15 countries**, including the USA, China, Japan, Germany, France, Brazil, UK, Italy, Russia, India, Canada, Spain, Australia, Mexico, and South Korea.

Survey content covered:
1. **Mobile App Usage Behavior**
   - App store preferences
   - Triggers for app searches
   - Reasons for downloading or abandoning apps
   - App categories downloaded
2. **Demographics**
   - Age, gender, education, income, nationality, etc.
3. **Psychographics**
   - **Big Five Personality Traits**

🔍 This project focuses **exclusively on mobile app usage behavior**, analyzing behavioral patterns and clustering user types using unsupervised machine learning.
As part of the applied use case, I created a **fictional mobile app prototype called “HiDriver”**, designed and prototyped in **Figma**, to help illustrate how insights from clustering could inform feature prioritization and user targeting.


> 🏆 The project was awarded **Best Data Analysis Project** in December 2024 during the final project competition of the Data Analytics Bootcamp at Ironhack Barcelona. 

---
## 🔬 Methodology

1. **Data Wrangling (Python & pandas)**
   - Source: Harvard Dataverse XLSX (10 208 entries)
   - Loaded, inspected, and reshaped data with `pandas`
   - Filtered for mobile-behaviour questions
   - Handled missing values, encoded categoricals, and standardised numerics

2. **Exploratory Data Analysis**
   - Assessed app-search triggers, download/abandon reasons, and store-visit frequency
   - Visualised patterns across targeted questions
   - Reduced dimensionality with PCA for clustering and plotting

3. **Unsupervised Learning**
   - **DBSCAN**
     - Tuned `eps` and `min_samples` via k-distance plot
   - **Gaussian Mixture Model (GMM)**
     - Selected component count with BIC

4. **Visual Storytelling**
   - Built an interactive Figma prototype for the mock app **HiDriver**
   - Summary slides with clustering insights
   - Visual archetypes of user groups 
---

## 🤖 Unsupervised Learning Models

### 1. **DBSCAN Clustering**
- Non-parametric clustering based on user behavior density
- Useful for identifying niche or irregular app usage types

📓 [View DBSCAN notebook](dbscan_clustering.ipynb)

### 2. **Gaussian Mixture Model (GMM)**
- Probabilistic clustering for nuanced, overlapping behavior
- Helped identify "explorers", "habitual users", and other app personas

📓 [View GMM notebook](gmm_clustering.ipynb)
