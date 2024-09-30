Lastly, Python also supports **logical operators**, these allow you to combine two or more conditionals in one statement. These are the supported logical operators we care about at this time:

| Operator | Name | Example |
|---|---|---|
| and | AND | CONDITIONAL1 and CONDITIONAL2 |
| or | OR | CONDITIONAL1 or CONDITIONAL2 |

**Example ofPython Logical Operators:**
```
number = 5
print(var > 3 and var < 10)
print(var > 3 or var < 4)
```

One thing to note, logical operators can be used inside of `if` and `elif` conditionals. If you use `and` the statement evaluates to `true` only if all the conditionals are `true`. If you use `or` the statement evaluates to `true` if one of the conditionals is `true`.

#### Challenge:
Use python to write a Student Classification System

1. Create a new file with the file extension `.py`
2. Write python code that gets two integers from the user (average test score, and attendence)
3. Use conditionals with logical operators to determine a classification, under the following conditions:
   1. Average Test Score greater than or equal to 85 and an attendance greater than or equal to 90 means they are honors
   2. Average Test Score greater than or equal to 70 and an attendance greater than or equal to 75 means they are passing
   3. Anything else is falling
4. Write the python code that prints the student's classification
```bash
# Example Running of the program
python yourScript.py
Average Test Score: 90
Attendance: 95
Student is a Honors Student
```
```bash
# Another Example
python yourScript.py
Average Test Score: 15
Attendance: 5
Student is a Failing Student
```

5. Test your code with `python yourFile.py`
6. Verify your solution with `verify yourFile.py`

