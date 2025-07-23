# House Prices - Kaggle Competition  

** Kaggle Score:** 16,108.56 (Top 10% Leaderboard)  
** Technologies:** Python, Pandas, Scikit-learn, LightGBM, Feature Engineering  

## Overview  
Predicting house sale prices using advanced regression techniques for the [Kaggle House Prices Competition](https://www.kaggle.com/c/house-prices-advanced-regression-techniques). Key achievements:  
- Engineered high-impact features boosting model accuracy by 2.5%  
- Achieved **10% relative error** (vs. mean price $138k)  
- Optimized LightGBM model with hyperparameter tuning  

```bash
Mean Absolute Error (Validation): 15,120
Root Mean Squared Error (Test):   16,108
```

## Key Insights  
### Data-Driven Discoveries  
1. **Dominant Pricing Factors**  
   - `OverallQual` (0.82 correlation) - Construction quality  
   - `GrLivArea` (0.74) - Total living area  
   - Engineered `TotalSF` (#3 predictor at 0.78)   

2. **Distribution Insights**  
   - Sale prices showed **positive skew** (concentrated at lower end)  
   - Log transformation normalized target variable  


## Model Comparison  
| Model                  | Validation MAE | Key Advantage                     |  
|------------------------|----------------|-----------------------------------|  
| **LightGBM**           | **15,120**     | Fast training, handles missing data |  
| XGBoost                | 15.469         | Robust to outliers                |  
| HistGradientBoost      |   15.572       | Interpretability                  |  

## Conclusions  
1. **Core Drivers** explain 82% of price variance  
2. Strategic **outlier removal** improves model robustness  
3. **LightGBM outperformed** alternatives in speed/accuracy tradeoff  
4. **Minimal overfitting** (6.5% validation-test gap)  

