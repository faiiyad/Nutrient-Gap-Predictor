# Nutrient Gap Predictor
![banner](https://raw.githubusercontent.com/faiiyad/Nutrient-Gap-Predictor/refs/heads/main/images/Banner_amini.png)

Predicts nutrient gaps for maize crops across Africa, contributing to solutions promoting sustainable agriculture and precision soil management.
Submitted for the <a href='https://zindi.africa/competitions/amini-soil-prediction-challenge'>Amini Soil Prediction Challenge.</a>

## How it works:
### Model selection:
Used a `RandomForestRegressor` (with `n_estimators=100`), wrapped in a `MultiOutputRegressor`, to predict all nutrient values simultaneously. Then calculated the nutrient gap for each site-nutrient pair to generate the final results.
### Feature engineering:
Used ratios of various given features such as pH, bio1, bio12 and bulk density to guide the model towards a more accurate result.
### Results:
Achieved a score of `1057.362854 RMSE`, which outperforms the given benchmark score. Ranked **top 150 out of 980+ participants globally.**
