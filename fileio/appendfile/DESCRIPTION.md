# Appending Data to File 

Last challenge we learned how to 'write' data to a new file. This act created a new file and put the data we wanted into it. What happens if you want to open an already existing file and write to it without overwriting the data? You can `append` to it!

Appending data to a file will always add the data to the end of the file, to preserve all previous data. 

To append data to a file, it's as simple as switch the `read` or `write` method with the `append` method.

```python
file_object.append("This is new data!")
```

For this challenge:
1. Append data to the file `/home/hacker/my_data.txt` in python.
2. Run `/challenge/verify` to receive the flag.
