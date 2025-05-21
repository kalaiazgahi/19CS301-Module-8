# 19CS301-Module-8

EX: 8.1  Hackerrank challenges-I

### AIM: 

To calculate simple interest given principal, rate, and time (in years), converting time from months to years if input is fractional.



### ALGORITHM:
Step 1: Start

Step 2: Input principal, rate, and time (can be fraction like 9/12)

Step 3: Convert time to float (years)

Step 4: Calculate simple interest = (principal * rate * time) / 100

Step 5: Print the simple interest

Step 6: Stop


### PROGRAM:
```
def simpleInterest(p,t,r):
    si=(p*t*r)/100
    return si
p,r,t = eval(input()),eval(input()),eval(input())    
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/8378646d-dfbd-490a-a76c-e80a2f7c7e57)



### RESULT: 

The program correctly calculates simple interest by converting time from months to years and applying the formula.

EXP.No: 8.b  Hackerrank challenges-II

### AIM: 

To write a Python program that replaces the substring between 'not' and 'poor' (inclusive) with 'good' if 'not' appears before 'poor'.

###ALGORITHM:
Step 1: Start

Step 2: Take input string

Step 3: Find the index of substring 'not'

Step 4: Find the index of substring 'poor'

Step 5: Check if 'not' occurs before 'poor' and both substrings exist

Step 6: If yes, replace the substring from 'not' to 'poor' with 'good'

Step 7: Return or print the modified string

Step 8: Stop


### PROGRAM:
```
def not_poor(str1):
    snot = str1.find('not')
    spoor = str1.find('poor')
    
    
    if spoor > snot and snot>0 and spoor>0:
        str1 = str1.replace(str1[snot:(spoor+4)], 'good')
        return str1
    else:
        return str1
print(not_poor('The lyrics is not that poor!'))       
    
```
###OUTPUT:


![image](https://github.com/user-attachments/assets/f2e9be34-63cc-479c-bc52-badfe9a9e5ff)




###RESULT: 

The program finds the first appearances of 'not' and 'poor' in the input string, and if 'not' appears before 'poor', replaces the entire 'not'...'poor' substring with 'good'.


EX: 8.3 Hackerrank challenges-III

### AIM: 

To read an integer n and print the cube of all non-negative integers less than n.

### ALGORITHM:

Step 1: Read the integer n from input.

Step 2: Iterate from 0 to n-1.

Step 3: For each number i, calculate i³ and print it.

### PROGRAM:


```
n=int(input())
l=[]
for i in range(n):
    l.append(i)
for i in l:
    print(i**3)     
```
### OUTPUT:

![image](https://github.com/user-attachments/assets/bd69dd6d-d387-4e5e-9dd4-d17d91855213)




### RESULT: 

The program correctly prints the cubes of all non-negative integers less than the given number, each on a new line.


EXP.No: 8.4  Hackerrank challenges-IV

### AIM:

To generate the first n Fibonacci numbers, cube each number using map() and a lambda function, and print the resulting list.

###ALGORITHM: 

Step 1: Start

Step 2: Read integer n

Step 3: Generate a list of first n Fibonacci numbers starting with 0

Step 4: Use map() with a lambda function to cube each Fibonacci number

Step 5: Convert the map object to a list and print it

Step 6: Stop


###PROGRAM:
```
cube = lambda x: x**3

def fibonacci(n):
    l = []
    if n==1:
        l.append(0)
        return l
        
    elif n==0:
        return l
    else:
        a=0
        b=1
        
        
        l.extend([a,b])
        for i in range(n-2):
            c=a+b
            l.append(c)
            a,b=b,c
        return l
if __name__== '__main__':
    n = int(input())
```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/65e85691-3744-4465-ab09-4a67e01ba8e6)


 

### RESULT: 

The program generates the first 5 Fibonacci numbers [0, 1, 1, 2, 3], cubes them, and prints the list [0, 1, 1, 8, 27].

EXP.No: 8.5  ASSESSMENT EXAM - VIII -SEB

### AIM:

To generate the first n Fibonacci numbers, cube each number using map() and a lambda function, and print the resulting list.

###ALGORITHM: 
Step 1: Start

Step 2: Read the number of inputs, n

Step 3: Loop through n lines of input strings

Step 4: For each string, use regex to check if it:
  
Step 5: If it matches, print "YES", else print "NO"

Step 6: Stop



###PROGRAM:
```
x=int(input())
for i in range(x):
    x=str(input())
    if x.isnumeric() ==True and x[0:1] in ['7','8','9'] and len(x)==10:
        print("YES")
    else:
        print('NO')
```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/fa530040-6eb9-4f39-aa80-3160a2362b56)


 

### RESULT: 

The program uses regular expressions to validate mobile numbers accurately as per the given conditions.




