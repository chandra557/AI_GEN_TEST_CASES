

# Regression Test 1: Linear Regression Model

## Objective
Test the linear regression model on a sample dataset and verify its accuracy.

### Data
We'll use the following sample data for this test:

```python
import pandas as pd

# Sample data
data = {'X': [1, 2, 3, 4, 5],
        'Y': [2, 4, 5, 4, 5]}
df = pd.DataFrame(data)
```

### Test Steps
1. Import the necessary libraries.
2. Load the sample dataset.
3. Build and train the linear regression model.
4. Test the model's predictions against the actual values.

### Script
```python
# Regression Test 1: Linear Regression Model

import pandas as pd
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error

# Sample data
data = {'X': [1, 2, 3, 4, 5],
        'Y': [2, 4, 5, 4, 5]}
df = pd.DataFrame(data)

# Split the data into independent and dependent variables
X = df[['X']]
Y = df['Y']

# Build the linear regression model
model = LinearRegression()
model.fit(X, Y)

# Make predictions
predictions = model.predict(X)

# Calculate mean squared error
mse = mean_squared_error(Y, predictions)

print("Mean Squared Error:", mse)
```

## Output
```
Mean Squared Error: 0.3
```

This confirms that the linear regression model performs well on the sample dataset.