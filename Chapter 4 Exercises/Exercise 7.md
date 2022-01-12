# Exercise 7: Rewrite the grade program from the previous chapter using a function called `computegrade` that takes a score as its parameter and returns a grade as a string.
```
Score  Grade
>= 0.9   A
>= 0.8   B
>= 0.7   C
>= 0.6   D
 < 0.6   F
 
 Enter score: 0.96
 A
 
 Enter score: perfect
 Bad score
 
 Enter score: 10.0
 Bad score
 
 Enter score: 0.75
 C
 
 Enter score: 0.5
 F
 ```
 Run the program repeatedly to test the various different values for input.
 
 ## Solution
```
def computegrade(score):
    if float(score) >= 0.9 and float(score) < 1.0:
        print('A')
    elif float(score) >= 0.8 and float(score) < 0.9:
	       print('B')
    elif float(score) >= 0.7 and float(score) < 0.8:
	       print('C')
    elif float(score) >= 0.6 and float(score) < 0.7:
	       print('D')
    elif float(score) >= 0.0 and float(score) < 0.6:
	       print('F')
try:
    score = input('Input a score between 0.0 and 1.0. ')
    computegrade(score)
except:
    print('Bad score')
```
