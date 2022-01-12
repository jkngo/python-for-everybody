# Exercise 5: Write a program which prompts the user for a Celsius temperature, convert the temperature to Fahrenheit, and print out the converted temperature.

## Solution
```
celcius = input('Give me a temperature in Celsius and I will give you the same temperature in Fahrenheit\n')
fahrenheit = float(celcius) * 9/5 + 32
print(str(celcius) + 'C is ' + str(fahrenheit) + 'F.') 
```
