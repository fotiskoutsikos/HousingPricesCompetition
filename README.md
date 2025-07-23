# House Prices - Kaggle Competition  

**Kaggle Score:** 16,108.56 (Top 10% Leaderboard)  
**Technologies:** Python, Pandas, Scikit-learn, LightGBM, Feature Engineering  

## Overview  
Predicting house sale prices using machine learning for the [Kaggle House Prices Competition](https://www.kaggle.com/competitions/home-data-for-ml-course).
Key achievements:  
- Engineered high-impact features boosting model accuracy by 2.5%  
- Achieved **11.7% relative error** (vs. mean price $138k)  
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

2. **Distribution Insights**  
   - Sale prices showed **positive skew** (concentrated at lower end)  
   - Log transformation normalized target variable  


## Model Comparison  
| Model                  | Validation MAE |  
|------------------------|----------------|  
| **LightGBM**           | **15,120**     |   
| XGBoost                | 15,469         |   
| HistGradientBoost      |   15,572       |   

## Conclusions  
1. **Core Drivers** explain 82% of price variance  
2. Strategic **outlier removal** improves model robustness  
3. **LightGBM outperformed** alternatives in speed/accuracy tradeoff  
4. **Minimal overfitting** (6.5% validation-test gap)  

