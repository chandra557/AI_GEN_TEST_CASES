

Sure, here is an example structure for a test script in Python using the popular `unittest` library along with a data structure in markdown format:

`test_unit_1.py`:
```python
import unittest

class TestUnit1(unittest.TestCase):
    
    def test_case_1(self):
        # Your test case 1 code here
        pass
    
    def test_case_2(self):
        # Your test case 2 code here
        pass

if __name__ == '__main__':
    unittest.main()
```

Markdown format for test data:

# Test Unit 1
## Test Case 1
This test case checks for the correctness of the output when the input is {input_data_1}

### Input
```
{input_data_1}
```

### Expected Output
```
{expected_output_1}
```

## Test Case 2
This test case checks for the correctness of the output when the input is {input_data_2}

### Input
```
{input_data_2}
```

### Expected Output
```
{expected_output_2}
```

You can create similar test scripts and corresponding markdown data for each unit test and save them in separate files. This way, you have a clear separation of concerns for each unit test, as well as a detailed description of the test cases and the expected outputs in markdown format.