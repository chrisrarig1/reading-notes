# How to run Linear regression in Python

## Exporting Data

- Import lib: `import sklearn`
- Import data: `from sklearn.datasets import data`
- Rename data: `data_set = data()`
- Convert into panda data frame: `data_frame = pd.DataFrame(data_set.data)`
- Replace column names with actual labels: `data_frame.columns = data_set.feature_names`

## Scikit Learn

- **Y** = target data
- **X** = independent variable
- Import Scikit: ` from sklearn.linear_model import LinearRegression`
- Drop: `X = data_frame.drop('target data', axis = 1)`
- Linear Regression: `lm = LinearRegression()`

### Linear Reg

- `lm.fit()`: fits a linear model
- `lm.predict()`: Predict Y using the linear model with estimated coefficients
- `lm.score()`: Returns coefficient of determination (R^2)
- `lm.coef_`: Estimated coefficients
- `lm.intercept_`: Estimated intercept

## Fitting

- `lm.fit(x, data_frame.target)`
- Check intercepts and number of coefficients:
  - `print 'Estimated intercept coefficient:', lm.intercept_`
  - `print 'Number of coefficients:', len(lm.coef_)`
- Construct data frame that contains features and estimated coefficients:
  - `pd.DataFrame(zip(X.columns, lm.coef_), columns = ['Features', 'estcoeff'])`

## Plotting

- Scatter Plot: `plt.scatter(data_frame.x-axis, data_frame.y-axis)`
- X labels: `plt.xlabel("x-axis Label`)
- Y labels: `plt.ylabel("y-axis Label`)
- Title: `plt.title("graph title")`
- Display: `plt.show()`

## Predicting Data

- Predicting: `lm.predict(target_data)`
- Mean Squared Error: `np.mean((data_frame.data - lm.predict(target_data))**2))`

# Useful Links

- [Linear Regression](https://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn/)
- [Introduction to Simple Linear Regression](https://www.youtube.com/watch?v=KsVBBJRb9TE)