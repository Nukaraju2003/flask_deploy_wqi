# WaterQuality
<p align="center">
<img src="#" >
</p>

Build web application using flask and python to predict water potability.

## Context
"WATER QUALITY INDEX PREDICTION ON EAST AND WEST GODAVARI DISTRICTS Utilizing machine learning techniques, we've developed a predictive model for water quality in East and West Godavari districts. By considering factors like pH, hardness, solids, chloramines, sulfate conductivity, organic carbon, and trihalomethanes turbidity, our model assesses whether the water is suitable for consumption. After thorough comparison, XGBoost emerged as the top-performing model, offering the most accurate predictions."

Here's a brief overview of what's happening in the code:
1. Data loading: A dataset (Kollerudataset.csv) containing water quality parameters is loaded into a Pandas DataFrame.
2. Data preprocessing: The dataset is cleaned by removing duplicates and handling missing values.
3. Data visualization: Histograms and a heatmap are used to visualize the data's distribution and correlation between features.
4. Feature engineering: Some missing values in the dataset are filled using the mean values of corresponding features.
5. Model building: Several machine learning models like Logistic Regression, K-Nearest Neighbors, Decision Tree, Random Forest, AdaBoost, Bagging, and XGBoost are trained and tuned using GridSearchCV or RandomizedSearchCV for hyperparameter optimization.
6. Model evaluation: The trained models are evaluated using the test set, and their accuracy scores are printed.
7. Model deployment: The best-performing model (XGBoost) is saved to a file using pickle for future use.
8. Model prediction: An example prediction is made using the saved model and a sample input, demonstrating how to use the model for inference.


## Architecture
<p align="center">
<img src="#">
</p>

## About Data

ppm: parts per million\
μg/L: microgram per litre\
mg/L: milligram per litre

**Column description:**

**1. ph:** pH of 1. water (0 to 14).\
**2. Hardness:** Capacity of water to precipitate soap in mg/L.\
**3. Solids:** Total dissolved solids in ppm.\
**4. Chloramines:** Amount of Chloramines in ppm.\
**5. Sulfate:** Amount of Sulfates dissolved in mg/L.\
**6. Conductivity:** Electrical conductivity of water in μS/cm.\
**7. Organic_carbon:** Amount of organic carbon in ppm.\
**8. Trihalomethanes:** Amount of Trihalomethanes in μg/L.\
**9. Turbidity:** Measure of light emiting property of water in NTU.\
**10. Potability:** Indicates if water is safe for human consumption. Potable is 1 and not potable is 0.


## Prediction

  ph | Hardness | Solids | Chloramines | Sulfate | Conductivity | Organic_carbon | Trihalomethanes | Turbidity | Potability
 --- | --- | --- |--- |--- |--- |--- |--- |--- |---
  8.8 | 224 | 1100 | 6 | 1500 | 600 | 5 | 90 | 6 | 0


<p align="center">
<img src="#" >
</p>

