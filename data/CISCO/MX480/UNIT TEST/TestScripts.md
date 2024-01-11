

Sure! Below are separate Python scripts for each unit test. Additionally, I will provide data with markdown-compatible for headers, sub-headers, paragraphs, and code snippets that resemble the output format of ChatGPT.

### Unit Test 1: Test Addition Function
#### Script: test_addition.py
```python
# test_addition.py
import unittest
from calculator import addition

class TestAddition(unittest.TestCase):
    def test_add_positive_numbers(self):
        result = addition(3, 5)
        self.assertEqual(result, 8)

    def test_add_negative_numbers(self):
        result = addition(-3, -5)
        self.assertEqual(result, -8)

if __name__ == '__main__':
    unittest.main()
```

### Unit Test 2: Test Subtraction Function
#### Script: test_subtraction.py
```python
# test_subtraction.py
import unittest
from calculator import subtraction

class TestSubtraction(unittest.TestCase):
    def test_subtract_positive_numbers(self):
        result = subtraction(8, 5)
        self.assertEqual(result, 3)

    def test_subtract_negative_numbers(self):
        result = subtraction(-3, -5)
        self.assertEqual(result, 2)

if __name__ == '__main__':
    unittest.main()
```

### Data with Markdown Format
#### Headers
# Main Header
## Sub Header

#### Paragraphs
This is a paragraph.

#### Code Snippet
```python
print("Hello, world!")
```

Feel free to use the provided script and data for your needs. Let me know if you need any more help!