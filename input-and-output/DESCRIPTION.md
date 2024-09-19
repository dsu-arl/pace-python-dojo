All about learning input and output from a user on the commandline

## Printing
The first thing to learn when programming is how to print information to the screen, as a program is only useful if you can see its results. In Python, to print to the screen, we will use the `print()` function (We will cover functions in  more detail later).

### Print Syntax:
```commandline
print(STRING MESSAGE TO PRINT)
```


For Example:
```commandline
print("My Output!!")
```
When run this will display the following:
```commandline
My Output!!
```

## Variables
Programming is so much more than printing things to the screen. We need to learn how to store information and use it throughout the program: this can be accomplished with variables.

Python makes this super simple, as it doesn't care about defining the type of the variable. That is to say, you give python what you want to store and it just handles it, whereas some languages require you to explicitly declare what type it is beforehand.

For the sake of this lesson we only care about Integers (whole numbers), Floats (decimal point numbers), and Strings (words/sentences). Here is how we declare each:
```
counter = 1000          # creates an integer numeric variable
total = 1024.67		    # creates a float numeric variable
name = "The Rizzler" 	# Creates a string variable
```
Later we will learn how to use these variable throughout the program, but for now we are only concerned about declaring them correctly. The easiest way to verify varables is to print them to the screen. Thankfully, Python makes this super easy. We will use the same method (`print()`) we used in Level 1, but pass the variables into it instead of hardcoding a string.

```
print(counter)
print(total)
print(name)
```
Print out your variables, and verify they are exactly the same as what you assigned them to in your program. 

### User Input and Type Casting
Now that you understand variables, it is important to learn how to change them on the fly. This allows your program to be interactive, and can be accomplished by using user input. 

Starting with what you already know, you should be able to understand what the following does:
```
name 		= "The Rizzler"
location = "Ohio"

print("Hello, my name is", name)
print("I am from", location)
```
If you run this program repeatedly, the same output would be displayed. But what happens if you want to use a different name? Or different location? You have to open the code, change the values for each variable, save and run. This doesn't sound too bad right now, but imagine the code base was thousands of lines of python - this would not be ideal.

Because of this you need something to assign different values from the user in runtime - while the program is running. This can be accomplished with the `input()` function.

When the program encounters the `input()` function, it will wait for the user to enter data until the Enter key is pressed. The sequence of characters then get stored in a string variable for further use. The program then proceeds to run the next statement. 

*Can we have multiple flags in a single level??*
Change the code above to make use of Python's `input()` function and allow the user to enter their name and location.
```
name = input()
location = input()

print("Hello, my name is", name)
print("I am from", location)
```
Now the variables are not assigned a specific value until runtime, Every time this program is run different values can be inputed. So, the program has become truly interactive. But it brings up a couple of questions.

***How does the user know the program is waiting for input?***
The user will have no idea that the program is waiting for input. If they know what the program is supposed to be doing, it will probably be fine. But if they don't, it might appear as though the program is hanging or not responding. You can alert the user by providing a text prompt. This could be as simple as a print statement before the input line or by passing a prompt string to the input function.

These will effectively accomplish the same thing. Note: If the prompt is a seperate print line before the input call, the program will display these on two lines. If you pass the prompt to the input function, the program will display both of these on the same line. 
  ```
  print("Enter your name:")
  name = input()
  
  name = input("Enter your name: ")
  ```
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