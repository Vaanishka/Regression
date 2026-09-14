# Linear Regression: WWII Weather Temperature Prediction
This project demonstrates the implementation of a single-variable Linear Regression model to forecast weather conditions. Using a historical dataset of weather conditions recorded at various weather stations during World War II, the model investigates the linear relationship between daily minimum and maximum temperatures to predict peak daily temperatures.

## Technical Implementation: 
* **Mathematical Foundation:** The model is built on the standard linear equation $y = ax + b$, where the predictor variable ($x$) is the Minimum Temperature and the target variable ($y$) is the Maximum Temperature.
* **Data Processing & EDA:** Utilized pandas for data ingestion and descriptive statistics. Implemented matplotlib to visualize the linear correlation between minimum and maximum temperatures prior to modeling.
* **Model Training:** Leveraged scikit-learn to partition the dataset into an 80/20 train-test split and train an Ordinary Least Squares (OLS) Linear Regression model.
* **Performance Evaluation:** Evaluated the model's accuracy using $R^2$ scoring. The model achieved a training score of 0.770 and a testing score of 0.776, indicating robust generalization to unseen data with no signs of overfitting or underfitting.





# Multiple Linear Regression: Hardware Performance Prediction
This project explores the implementation of a Multiple Linear Regression model to estimate the relative CPU performance of computer hardware. Utilizing the UCI Computer Hardware dataset, the model predicts the Estimated Relative Performance (ERP) based on six continuous hardware specifications, including machine cycle time, main memory, and cache memory.

## Technical Implementation: 
* **Exploratory Data Analysis (EDA):** Filtered out categorical variables and generated a correlation heatmap using Seaborn to identify strong positive linear relationships between main memory (MMIN, MMAX) and the target variable.
* **Data Preprocessing:** Standardized all continuous features using Scikit-Learn's StandardScaler to ensure uniform scale and improve model convergence before applying the 70/30 train-test split.
* **Model Training:** Fitted an Ordinary Least Squares Multiple Linear Regression model, extracting the intercept and multi-dimensional coefficients to understand the weight of each hardware feature.
**Model Validation:** Employed 5-Fold Cross-Validation to test the model's generalization capabilities across different data subsets, providing a more rigorous assessment than standard train-test splitting.



