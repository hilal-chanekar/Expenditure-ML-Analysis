# 📊 UK Household Expenditure Analysis

A machine learning project analyzing household spending patterns in the United Kingdom using the Living Costs and Food Survey (LCF) dataset.

## 🎯 Project Objective

To identify and quantify the key socioeconomic factors that influence household expenditure in the UK, providing actionable insights for policy makers and researchers.

## 📁 Dataset

| Attribute | Description |
|-----------|-------------|
| **Source** | Living Costs and Food Survey (LCF) |
| **Sample Size** | 5,144 UK households |
| **Features** | 19 variables |

### Key Variables
- `P550tpr` - Total weekly household expenditure (target)
- `P344pr` - Gross normal weekly household income
- `A049r` - Tenure type (Owned/Rented)
- `A094r` - NS-SEC occupational classification
- `NumAdult` / `NumChild` - Household composition
- `Gorx` - UK region

## 🔬 Methodology

### Statistical Analysis
- **Welch-ANOVA** - Comparing expenditure across demographic groups
- **Shapiro-Wilk Test** - Normality assessment
- **Levene's Test** - Homogeneity of variances

### Machine Learning Pipeline

```
Raw Data → Preprocessing → Feature Engineering → Model Training → Evaluation
```

| Model | Purpose |
|-------|---------|
| Linear Regression | Baseline model |
| Random Forest | Non-linear relationships |
| XGBoost | Gradient boosting |
| CatBoost | Categorical feature handling |

## 📈 Key Findings

| Factor | Correlation with Expenditure |
|--------|------------------------------|
| Income | 0.71 (Strong positive) |
| Number of Adults | 0.34 |
| Household Size | 0.31 |
| Number of Children | 0.14 |

### Statistical Insights
- ✅ Significant differences in expenditure across **tenure types** (p < 0.05)
- ✅ Significant differences across **occupational classes** (p < 0.05)
- ✅ **Income** is the strongest predictor of household spending

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn)

- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: scikit-learn, XGBoost, CatBoost
- **Statistical Testing**: pingouin

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib scikit-learn xgboost catboost pingouin
```

### Run the Analysis

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/Expenditure-ml-analysis.git
cd Expenditure-ml-analysis

# Launch Jupyter Notebook
jupyter notebook case_study.ipynb
```

## 📂 Project Structure

```
Expenditure-ml-analysis/
│
├── case_study.ipynb    # Main analysis notebook
├── README.md           # Project documentation
└── .gitignore          # Git ignore rules
```

## 📊 Sample Visualizations

The notebook includes:
- Correlation heatmaps
- Feature importance plots
- Distribution analysis by demographic groups

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Hilal**

[![GitHub](https://img.shields.io/badge/GitHub-Profile-black?logo=github)](https://github.com/YOUR_USERNAME)

---

⭐ Star this repository if you found it helpful!