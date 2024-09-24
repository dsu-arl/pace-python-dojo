**Function arguments** are the values or variables passed into a function when it is called. You can define what is to be passed when calling your function and the function's behavior will often depend on the arguments passed. This adds a new rule to our function definition:
-  Any parameters or arguments should be placed within the function definition's parentheses

While defining a function, you specify a list of variables within the parentheses (these are referred to as **parameters**). These parameters act as a placeholder for the data that will be passed to the function when it is called. When the function is called, value to each of these parameters must be provided and can be used just like any other variable, but are referred to by the parameter name. The values provided are known as **arguments**. 

**Example:**
```
def greeting(name):
	print("Hello {}".format(name))
  return
  
greeting("Batman")
greeting("Brandon")
greeting("Chris")
```
Running this code will produce the following output:
```
Hello Batman
Hello Brandon
Hello Chris
```

Python supports mainy different types of Function Arguments, but the one we will cover in-depth is **Positional/Required** arguments. This is nothing new, as what we just wrote is considered a positional or required argument. They are called this, because the function cannot execute unless every parameter listed gets an argument in the correct positional order. Let's look at another example:
```
def printInfo(name, age):
	print("Name: ", name)
  print("Age: ", age)
  
printInfo("Brandon", 14)
printInfo("Chris")
```
Executing this code will print the following:
```
Name: Brandon
Age: 14
Traceback (most recent call last):
	File "test.py", line 6, in <module>
  	printInfo();
TypeError: printInfo() takes exactly 2 arguments (1 given)
```
From this we can see the first function call worked as expected because every parameter was passed in the correct order. The second one did not, as we did not pass anything for `age` and that is a required parameter.


***CHALLENGE:*** Challenge Goes Here.