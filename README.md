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
   
