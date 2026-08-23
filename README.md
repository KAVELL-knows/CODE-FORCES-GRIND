# CODE-FORCES-GRIND
All the problems I did lol


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
1 Learned how to create code to test for a prime number.
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


07/08/2026
learnt that if I wanted to print l10z
I would have to do l + 10 + z
NB: l*10*z would print llllllllll*z (Python does not multiply string by string)

len(word) would give 4
Nb len[4] is wrong

Let's say we did x = word and want to know what the first and last letters were
first_letter = x[0]
last_letter = x[-1]

08/08/2026
y = area // 2     #it should round down if 9/2    NB // round down  but / give the decimal 

09/08/2026
1.
y = list(map(int, input().split()))
list() is taking the results from map() and putting them into a list,
So it allows me to input 10 8 6 4 2
and saves it as y =[10, 8, 6, 4, 2]

2.
y.sort(reverse=True)
It goes through a list/array named y and sorts it in descending order.

y.sort()
It goes through a list/array named y and sorts it in ascending order.

eg 
y =[10, 8, 6, 4, 2]
y.sort()
print(y)
output would be [2, 4, 6, 8, 10]

to get rid of the [..]
print(*y) would output 2 4 6 8 10

3.
Always remember index notation with an array, so [2, 4, 6, 8, 10]
2 is the 0 position
10 is the 4th position

4. To go through each number within an array
   for num in y:
   print(num)


11/08/26
to get an absolute number/modulus, so abs
so abs(-1) = 1

12/08/2026

if I wanted to separate input by + rather than split, I can use .split('+')

int converts each item entered into an integer so that it can be sorted by .sort
then map(str, s) takes the numbers and converts them back into text [1, 2, 3] ---> ['1', '2', '3']
'+'.join puts a + between each number  printed 
NB: .join() works directly on a map object without needing to convert it into a list
However, usually to print something mapped we need to list it, so print((list(map(str, s))))
print'+'.join(list(map(str, s))) is also correct

13/08/2026

Suppose you want to count the number of A's in the word AAPLE
x = input()
countA = 0 
for char in x:        
    if char == 'A':         
        countA = countA + 1
print("CountA")


15/08/2026
The code for identifying odd numbers in a list

odd = [i for i in x if i % 2 == 1]

alternaitvely odd = [i for i in x if i % 2 != 0]

#important note
# / is for float, so it expects a decimal (ie input was float)
# % is for MOD
# // is for dividing integers ( ie your input was integers)


16/08/2026
    #str(y) changes the integer to a string
    #len checks how many digits/ characters are in the code
    #set() keeps unique values so 
    # y = 1998 
    # str(y) = "1998"
    # len(str(y)) = 4
    # set(str(y)) = 1,9,8   # gets rid of repeating value; if it were 999, I would just be 9
    # len(set(str(y))) = 3
    # we want only to run the code if the 2 lengths remain the same


    #How to slice strings
n = input
x = input()
first_half = list(map(int, x[:n]))
#this is going to the first half of th string and counts n times
# eg 2421 = 24 
#it then uses list to create [2, 4]

all(first_half[i] < second_half[i] for i in range(n))
#all checks to make sure EVERY STATEMENT IS TRUE; if one statement is false, the if statement fails. 



#HOW TO SUBSETS
p = set(str(w))
z = {'I', 'O', 'S', 'H', 'Z', 'X', 'N'}
if p.issubset(z)


17/08/2026
#How to do capitalization
#This code just takes the first letter, makes it capital, and makes all other letters lowercase
word = input().capitalize()
print(word)

#How to  make only the first letter capital and leave everything else the same
word = list(input())
word[0] = word[0].upper()  # Saves the uppercase letter
print("".join(word))       # Converts the list back to a normal word

19/08/2026
1. Always remember we are doing if statements to look for all scenarios, including if > < and = 

2. How to get the ASII value for some letter

s = input()
for i in range(len(s)):
    letter_value = ord(s[i])

3. If we want to do upper and lower
In Python, .upper() and .lower() are string methods.
This means they are specifically designed to look at a sequence of text characters and change their casing.

If we want to use upper or lower, we need to have a STRING, so input can be a LIST 


20/08/2026
Code to check for a word if the forward spelling is equal to the backward spelling

s = input()
t = input()
if s == t[::-1]:
    print("YES")
else:
    print("NO")

HOW TO READ A WORD BACKWARDS
word = "python"
reversed_word = word[::-1]

    
23/08/2026
list say you had a list of people = [2, 0 ,4, 6, 1]

and you wanted to check if 1 was in that list
you can do 
if 1 in people
          xyz          
notice 1 isnt in ""
