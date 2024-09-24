Now, sometimes we want functions to do something to our variables and return a result. This requires defining a function **return value**.

The `return` keyword as the last statement in function definition indicates the end of function block and that program flow "returns" to the calling function. Along with returning flow control, the function can also return values to the calling function. These values can be stores in variables for further processing. This introduces a change to the function definition rules:
- Finally, the statement `return [values]` exits a function, optionally passing back a value to the calling function.

Let's also update our syntax:
```
def FUNCTION_NAME(PARAMETERS):
	# Function Code Block Starts
  # Statement(s) to be executed
  return VALUE
```

One thing to note, the `return` statement with no arguments (how we have been doing it up until this point) is the same as a `return None` statement. 

**Example:**
```
def add(x,y,z)
	return x+y+z
  
a = 1
b = 2
c = 7
result = add(a,b,c)
print("a={}, b={}, c={}, a+b+c={},".format(a, b, c, result)
```
Executing this will produce the following output:
```
a=1, b=2, c=7, a+b+c=10
```


***CHALLENGE:*** Challenge Goes Here.