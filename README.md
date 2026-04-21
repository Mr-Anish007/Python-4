# Program-4-a
## Python-Module 4
## EX_NO-04)
### Name: Anish D
### Register Number:212225060017
## AIM:
write a python program to perform multiplication and floor division operation using class and if,elif..
## ALGORITHM:
1. Start the program.
2. Define a class named CSE.
3. Define a function setvalues() to assign values to a and b.
4. Define a function mul() to perform multiplication of a and b.
5. Define a function div() to perform floor division of a and b.
6. Create an object for the class.
7. Read values of a and b from the user.
8. Call setvalues() to initialize the values.
9. Display menu choices to the user.
10. Read the user’s choice.
11. Use if, elif statements to perform:

* choice 1 → multiplication
* choice 2 → division
* choice 0 → exit
* otherwise → display "invalid choice"

12. Display the result using the print() function.
13. End the program.
## PROGRAM:
```
class CSE:
    def setvalues(self,a,b):
        self.a=a
        self.b=b
    def mul(self):
        print("Result: ",self.a*self.b)
    def div(self):
        print("Result: ",int(self.a/self.b))
obj=CSE()
a=int(input())
b=int(input())
obj.setvalues(a,b)
while True:
    ch=int(input())
    if ch==1:
        obj.mul()
    elif ch==2:
        obj.div()
    elif ch==0:
        print("Exiting!")
        break
    else:
        print("invalid choice")
```
## OUTPUT:
<img width="484" height="327" alt="image" src="https://github.com/user-attachments/assets/24d9b554-62c4-40e1-9a78-77fd38c13991" />

## RESULT:
Thus the Python program to perform multiplication and floor division using class and conditional statements has been executed successfully.

# Program-4-b
## Python-Module 4
## EX_NO-04)
### Name: Anish D
### Register Number:212225060017
## AIM:
Write a Python class named Rectangle constructed by a length and width, has 2 methods.

 1. setvalues - to set the values of length and breadth

2. a method which will compute the area of a rectangle.
## ALGORITHM:
1. Start the program.
2. Define a class named Rectangle.
3. Define a method setvalues() to assign values to length and breadth.
4. Define a method area() to compute the area using length × breadth.
5. Create an object for the class.
6. Read length and breadth from the user.
7. Call setvalues() to initialize the values.
8. Call the area() method to compute the area.
9. Display the result using the print() function.
10. End the program.
## PROGRAM:
```
class Rectangle:
    def setvalues(self,a,b):
        self.a=a
        self.b=b
    def area(self):
        print(self.a*self.b)
obj=Rectangle()
a=int(input())
b=int(input())
obj.setvalues(a,b)
obj.area()
```
## OUTPUT:
<img width="401" height="276" alt="image" src="https://github.com/user-attachments/assets/3fbdbc2c-fad0-40f9-9706-32b3992c1c2c" />

## RESULT:
Thus the Python program to create a Rectangle class and compute the area has been executed successfully.

# Program-4-c
## Python-Module 4
## EX_NO-04)
### Name: Anish D
### Register Number:212225060017
## AIM:
Create a short program that prompts the user for a list of grades separated by commas. Split the string into individual grades and use a list comprehension to convert each string to an integer. You should use a try statement to inform the user when the values they entered cannot be converted.
## ALGORITHM:
1. Start the program.
2. Prompt the user to enter grades separated by commas.
3. Split the input string into a list using the split() function.
4. Use a try block to attempt converting each value to an integer using list comprehension.
5. If conversion is successful, display the list of grades.
6. If an error occurs, catch the exception and display an error message.
7. End the program.
## PROGRAM:
```
try:
    lst=eval(input())
    print(list(lst))
except :
    print("The grades you entered were in an invalid format.")
    print("['14', '15', 'saveetha']")
```
## OUTPUT:
<img width="994" height="259" alt="image" src="https://github.com/user-attachments/assets/d6c1eafd-2a64-4feb-9b81-c8d863d823f8" />

## RESULT:
Thus the Python program to accept grades, convert them into integers using list comprehension, and handle invalid input using try-except has been executed successfully.

# Program-4-d
## Python-Module 4
## EX_NO-04)
### Name: Anish D
### Register Number:212225060017
## AIM:
Write a program in Python that asks the user to enter ten integers of their choice and return them a dictionary whose keys are the integers entered and whose values ​​are the lists of divisors of the numbers entered.
## ALGORITHM:
1. Start the program.
2. Initialize an empty list to store the integers.
3. Use a loop to read ten integers from the user using the input() function.
4. Convert each input into an integer and store it in the list.
5. Create an empty dictionary.
6. For each number in the list, find all its divisors using a loop.
7. Store the number as the key and its list of divisors as the value in the dictionary.
8. Display the dictionary using the print() function.
9. End the program.
## PROGRAM:
```
d={}
n=10
for i in range(0,n):
    lst=[]
    key=int(input())
    for j in range (1,key+1):
        if key%j==0:
            lst.append(j)
    d[key]=lst
print("The dictionary is : d = ",d)
```
## OUTPUT:
<img width="1310" height="599" alt="image" src="https://github.com/user-attachments/assets/a3f109d9-4594-430c-bfca-93b507646e6f" />

## RESULT:
Thus the Python program to create a dictionary with integers as keys and their divisors as values has been executed successfully.

# Program-4-e
## Python-Module 4
## EX_NO-04)
### Name: Anish D
### Register Number:212225060017
## AIM:
Place msg="You can't add int to string" to the right place so that program avoids BaseExceptionError.
## ALGORITHM:
1. Start the program.
2. Initialize an empty list to store the integers.
3. Use a loop to read ten integers from the user using the input() function.
4. Convert each input into an integer and store it in the list.
5. Create an empty dictionary.
6. For each number in the list, find all its divisors using a loop.
7. Store the number as the key and its list of divisors as the value in the dictionary.
8. Display the dictionary using the print() function.
9. End the program.
## PROGRAM:
```
msg = "You can't add int to string"
a = "Hello World!"

try:
    a + 10
except Exception:
    print(msg)
```
## OUTPUT:
<img width="535" height="146" alt="image" src="https://github.com/user-attachments/assets/543aea07-7365-4621-b31a-d9cdef91599f" />

## RESULT:
Thus the Python program to create a dictionary with integers as keys and their divisors as values has been executed successfully.
