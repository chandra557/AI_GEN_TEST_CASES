

## Unit Test 1: Test User Input

### Description
This unit test will check if the user input is being correctly processed in the program.

### Test Data
```python
from my_program import process_user_input

def test_user_input():
    assert process_user_input("hello") == "You said: hello"
    assert process_user_input("How are you?") == "You said: How are you?"
```

## Unit Test 2: Test ChatGPT Response

### Description
This unit test will check if the ChatGPT model is generating valid responses to user input.

### Test Data
```python
from my_program import generate_gpt_response

def test_chatgpt_response():
    assert generate_gpt_response("hello") == "Nice to meet you!"
    assert generate_gpt_response("How are you?") == "I'm doing well, thank you for asking."
```

## Unit Test 3: Test ChatGPT with Invalid Input

### Description
This unit test will check if the program handles invalid input gracefully.

### Test Data
```python
from my_program import generate_gpt_response

def test_invalid_input():
    assert generate_gpt_response("") == "I'm sorry, I didn't understand that."
    assert generate_gpt_response("!@#$%") == "I'm sorry, I didn't understand that."
```