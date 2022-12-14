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
11**reverse a number**<br>
num = 1234<br>
reversed_num = 0<br>
while num != 0:<br>
    digit = num % 10<br>
    reversed_num = reversed_num * 10 + digit<br>
    num //= 10<br>
print("Reversed Number: " + str(reversed_num))<br>
**output**<br>
Reversed Number: 4321<br>
12**power of a number<br>
base = 3<br>
exponent = 4<br>
result = 1<br>
while exponent != 0:<br>
    result *= base<br>
    exponent-=1<br>
print("Answer = " + str(result))<br>
**output**<br>
Answer = 81<br>
13**count down timer**<br>
import time<br>
def countdown(time_sec):<br>
    while time_sec:<br>
        mins, secs = divmod(time_sec, 60)<br>
        timeformat = '{:02d}:{:02d}'.format(mins, secs)<br>
        print(timeformat, end='\r')<br>
        time.sleep(1)<br>
        time_sec -= 1<br>
    print("stop")<br>
countdown(5)<br>
**output**<br>
stop1<br>
14**convert byte to string<br>
print(b'Easy \xE2\x9C\x85'.decode("utf-8"))<br>
**output**<br>
Easy ✅<br>
15**append the file**<br>
# Python program to merge two files<br> 
data = data2 = "" <br>
# Reading data from first file <br>
with open('file1.txt') as fp:<br> 
    data = fp.read() <br>
with open('file2.txt') as fp: <br><br>
    data2 = fp.read() <br>
# Merging two files into one another file <br><br>
data += "\n"<br>
data += data2 <br>
with open ('file3.txt', 'w') as fp:<br> 
    fp.write(data)<br>
    
    
    
    
**lablist program**
1 **breadth first search**
graph = { 
 '1' : ['2','10'], 
 '2' : ['3','8'], 
 '3' : ['4'], 
 '4' : ['5','6','7'], 
 '5' : [], 
 '6' : [], 
 '7' : [], 
 '8' : ['9'], 
 '9' : [], 
 '10' : [] 
 } 
visited = []  
queue = []  
def bfs(visited, graph, node): 
 visited.append(node) 
 queue.append(node) 
 while queue:  
  m = queue.pop(0)  
  print (m, end = " ")  
  for neighbour in graph[m]: 
   if neighbour not in visited: 
    visited.append(neighbour) 
    queue.append(neighbour) 
print("Following is the Breadth-First Search")
bfs(visited, graph, '1')  

**output**
Following is the Breadth-First Search
1 2 10 3 8 4 9 5 6 7 

2 **depth first search**
# Using a Python dictionary to act as an adjacency list
graph = {
 '5' : ['3','7'], 
 '3' : ['2', '4'], 
 '7' : ['6'], 
 '6': [], 
 '2' : ['1'], 
 '1':[], 
 '4' : ['8'], 
 '8' : [] 
} 
visited = set() # Set to keep track of visited nodes of graph.
def dfs(visited, graph, node): #function for dfs  
  if node not in visited: 
     print (node) 
     visited.add(node) 
     for neighbour in graph[node]: 
        dfs(visited, graph, neighbour) 
# Driver Code 
print("Following is the Depth-First Search") 
dfs(visited, graph, '5')

**output**
Following is the Depth-First Search
5
3
2
1
4
8
7
6

3 ** waterjug problem**
from collections import defaultdict
jug1, jug2, aim = 4, 3, 2
visited = defaultdict(lambda: False)
def waterJugSolver(amt1, amt2):
 if (amt1 == aim and amt2 == 0) or (amt2 == aim and amt1 == 0):
  print(amt1, amt2)
  return True
 if visited[(amt1, amt2)] == False:
  print(amt1, amt2)
  visited[(amt1, amt2)] = True
  return (waterJugSolver(0, amt2) or
     waterJugSolver(amt1, 0) or
     waterJugSolver(jug1, amt2) or
     waterJugSolver(amt1, jug2) or
     waterJugSolver(amt1 + min(amt2, (jug1-amt1)),
     amt2 - min(amt2, (jug1-amt1))) or
     waterJugSolver(amt1 - min(amt1, (jug2-amt2)),
     amt2 + min(amt1, (jug2-amt2))))
 else:
  return False

print("Steps: ")
waterJugSolver(0, 0)
**output**
Steps: 
0 0
4 0
4 3
0 3
3 0
3 3
4 2
0 2
True

4**tower of hanoi**
def TowerOfHanoi(n , source, destination, auxiliary):
    if n==1:
        print ("Move disk 1 from source",source,"to destination",destination)
        return
    TowerOfHanoi(n-1, source, auxiliary, destination)
    print ("Move disk",n,"from source",source,"to destination",destination)
    TowerOfHanoi(n-1, auxiliary, destination, source)

n = 3
TowerOfHanoi(n,'A','B','C')

**output**
Move disk 1 from source A to destination B
Move disk 2 from source A to destination C
Move disk 1 from source B to destination C
Move disk 3 from source A to destination B
Move disk 1 from source C to destination A
Move disk 2 from source C to destination B
Move disk 1 from source A to destination B

5 **best first search**
from queue import PriorityQueue
import matplotlib.pyplot as plt
import networkx as nx

# for implementing BFS | returns path having lowest cost
def best_first_search(source, target, n):
  visited = [0] * n
  visited[source] = True
  pq = PriorityQueue()
  pq.put((0, source))
  while pq.empty() == False:
   u = pq.get()[1]
   print(u, end=" ") # the path having lowest cost
   if u == target:
      break

   for v, c in graph[u]:
     if visited[v] == False:
        visited[v] = True
        pq.put((c, v))
print()
# for adding edges to graph
def addedge(x, y, cost):
  graph[x].append((y, cost))
  graph[y].append((x, cost))



v = int(input("Enter the number of nodes: "))
graph = [[] for i in range(v)] # undirected Graph
e = int(input("Enter the number of edges: "))
print("Enter the edges along with their weights:")
for i in range(e):
  x, y, z = list(map(int, input().split()))
  addedge(x, y, z)

source = int(input("Enter the Source Node: "))
target = int(input("Enter the Target/Destination Node: "))
print("\nPath: ", end = "")
best_first_search(source, target, v)

**output**

Enter the number of nodes: 4
Enter the number of edges: 5
Enter the edges along with their weights:
0 1 1
0 2 1
0 3 2
2 3 2
1 3 3
Enter the Source Node: 2
Enter the Target/Destination Node: 1

Path: 2 0 1 






