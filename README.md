# From Light to Structure
---

# Galaxy Clustering Analysis – Unsupervised Machine Learning Capstone

This repository contains the code, figures, and final report for my **Unsupervised Machine Learning** capstone project, in which I performed end-to-end clustering of galaxies using Sloan Digital Sky Survey (SDSS) data.

## 📄 Project Overview

As part of the course requirements, I analyzed a large sample of galaxies using photometry, redshift, and morphological features, applying multiple unsupervised learning techniques to discover natural groupings without prior class labels.

I compared and evaluated:

* **K-Means**
* **Gaussian Mixture Models (GMM)**
* **Agglomerative Clustering**
* **DBSCAN** (exploratory tuning)

Clusters were validated against physical classifications using the **BPT diagram** for the emission-line subset.

---

## 🚀 Key Findings

* **Best Model:** K-Means with *k* = 3, PCA-reduced photometric data.
* Strong alignment between photometric clusters and spectroscopic classes (χ² p < 0.001).
* Demonstrated that photometric clustering can serve as a scalable proxy for galaxy classification in large surveys, reducing dependency on full spectroscopy.

---

## 📊 Dataset

* **Source:** [SDSS CasJobs](https://skyserver.sdss.org/casjobs/)
* **Attributes:** Photometric magnitudes (u, g, r, i, z), colors, spectroscopic redshift, morphological parameters, and emission-line fluxes for validation.
* **Selection:** 13 ≤ modelMag\_r ≤ 20, 0.003 ≤ z ≤ 0.25
* **Sample sizes:**

  * Photometry branch: \~100k galaxies
  * Emission-line subset: \~89.8% of photometry branch after S/N filtering

---

## 🛠 Methods & Tools

* **Languages/Libraries:** Python, Pandas, Scikit-learn, Matplotlib, Seaborn, Jupyter
* **Techniques:**

  * Data cleaning and feature engineering (color indices, morphological proxies)
  * Standardization and PCA for dimensionality reduction
  * Clustering with multiple algorithms and hyperparameter sweeps
  * Post-hoc validation using BPT diagrams

---

## 📷 Key Figures

* PCA variance explained curve
* K-Means, GMM, and Agglomerative cluster projections
* DBSCAN k-distance curve
* BPT diagrams colored by photometric clusters
* Missingness heatmap for emission-line features

---

## 📈 Future Work

* Broaden validation beyond BPT using WHAN diagrams, Dn4000, and sSFR.
* Integrate Galaxy Zoo morphologies for enhanced interpretability.
* Apply methodology to deeper and wider surveys (DESI, LSST).
* Explore probabilistic clustering and semi-supervised learning.

---

## 📄 License

None



