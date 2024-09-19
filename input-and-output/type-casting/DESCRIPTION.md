***Input is only stored in strings, how do we do math on strings?***
Python does not have the ability to do math on strings. So, if you're expecting the user to input a numeric value it will have to be converted to be used throughout the rest of the program. Thankfully, Python allows type casting and makes this process very easy. 

```
age = input("Enter your age: ")
future_age = age + 7
print("Age in the future", future_age)
```

If you were to run the code above you would likely encouter a `TypeError`. If we see what the program is doing, we can most likely assume that age is an integer and the input we get from the user will be an integer. You can simply cast it to an integer, by using the `int()` function. 

```
age = int(input("Enter your age: "))
future_age = age + 7
print("Age in the future", future_age)
```

Python will let you type cast other things as well. The ones you should be concerned about are `int()`, `float()`, and `str()`. 

***Challenge:*** ENTER CHALLENGE HERE