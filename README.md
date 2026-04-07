# 🏆 Hi! Paris Hackathon 2026 — PISA Data Challenge

> **Top 3 / 400+** participants · Polytechnique × HEC Paris

## 📋 Overview

Data science competition predicting **mathematical performance scores** of **1.7 million students** from the [PISA](https://www.oecd.org/pisa/) dataset. Our team achieved **R² ≈ 0.77** on the test set.

## 🎯 Challenge

Given socio-economic, educational, and behavioral features from the PISA survey, predict each student's math score with maximum accuracy.

## 🔧 Approach

### Feature Engineering
- **Missing data handling**: Advanced imputation for datasets with 50%+ missing values
- **Target encoding** for high-cardinality categoricals
- **Interaction features** and domain-specific encodings

### Modeling
- **Ensemble** of gradient boosting models:
  - `XGBoost`
  - `LightGBM`
  - `GradientBoosting` (scikit-learn)
- **Optuna** automated hyperparameter tuning
- **Stacking** with ridge regression meta-learner

### Results
| Metric | Score |
|--------|-------|
| R² (test) | ≈ 0.77 |
| Ranking | Top 3 / 400+ |

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/yacine924/hiparis-hackathon.git
cd hiparis-hackathon

# Install dependencies
pip install -r requirements.txt

# Run the pipeline
python main.py
```

## 📂 Project Structure

```
hiparis-hackathon/
├── data/                # Data loading & preprocessing
├── features/            # Feature engineering pipelines
├── models/              # Model training & ensembling
├── notebooks/           # Exploratory analysis
├── main.py              # Main pipeline script
├── requirements.txt
└── README.md
```

## 🛠️ Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189FDD?style=flat-square)
![LightGBM](https://img.shields.io/badge/LightGBM-02569B?style=flat-square)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Optuna](https://img.shields.io/badge/Optuna-4B8BBE?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)

## 👥 Team

- **Yacine Hadioui** — Double BSc Maths & CS, Sorbonne Paris Nord

## 📄 License

MIT License
