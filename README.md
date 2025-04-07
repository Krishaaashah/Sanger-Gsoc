# 🧬 Cloud-Native ML Classifier for Genomic Classification of *Anopheles* Mosquitoes

> Google Summer of Code 2025 Proposal | **Sanger Institute**  
> Contributor: Krisha | Status: For Review

---
Self Link: [View GSoC Proposal Draft](https://docs.google.com/document/d/1vhLDmtNGIYiJTOX3fdL9POejZ-XjGz7dfH1JXPArSZM/edit?usp=sharing)

## 📌 Summary

This project aims to develop a scalable, cloud-native machine learning pipeline for classifying *Anopheles* mosquito species using genomic data from the MalariaGEN Vector Observatory. This classifier will help entomologists and researchers automate and accelerate vector surveillance efforts globally.

---

## 🚀 Project Goal

Build a reproducible, well-documented ML pipeline that:
- Accepts raw genome sequence data (FASTA/CSV)
- Preprocesses and extracts features using k-mer or one-hot encoding
- Trains multiple classification models (Random Forest, XGBoost, CNN)
- Evaluates and benchmarks performance
- Deploys the best model as an API using a cloud-native approach (e.g., Docker + Streamlit/FastAPI on GCP/AWS)

---

## 🧱 Tech Stack

| Stage            | Technology                             |
|------------------|----------------------------------------|
| Data Handling    | `Biopython`, `Pandas`, `Scikit-learn`  |
| ML Training      | `XGBoost`, `PyTorch`, `LightGBM`       |
| Deployment       | `Docker`, `FastAPI`, `Streamlit`, `GCP`|
| Visualization    | `Plotly`, `Matplotlib`, `Seaborn`      |
| CI/CD            | `GitHub Actions`, `pre-commit`         |

---

## 📂 Repository Structure

```bash
📦 Anopheles-Classifier
├── data/                  # Sample / test genomic datasets
├── notebooks/             # Jupyter notebooks for exploration
├── src/                   # Core pipeline code (preprocess, train, evaluate)
├── models/                # Saved models (.pkl / .onnx)
├── app/                   # Streamlit / FastAPI app code
├── Dockerfile             # For containerizing the app
├── .github/workflows/     # GitHub Actions CI/CD configs
└── README.md              # You are here
