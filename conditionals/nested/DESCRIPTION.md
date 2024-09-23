Python also supports **nested conditional statements** which basically we can use an `if` or `if-else` statement inside of an existing `if` or `if-else` statement.

#### Python Nested Conditional Statement Syntax:
```
if EXPRESSION1:
	# statement(s) to be executed if EXPRESSION1 is true
  if EXPRESSION2:
  	# statement(s) to be executed if EXPESSION1 and EXPRESSION2 is true
```

**Example of Python Nested Conditional Statements:**
```
number = 36
print("number= ", number)

if number % 2 == 0:
	if number % 3 == 0:
  		print("Divisible by 3 and 2")
```

Again, nesting isn't just limited to `if` statements. Say we have the following example: We offer different rates of discount on different purchase prices.
	- 20% on amounts exceeding 10000
  	- 10% on amounts between 5000 - 10000
    - 5% on amounts between 1000 - 5000
    - No discounts on amounts under 1000

```
amount = 2500
print("Amount: ", amount)

if amount > 10000:
	discount = amount * 20 / 100
else:
	if amount > 5000:
  	discount = amount * 10 / 100
  else:
  	if amount  > 1000:
    	discount = amount * 5 / 100
    else:
     	discount = 0

print("Total: ", amount - discount)
```

***Challenge:*** ENTER CHALLENGE HERE.