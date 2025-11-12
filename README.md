# Bank Customer Churn Prediction

*One-line:* Predict which bank customers are likely to close their accounts and recommend retention actions.

## Project overview
This repository contains an end-to-end churn analysis and prediction project: data, EDA notebook, modeling notebook, trained model, report figures and a simple demo.

## Deliverables
- data/ — raw and processed datasets
- notebooks/ — 01_EDA.ipynb, 02_modeling.ipynb
- src/ — helper modules (data loading, feature engineering, model utils)
- models/ — saved model artifacts (e.g., best_model.pkl)
- reports/ — figures, presentation, insights
- requirements.txt — Python dependencies

## Quick run (high level)
1. Open the notebooks in Jupyter.
2. Install dependencies from requirements.txt.
3. Run notebooks/01_EDA.ipynb then notebooks/02_modeling.ipynb.

## 🧠 EDA Insights

- Total customers: 10,000  
- Churn rate: 20%  
- Spain shows highest churn rate among countries  
- Inactive members are more likely to churn  

### Key Visuals
![Churn Distribution](reports/figures/churn_distribution.png)
![Churn by Geography](reports/figures/churn_by_geography.png)
![Correlation Heatmap](reports/figures/correlation_heatmap.png)
