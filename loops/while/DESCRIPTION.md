**While loops** will repeat whatever is in the loop block *while* a given condition is `true`. It checks the conditional every iteration before executing the loop block. As soon as the condition is `false`, the program control passes to the line immediately following the loop.

If it fails to turn `false`, the loop continues to run and will not stop unless forced to stop. Such loops are called infinite loops, and are not ideal in a compute program.

#### Syntax of a Python while loop:
```
while EXPRESSION:
	# statement(s) to run will EXPRESSION evaluates to true
```

**Example of a Python while loop:**
```
count = 0
while count < 5:
	count = count + 1
  print("Iteration number {}".format(count))

print("End of while loop")
```

***CHALLENGE:*** Enter Challenge Here.