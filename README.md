# CODE-FORCES-GRIND
all the problems i did lol


04/08/2026
To set up a 3 x 3 matrix
with 3 rows and 3 columns
grid = [input(),input(),input()]
that creates something like this
(0,0) (0,1) (0,2)
(1,0) (1,1) (1,2)
(2,0) (2,1) (2,2)

to print one of the keys type print("g[0][1]")

05/08/2026
To repeat tasks in Python 
just do 
for _ in range(x)
It is not specified in this case, so it just goes on x times
          


06/08/2026
1 Learned how to create a code to test for a prime number.
It works on the principle that by finding the square root of a number, since multiplication works in pairs, one number must be smaller than the root:

if x < 2: #prime numbers are greater than 1
        return False
    for i in range(2, int(x**0.5)+1):   
        if x % i == 0:   
            return False                
    return True           


2  The start value is inclusive, and the stop value is exclusive 
   When working with a range, for example, if I wanted to check numbers from 2 to 5
   I would do for i in range(2, 6)

3  .append creates an array in which all numbers are just added on, not replaced.

4. To have more than one input in the same line, you can do 
x, y = map(int, input("Enter two numbers: ").split())

NB: to do more than one input for words on the same line
x, y = input("Enter two words: ").split()
