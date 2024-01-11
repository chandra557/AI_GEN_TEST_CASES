

For regression testing in Python, you can create separate test scripts for each regression test. Here's an example of a Python script for a regression test:

test_case_1.py

```python
import unittest
from your_module import regression_function_1

class TestRegressionFunction1(unittest.TestCase):
    def test_input_1(self):
        result = regression_function_1(input_1)
        self.assertEqual(result, expected_output_1)

    def test_input_2(self):
        result = regression_function_1(input_2)
        self.assertEqual(result, expected_output_2)

    # Add more test cases as needed

if __name__ == '__main__':
    unittest.main()
```

You can then define the test data in a markdown-compatible format:

## Data for Regression Test 1
### Input 1
Paragraph describing the input data for test case 1.

```python
input_1 = ...
```

### Input 2
Paragraph describing the input data for test case 2.

```python
input_2 = ...
```

### Expected Output 1
Paragraph describing the expected output for test case 1.

```python
expected_output_1 = ...
```

### Expected Output 2
Paragraph describing the expected output for test case 2.

```python
expected_output_2 = ...
```

This approach allows you to clearly document the test data, expected outputs, and code snippets in a format that resembles the output format of ChatGPT. You can create similar Python scripts and corresponding markdown data for each regression test.