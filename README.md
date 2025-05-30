Linear Regression Project Report – Housing Price Prediction
Objective
The aim of this project is to predict housing prices using Linear Regression, by analyzing various features such as area, amenities, and furnishing status from a dataset.

Tools and Libraries
•	Python
•	pandas
•	numpy
•	matplotlib
•	seaborn
•	scikit-learn

Dataset
•	Source: Kaggle - Housing Price Prediction Dataset
•	Format: CSV
•	Target Variable: price
•	Features include: area, bedrooms, bathrooms, mainroad, guestroom, basement, hotwaterheating, airconditioning, parking, furnishingstatus, etc.

 Data Preprocessing
•	Encoded categorical variables into numerical form using mapping.
•	Removed missing values (if any).
•	Separated features (X) and target (y).
Model Training
•	Model Used: LinearRegression from sklearn.linear_model
•	Split: 80% training, 20% testing using train_test_split()
•	Fitting: Model trained on the training set using model.fit(X_train, y_train)

 Evaluation Metrics
Metric	       Value (approx)
MAE	           63,000
MSE	           8.1e+09
RMSE	         90,000
R² Score	     0.67
Note: These may vary slightly depending on the data split and pre-cleaning.

 Visualizations
1. Predicted vs Actual Price (by Area)
•	Plotted the predicted prices (line) against actual prices (scatter).
•	Smoother output achieved by sorting area.
(if exporting image)
2. Seaborn Regression Plot
•	sns.regplot() used to fit a linear regression line with confidence interval over test data.
Observations
•	The model captures the trend well but has noticeable variance.
•	Linear Regression works decently here, but performance might improve with:
o	Feature engineering (e.g., log-transform of skewed features)
o	Polynomial regression
o	Regularization (Ridge/Lasso)

