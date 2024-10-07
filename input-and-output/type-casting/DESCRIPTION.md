***Input is only stored in strings, but how do we do math on strings?***
Python does not have the ability to do math on strings. So if you're expecting the user to input a numeric value, it will have to be converted to be used throughout the rest of the program. Thankfully, Python allows type casting and makes this process very easy. 

```python
age = input("Enter your age: ")
future_age = age + 7
print("Age in the future", future_age)
```

If you were to run the code above you would likely encouter a `TypeError`. If we see what the program is doing, we can most likely assume that age is an integer and the input we get from the user will be an integer. You can simply cast it to an integer using the `int()` function. 

```python
age = int(input("Enter your age: "))
future_age = age + 7
print("Age in the future", future_age)
```

Python will let you type cast other things as well. The ones you should be concerned about are `int()`, `float()`, and `str()`. 

#### Challenge:
Use python to calculate a users age + 7

1. Create a new file with the file extension `.py`
2. Write python to accept an integer from user input that represents their age
3. Write the python code to calculate their age in 7 years and prints the resulting number
```bash
# Example Running of the program
python yourScript.py
What is your age: 15
22
```
4. Test your code with `python yourFile.py`
5. Verify your solution with `verify yourFile.py`
