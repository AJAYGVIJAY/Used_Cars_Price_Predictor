```markdown
# Car Price Prediction Model

Predict used car prices using XGBoost (MAE: $2,914 | R²: 0.96).

## Features
- Clean data & remove outliers
- Feature engineering (Age, HP/cylinder)
- XGBoost model with hyperparameter tuning
- Identify underpriced cars

## Getting Started
1. Clone repo:
   ```bash
   git clone https://github.com/yourusername/car-price-prediction.git
   ```
2. Install packages:
   ```bash
   pip install pandas xgboost scikit-learn matplotlib
   ```
3. Run Jupyter notebook:
   ```bash
   jupyter notebook Car_Price_Prediction.ipynb
   ```

## Code Highlights
```python
# Clean data
df = df[df['MSRP'] < 200_000]

# Train model
model = XGBRegressor(n_estimators=1000, learning_rate=0.05)
model.fit(X_train, y_train)
```

## Results
- **MAE**: $2,914
- **R²**: 0.96

| Make   | Actual Price | Predicted Price |
|--------|--------------|-----------------|
| Honda  | $18,500      | $21,200         |
| Toyota | $19,999      | $22,800         |

## Project Structure
```
.
├── Car_Price_Prediction.ipynb  # Main code
├── data_sample.csv             # Sample data
└── images/                     # Charts
```

