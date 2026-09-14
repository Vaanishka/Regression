# Multiple Linear Regression: Hardware Performance Prediction
This project explores the implementation of a Multiple Linear Regression model to estimate the relative CPU performance of computer hardware. Utilizing the UCI Computer Hardware dataset, the model predicts the Estimated Relative Performance (ERP) based on six continuous hardware specifications, including machine cycle time, main memory, and cache memory.

## Technical Implementation: 
**Exploratory Data Analysis (EDA):** Filtered out categorical variables and generated a correlation heatmap using Seaborn to identify strong positive linear relationships between main memory (MMIN, MMAX) and the target variable.
**Data Preprocessing:** Standardized all continuous features using Scikit-Learn's StandardScaler to ensure uniform scale and improve model convergence before applying the 70/30 train-test split.
**Model Training:** Fitted an Ordinary Least Squares Multiple Linear Regression model, extracting the intercept and multi-dimensional coefficients to understand the weight of each hardware feature.
**Model Validation:** Employed 5-Fold Cross-Validation to test the model's generalization capabilities across different data subsets, providing a more rigorous assessment than standard train-test splitting.



