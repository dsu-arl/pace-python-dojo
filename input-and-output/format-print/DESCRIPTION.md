Sometimes when we print, we want to include some more information instead of just the value stored in a variable. This can be accomplished in a couple different ways. The first way is simply adding multiple strings together. We just need to use commas to separate each thing we want to print. Using the `name` variable we defined in the previous challenge, we could print a message before we print the value of `name` by doing something like this:
```python
print("Name is defined as", name)
```
When run, the program will output the following:
```commandline
Name is defined as The Rizzler
```

This is rather straightforward, but can become messy quickly if printing multiple variables and messages. The other way we could accomplish this is by using a **format string**. This requires some different things: the variable place holders `{}`, the `.format()` function call, and the variables to be printed. Each place you have a placeholder `{}` is where a value will be printed. The order of your variables matters here - the first variable will print where the first place holder is in your string.

If we put it all together, we can create some interactive prints. Using variables we defined above, let's build out a format string:
```python
print("Hello {}, Your Total is: {}".format(name, total))
```
When running this code, we will get the following output:
```commandline
Hello The Rizzler, Your Total is: 1024.67
```


#### Challenge:
Use python to create and print a variable with `.format`

1. Create a new file with the file extension `.py`
2. Create a python variable that contains a name
2. Write the python code to print the text `Hello, <name>` where `<name>` is the name stored in a variable
3. Test your code with `python yourFile.py`
4. Verify your solution with `verify yourFile.py`
