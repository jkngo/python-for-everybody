# Exercise 6: Rewrite your pay computation with time-and-a-half for overtime and create a function called `computepay` which takes two parameters (hours and rate).
```
Enter Hours: 45
Enter Rate: 10
Pay: 475.0
```
## Solution
```
def computepay(hours, rate):
	if float(hours) > 40:
		pay = 40.0 * float(rate) + ((float(hours) - 40.0) * float(rate) * 1.5)
	else:
		pay = float(hours) * float(rate)
	print('Pay: ' + str(format(pay, '.2f')))
try:
	hours = input('Enter Hours: ')
	rate = input('Enter Rate: ')
	computepay(hours, rate)
except:
	print('Error, please enter numeric input.')
```
