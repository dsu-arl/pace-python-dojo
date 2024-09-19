Now that you understand variables, it is important to learn how to change them on the fly. This allows your program to be interactive, and can be accomplished by using user input. 

Starting with what you already know, you should be able to understand what the following does:
```
name = "The Rizzler"
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

***Challenge:*** ENTER CHALLENGE HERE