# Exercise 2: Rewrite your pay program using `try` and `except` so that your program handles non-numeric input gracefully by printing a message and exiting the program. The following shows two executions of the program: 
```
Enter Hours: 20
Enter Rate: nine
Error, please enter numeric input
```
```
Enter Hours: forty
Error, please enter numeric input
```
## Solution
```
inp = input('Enter Hours: ')
rate = input('Enter Rate: ')
try:
   if float(inp) > 40.0:
      pay = 40.0 * float(rate) + ((float(inp) - 40.0) * float(rate) * 1.5)
   else:
      pay = float(inp) * float(rate)
except:
   print('Error, please enter numeric input.')
```
