### Summary:
&rarr; Chosen model: **LightGBM**
- The assignment was to predict daily sales for each combination of the 54 stores and the 33 product families &rarr; Need to predict 54 (stores) * 33 (families) = 1782 values per day
- There are 1782 target series but traditional statistical models are focused on forecasting a single target series per model
- Need for a global model which is able to forecast multiple target series in one model

&rarr; As the different product families have different seasonal patterns, we train 33 models, one for each product family, which then predicts the sales for each store

### Model Accuracy:
Root Mean Squared Logarithmic Error (RMSLE) as accuracy metric:
- Highest RMSLE: 1.24
- Lowest RMSLE: 0.08

&rarr; **Overall RMSLE: 0.65**
