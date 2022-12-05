# Artificial-intelligence-and-machine-learning-lab

1 ** program to calculate square root of numbers<br>
# Python Program to calculate the square root<br>
# Note: change this value for a different result<br>
num = 4<br>
# To take the input from the user<br>
#num = float(input('Enter a number: '))<br>
num_sqrt = num ** 0.5<br>
print('The square root of %0.3f is %0.3f'%(num ,num_sqrt))<br>
**output**<br>
The square root of 4.000 is 2.000<br>
<br>
2 **program to solve the quadratic equation**<br>
# Solve the quadratic equation ax**2 + bx + c = 0<br>
# import complex math module<br>
import cmath<br>
a = 1<br>
b = 5<br>
c = 6<br>
# calculate the discriminant<br>
d = (b**2) - (4*a*c)<br>
# find two solutions<br>
sol1 = (-b-cmath.sqrt(d))/(2*a)<br>
sol2 = (-b+cmath.sqrt(d))/(2*a)<br>
print('The solution are {0} and {1}'.format(sol1,sol2))<br>
**output**<br>
The solution are (-3+0j) and (-2+0j)<br>
3 **program to swap the two variables**<br>
# Python program to swap two variables<br>
x = 5<br>
y = 10<br>
# To take inputs from the user<br>
#x = input('Enter value of x: ')<br>
#y = input('Enter value of y: ')<br>
# create a temporary variable and swap the values<br>
temp = x<br>
x = y<br>
y = temp<br>
print('The value of x after swapping: {}'.format(x))<br>
print('The value of y after swapping: {}'.format(y))<br>
**output**<br>
The value of x after swapping: 10<br>
The value of y after swapping: 5<br>
4 ** Python program to check if the number is an Armstrong number or not**<br>
# Python program to check if the number is an Armstrong number or not<br>
# take input from the user<br>
num = int(input("Enter a number: "))<br>
# initialize sum<br>
sum = 0<br>
# find the sum of the cube of each digit<br>
temp = num<br>
while temp > 0:<br>
   digit = temp % 10<br>
   sum += digit ** 3<br>
   temp //= 10<br>
# display the result<br>
if num == sum:<br>
   print(num,"is an Armstrong number")<br>
else:<br>
   print(num,"is not an Armstrong number")<br>
   **output**<br>
   Enter a number: 153<br>
153 is an Armstrong number<br>
5 **create a program to print the gcd of two number in python **<br>
# create a program to print the gcd of two number in python using the math.gcd() function.<br>  
import math <br> 
print(" GCD of two number 0 and 0 is ", math.gcd(0, 0)) #math.gcd(a, b), a and b are the two integer number<br> 
print(" GCD of two number 0 and 48 is ", math.gcd(0, 48))<br> 
a = 60 # assign the number to variable a<br>  
b = 48 # assign the number to variable b <br> 
print(" GCD of two number 60 and 48 is ", math.gcd(a, b)) # pass the variable a and b to math.gcd() function.<br>  
print(" GCD of two number 48 and -12 is ", math.gcd(48, -12)) # pass the integer number<br>  
print(" GCD of two number -24 and -18 is ", math.gcd(-24, -18))<br>  
print(" GCD of two number -60 and 48 is ", math.gcd(-60, 48))<br>  
**output**<br>
 GCD of two number 0 and 0 is  0<br>
 GCD of two number 0 and 48 is  48<br>
 GCD of two number 60 and 48 is  12<br>
 GCD of two number 48 and -12 is  12<br>
 GCD of two number -24 and -18 is  6<br>
 GCD of two number -60 and 48 is  12<br>
 6**Python Program to find the L.C.M. of two input number**<br>
 # Python Program to find the L.C.M. of two input number<br>
def compute_lcm(x, y):<br>
   # choose the greater number<br>
   if x > y:<br>
       greater = x<br>
   else:<br>
       greater = y<br>
   while(True):<br>
       if((greater % x == 0) and (greater % y == 0)):<br>
           lcm = greater<br>
           break<br>
       greater += 1<br>
   return lcm<br>
num1 = 4<br>
num2 = 2<br>
print("The L.C.M. is", compute_lcm(num1, num2))<br>
**output**<br>
The L.C.M. is 4<br>
7 ** python Program to transpose a matrix<br>
# Program to transpose a matrix using a nested loop<br>
X = [[12,7],<br>
    [4 ,5],<br>
    [3 ,8]]<br>
result = [[0,0,0],<br>
         [0,0,0]]<br>
# iterate through rows<br>
for i in range(len(X)):<br>
   # iterate through columns<br>
   for j in range(len(X[0])):<br>
       result[j][i] = X[i][j]<br>
for r in result:<br>
   print(r)<br>
   **output**<br>
   [12, 4, 3]<br>
[7, 5, 8]<br>
8 **python Program to add two matrices<br> 
   # Program to add two matrices using nested loop<br>
X = [[12,7,3],<br>
    [4 ,5,6],<br>
    [7 ,8,9]]<br>
Y = [[5,8,1],<br>
    [6,7,3],<br>
    [4,5,9]]<br>
result = [[0,0,0],<br>
         [0,0,0],<br>
         [0,0,0]]<br>
# iterate through rows<br>
for i in range(len(X)):<br>
   # iterate through columns<br>
   for j in range(len(X[0])):<br>
       result[i][j] = X[i][j] + Y[i][j]<br>
for r in result:<br>
   print(r)<br>
**output**<br>
[17, 15, 4]<br>
[10, 12, 9]<br>
[11, 13, 18]<br>
9 ** python program to find dictionary**<br>
dt = {5:4, 1:6, 6:3}<br>
sorted_dt = {key: value for key, value in sorted(dt.items(), key=lambda item: item[1])}<br>
print(sorted_dt)<br>
**output**<br>
{6: 3, 5: 4, 1: 6}<br>
dt = {5:4, 1:6, 6:3}<br>
sorted_dt_value = sorted(dt.values())<br>
print(sorted_dt_value)<br>
**output**<br>
[3, 4, 6]<br>
10** python program to convert string to date time**<br>
from datetime import datetime<br>
my_date_string = "Mar 11 2011 11:31AM"<br>
datetime_object = datetime.strptime(my_date_string, '%b %d %Y %I:%M%p')<br>
print(type(datetime_object))<br>
print(datetime_object)<br>
**output**<br>
<class 'datetime.datetime'><br>
2011-03-11 11:31:00<br>


