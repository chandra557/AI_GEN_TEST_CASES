

Sure, here's an example of how a Python script for a regression test would look like:

```python
# test_regression_1.py

import numpy as np
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error

# Data
X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
y = np.array([2, 4, 5, 4, 5])

# Model
model = LinearRegression()
model.fit(X, y)

# Prediction
y_pred = model.predict(X)

# Evaluation
mse = mean_squared_error(y, y_pred)
print("Mean Squared Error:", mse)
```

And here's an example of markdown compatible data for the test:

```
# Regression Test 1
## Description
This test examines the performance of a simple linear regression model on a small dataset.

### Inputs
- X: [1, 2, 3, 4, 5]
- y: [2, 4, 5, 4, 5]

### Steps
1. Fit a linear regression model on X and y
2. Predict the values using the model
3. Calculate the Mean Squared Error (MSE) between the actual and predicted values

### Expected Output
Mean Squared Error: 0.7
```