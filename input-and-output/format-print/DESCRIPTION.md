Sometimes when we print we want to include some more information instead of just the value. This can be accomplished in a couple different ways. The first way is simply adding multiple strings together. Using the `name` variable we defined above, we could print a message before we print the value of `name` by doing something like this:
```commandline
print("Name is defined as ", name)
```
When run, the program will output the following:
```commandline
Name is defined as The Rizzler
```

This is rather straightforward, but can become messy quickly if printing multiple variables and messages.The other way we could accomplish this is by using a **format string**. This requires some different things: the variable place holders, the `.format()` function call, and the variables to be printed. The placeholders are just `{}` inside of your string.

If we put it all together, we can create some interactive prints. Using variables, we defined above let's build out a format string:
```commandline
print("Hello {}, Your Total is: {}".format(name, total))
```
When running this code, we will get the following output:
```commandline
Hello The Rizzler, Your Total is: 1024.67
```

***Challenge:*** CHALLENGE MESSAGE GOES HERE