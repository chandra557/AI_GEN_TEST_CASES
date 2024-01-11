

Sure, here is an example of how you can structure your unit tests in separate Python files with data provided in Markdown format:

### test_addition.py

```python
import unittest
from my_math_functions import add

class TestAddition(unittest.TestCase):
    def test_add_positive_numbers(self):
        result = add(2, 3)
        self.assertEqual(result, 5)

    def test_add_negative_numbers(self):
        result = add(-5, -3)
        self.assertEqual(result, -8)

if __name__ == "__main__":
    unittest.main()
```

### my_math_functions.py

```python
def add(a, b):
    return a + b
```

### test_subtraction.py

```python
import unittest
from my_math_functions import subtract

class TestSubtraction(unittest.TestCase):
    def test_subtract_positive_numbers(self):
        result = subtract(5, 3)
        self.assertEqual(result, 2)

    def test_subtract_negative_numbers(self):
        result = subtract(-5, -3)
        self.assertEqual(result, -2)

if __name__ == "__main__":
    unittest.main()
```

### my_math_functions.py

```python
def subtract(a, b):
    return a - b
```

This structure allows you to create separate test files for each unit of functionality in your code, making it easier to maintain and understand the tests. The Markdown format provided allows you to present the code and its output in a readable way that resembles the structure of a conversation in ChatGPT.