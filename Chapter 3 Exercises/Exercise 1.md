# Exercise 1: Rewrite your pay computation to give the employee 1.5 times the hourly rate for hours worked above 40 hours.
```
Enter Hours: 45
Enter Rate: 10
Pay: 475.0
```
## Solution
```
hours = input('Enter Hours: ')
rate = input('Enter Rate: ')
if float(hours) > 40:
    pay = 40 * float(rate) + (float(hours) - 40) * (1.5 * float(rate))
else:
    pay = float(hours) * float(rate)
print ('Pay: ' + str(format(pay, '.2f')))
```
