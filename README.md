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
    
    
    
    
**lablist program**<br>
1 **breadth first search**<br>
graph = { <br>
 '1' : ['2','10'],<br> 
 '2' : ['3','8'],<br> 
 '3' : ['4'],<br> 
 '4' : ['5','6','7'],<br> 
 '5' : [],<br> 
 '6' : [],<br> 
 '7' : [],<br> 
 '8' : ['9'],<br> 
 '9' : [],<br> 
 '10' : []<br> 
 }<br> 
visited = []<br>  
queue = []<br>  
def bfs(visited, graph, node):<br> 
 visited.append(node)<br> 
 queue.append(node)<br> 
 while queue:<br>  
  m = queue.pop(0)<br>  
  print (m, end = " ")<br>  
  for neighbour in graph[m]:<br> 
   if neighbour not in visited:<br> 
    visited.append(neighbour)<br> 
    queue.append(neighbour)<br> 
print("Following is the Breadth-First Search")<br>
bfs(visited, graph, '1')<br>  
<br>
**output**<br>
Following is the Breadth-First Search<br>
1 2 10 3 8 4 9 5 6 7<br> 
<br>
2 **depth first search**<br>
# Using a Python dictionary to act as an adjacency list<br>
graph = {<br>
 '5' : ['3','7'],<br>
 '3' : ['2', '4'],<br> 
 '7' : ['6'],<br> 
 '6': [],<br> 
 '2' : ['1'],<br> 
 '1':[],<br> 
 '4' : ['8'],<br> 
 '8' : []<br> 
}<br> 
visited = set() # Set to keep track of visited nodes of graph.<br>
def dfs(visited, graph, node): #function for dfs<br>  
  if node not in visited:<br> 
     print (node)<br> 
     visited.add(node)<br> 
     for neighbour in graph[node]:<br> 
        dfs(visited, graph, neighbour)<br> 
# Driver Code<br> 
print("Following is the Depth-First Search")<br> 
dfs(visited, graph, '5')<br>
<br>
**output**<br>
Following is the Depth-First Search<br>
5<br>
3<br>
2<br>
1<br>
4<br>
8<br>
7<br>
6<br>
<br>
3 ** waterjug problem**<br>
from collections import defaultdict<br>
jug1, jug2, aim = 4, 3, 2<br>
visited = defaultdict(lambda: False)<br>
def waterJugSolver(amt1, amt2):<br>
 if (amt1 == aim and amt2 == 0) or (amt2 == aim and amt1 == 0):<br>
  print(amt1, amt2)<br>
  return True<br>
 if visited[(amt1, amt2)] == False:<br>
  print(amt1, amt2)<br>
  visited[(amt1, amt2)] = True<br>
  return (waterJugSolver(0, amt2) or<br>
     waterJugSolver(amt1, 0) or<br>
     waterJugSolver(jug1, amt2) or<br>
     waterJugSolver(amt1, jug2) or<br>
     waterJugSolver(amt1 + min(amt2, (jug1-amt1)),<br>
     amt2 - min(amt2, (jug1-amt1))) or<br>
     waterJugSolver(amt1 - min(amt1, (jug2-amt2)),<br>
     amt2 + min(amt1, (jug2-amt2))))<br>
 else:<br>
  return False<br>
print("Steps: ")<br>
waterJugSolver(0, 0)<br>
**output**<br>
Steps:<br> 
0 0<br>
4 0<br><br>
4 3<br>
0 3<br>
3 0<br>
3 3<br>
4 2<br>
0 2<br>
True<br>
<br>
4**tower of hanoi**<br>
def TowerOfHanoi(n , source, destination, auxiliary):<br>
    if n==1:<br>
        print ("Move disk 1 from source",source,"to destination",destination)<br>
        return<br>
    TowerOfHanoi(n-1, source, auxiliary, destination)<br>
    print ("Move disk",n,"from source",source,"to destination",destination)<br>
    TowerOfHanoi(n-1, auxiliary, destination, source)<br>
n = 3<br>
TowerOfHanoi(n,'A','B','C')<br>
<br>
**output**<br>
Move disk 1 from source A to destination B<br>
Move disk 2 from source A to destination C<br>
Move disk 1 from source B to destination C<br>
Move disk 3 from source A to destination B<br>
Move disk 1 from source C to destination A<br>
Move disk 2 from source C to destination B<br>
Move disk 1 from source A to destination B<br>
<br>
5 **best first search**<br>
from queue import PriorityQueue<br>
import matplotlib.pyplot as plt<br>
import networkx as nx<br>
# for implementing BFS | returns path having lowest cost<br>
def best_first_search(source, target, n):<br>
  visited = [0] * n<br>
  visited[source] = True<br>
  pq = PriorityQueue()<br>
  pq.put((0, source))<br>
  while pq.empty() == False:<br>
   u = pq.get()[1]<br>
   print(u, end=" ") # the path having lowest cost<br>
   if u == target:<br>
      break<br>
   for v, c in graph[u]:<br>
     if visited[v] == False:<br>
        visited[v] = True<br>
        pq.put((c, v))<br>
print()<br>
# for adding edges to graph<br>
def addedge(x, y, cost):<br>
  graph[x].append((y, cost))<br>
  graph[y].append((x, cost))<br>
v = int(input("Enter the number of nodes: "))<br>
graph = [[] for i in range(v)] # undirected Graph<br>
e = int(input("Enter the number of edges: "))<br>
print("Enter the edges along with their weights:")<br>
for i in range(e):<br>
  x, y, z = list(map(int, input().split()))<br>
  addedge(x, y, z)<br>
source = int(input("Enter the Source Node: "))<br>
target = int(input("Enter the Target/Destination Node: "))<br>
print("\nPath: ", end = "")<br>
best_first_search(source, target, v)<br>
**output**<br>
Enter the number of nodes: 4<br>
Enter the number of edges: 5<br>
Enter the edges along with their weights:<br>
0 1 1<br>
0 2 1<br>
0 3 2<br>
2 3 2<br>
1 3 3<br>
Enter the Source Node: 2<br>
Enter the Target/Destination Node: 1<br>
Path: 2 0 1<br> 
<br> 
6 **tic tac toe**<br> 
# Tic-Tac-Toe Program using<br> 
# random number in Python<br> 
<br> 
# importing all necessary libraries<br> 
import numpy as np<br> 
import random<br> 
from time import sleep<br> 
<br> 
# Creates an empty board<br> 
<br> 
<br> 
def create_board():<br> 
	return(np.array([[0, 0, 0],<br> 
					[0, 0, 0],<br> 
					[0, 0, 0]]))<br> 
<br> 
# Check for empty places on board<br> 
def possibilities(board):<br> 
	l = []<br> 
<br> 
	for i in range(len(board)):<br> 
		for j in range(len(board)):<br> 
			if board[i][j] == 0:<br> 
				l.append((i, j))<br> 
	return(l)<br> 
# Select a random place for the player<br> 
def random_place(board, player):<br> 
	selection = possibilities(board)<br> 
	current_loc = random.choice(selection)<br> 
	board[current_loc] = player<br> 
	return(board)<br> 
# Checks whether the player has three<br> 
# of their marks in a horizontal row<br> 
def row_win(board, player):<br> 
	for x in range(len(board)):<br> 
		win = True<br> 
		for y in range(len(board)):<br> 
			if board[x, y] != player:<br> 
				win = False<br> 
				continue<br> 
		if win == True:<br> 
			return(win)<br> 
	return(win)<br> 
# Checks whether the player has three<br> 
# of their marks in a vertical row<br> 
def col_win(board, player):<br> 
	for x in range(len(board)):<br> 
		win = True<br> 
		for y in range(len(board)):<br> 
			if board[y][x] != player:<br> 
				win = False<br> 
				continue<br> 
		if win == True:<br> 
			return(win)<br> 
	return(win)<br> 
# Checks whether the player has three<br> 
# of their marks in a diagonal row<br> 
def diag_win(board, player):<br> 
	win = True<br> 
	y = 0<br> 
	for x in range(len(board)):<br> 
		if board[x, x] != player:<br> 
			win = False<br> 
	if win:<br> 
		return win<br> 
	win = True<br> 
	if win:<br> 
		for x in range(len(board)):<br> 
			y = len(board) - 1 - x<br> 
			if board[x, y] != player:<br> 
				win = False<br> 
	return win<br> 
# Evaluates whether there is<br> 
# a winner or a tie<br> 
def evaluate(board):<br> 
	winner = 0<br> 
	for player in [1, 2]:<br> 
		if (row_win(board, player) or<br> 
				col_win(board, player) or<br> 
				diag_win(board, player)):<br> 
			winner = player<br> 
	if np.all(board != 0) and winner == 0:<br> 
		winner = -1<br> 
	return winner<br> 
# Main function to start the game<br> 
def play_game():<br> 
	board, winner, counter = create_board(), 0, 1<br> <br> 
	print(board)<br> 
	sleep(2)<br>
	while winner == 0:<br> 
		for player in [1, 2]:<br> 
			board = random_place(board, player)<br> 
			print("Board after " + str(counter) + " move")<br> 
			print(board)<br> 
			sleep(2)<br> 
			counter += 1<br> 
			winner = evaluate(board)<br> 
			if winner != 0:<br> 
				break<br> 
	return(winner)<br> 
# Driver Code<br> 
print("Winner is: " + str(play_game()))<br> 
**output**<br> 
[[0 0 0]<br>
 [0 0 0]<br> 
 [0 0 0]]<br> 
Board after 1 move<br> 
[[0 0 0]<br> 
 [1 0 0]<br> 
 [0 0 0]]<br> 
Board after 2 move<br> 
[[0 2 0]<br> 
 [1 0 0]<br> 
 [0 0 0]]<br> 
Board after 3 move<br> 
[[0 2 1]<br> 
 [1 0 0]<br> 
 [0 0 0]]<br> 
Board after 4 move<br> 
[[0 2 1]<br> 
 [1 0 0]<br> 
 [0 0 2]]<br> 
Board after 5 move<br> 
[[1 2 1]<br> 
 [1 0 0]<br> 
 [0 0 2]]<br> 
Board after 6 move<br> 
[[1 2 1]<br> 
 [1 0 2]<br> 
 [0 0 2]]<br> 
Board after 7 move<br> 
[[1 2 1]<br> 
 [1 1 2]<br> 
 [0 0 2]]<br> 
Board after 8 move<br> <br> 
[[1 2 1]<br> 
 [1 1 2]<br> 
 [2 0 2]]<br> 
Board after 9 move<br> 
[[1 2 1]<br> 
 [1 1 2]<br> 
 [2 1 2]]<br> <br> 
Winner is: -1<br> 
<br> 
7 **8 puzzle problem**<br> 
# Python3 program to print the path from root<br> 
# node to destination node for N*N-1 puzzle<br> 
# algorithm using Branch and Bound<br> 
# The solution assumes that instance of<br> 
# puzzle is solvable<br> 
# Importing copy for deepcopy function<br> 
import copy<br> 
# Importing the heap functions from python<br> 
# library for Priority Queue<br> 
from heapq import heappush, heappop<br> 
# This variable can be changed to change<br> 
# the program from 8 puzzle(n=3) to 15<br> 
# puzzle(n=4) to 24 puzzle(n=5)...<br> 
n = 3<br> 
# bottom, left, top, right<br> 
row = [ 1, 0, -1, 0 ]<br> 
col = [ 0, -1, 0, 1 ]<br> 
# A class for Priority Queue<br> 
class priorityQueue:<br> 
	# Constructor to initialize a<br> 
	# Priority Queue<br> 
	def __init__(self):<br> 
		self.heap = []<br> 
	# Inserts a new key 'k'<br> 
	def push(self, k):<br> 
		heappush(self.heap, k)<br> 
	# Method to remove minimum element<br> 
	# from Priority Queue<br> 
	def pop(self):<br> 
		return heappop(self.heap)<br> 
	# Method to know if the Queue is empty<br> 
	def empty(self):<br> 
		if not self.heap:<br> 
			return True<br> 
		else:<br> 
			return False<br> 
# Node structure<br> 
class node:<br> 
	def __init__(self, parent, mat, empty_tile_pos,<br> 
				cost, level):<br> 
		# Stores the parent node of the<br> 
		# current node helps in tracing<br> 
		# path when the answer is found<br> 
		self.parent = parent<br> 
		# Stores the matrix<br> 
		self.mat = mat<br> 
		# Stores the position at which the<br> 
		# empty space tile exists in the matrix<br> 
		self.empty_tile_pos = empty_tile_pos<br> 
		# Stores the number of misplaced tiles<br> 
		self.cost = cost<br> 
		# Stores the number of moves so far<br> 
		self.level = level<br> 
	# This method is defined so that the<br> 
	# priority queue is formed based on<br> 
	# the cost variable of the objects<br> 
	def __lt__(self, nxt):<br> 
		return self.cost < nxt.cost<br> 
		# Function to calculate the number of<br> 
#misplaced tiles ie. number of non-blank<br> 
#tiles not in their goal position<br> 
def calculateCost(mat, final) -> int:<br> 
	count = 0<br> 
	for i in range(n):<br> 
		for j in range(n):<br> 
			if ((mat[i][j]) and<br> 
				(mat[i][j] != final[i][j])):<br> 
				count += 1<br> 
				
	return count

def newNode(mat, empty_tile_pos, new_empty_tile_pos,<br> 
			level, parent, final) -> node:<br> 
				
	# Copy data from parent matrix to current matrix<br> 
	new_mat = copy.deepcopy(mat)<br> 

	# Move tile by 1 position<br> 
	x1 = empty_tile_pos[0]<br> 
	y1 = empty_tile_pos[1]<br> 
	x2 = new_empty_tile_pos[0]<br> 
	y2 = new_empty_tile_pos[1]<br> 
	new_mat[x1][y1], new_mat[x2][y2] = new_mat[x2][y2], new_mat[x1][y1]<br> 

	# Set number of misplaced tiles<br> 
	cost = calculateCost(new_mat, final)<br> 

	new_node = node(parent, new_mat, new_empty_tile_pos,cost, level)<br> 
	return new_node<br> 

# Function to print the N x N matrix<br> 
def printMatrix(mat):<br> 
	
	for i in range(n):<br> 
		for j in range(n):<br> 
			print("%d " % (mat[i][j]), end = " ")<br> 
			<br> 
		print()<br> 

# Function to check if (x, y) is a valid<br> 
# matrix coordinate<br> 
def isSafe(x, y):<br> 
	<br> 
	return x >= 0 and x < n and y >= 0 and y < n<br> 

# Print path from root node to destination node<br> 
def printPath(root):<br> 
	<br> 
	if root == None:<br> 
		return<br> 
	<br> 
	printPath(root.parent)<br> 
	printMatrix(root.mat)<br> 
	print()<br> 
<br> 
# Function to solve N*N - 1 puzzle algorithm<br> 
# using Branch and Bound. empty_tile_pos is<br> 
# the blank tile position in the initial state<br> 
def solve(initial, empty_tile_pos, final):<br> 
	
	# Create a priority queue to store live<br> 
	# nodes of search tree<br> 
	pq = priorityQueue()<br> 
<br> 
	# Create the root node<br> 
	cost = calculateCost(initial, final)<br> 
	root = node(None, initial,<br> 
				empty_tile_pos, cost, 0)<br> 
<br> 
	# Add root to list of live nodes<br> 
	pq.push(root)<br> 
<br> 
	# Finds a live node with least cost,<br> 
	# add its children to list of live<br> 
	# nodes and finally deletes it from<br> 
	# the list.<br> 
	while not pq.empty():<br> 
<br> 
		# Find a live node with least estimated<br> 
		# cost and delete it form the list of<br> 
		# live nodes<br> 
		minimum = pq.pop()<br> 
<br> 
		# If minimum is the an<br> swer node<br> 
		if minimum.cost == 0:
			<br> 
			# Print the path from root to<br> 
			# destination;<br> 
			printPath(minimum)<br> 
			return<br> 
<br> 
		# Generate all possible children<br> 
		for i in range(4):<br> 
			new_tile_pos = [<br> 
				minimum.empty_tile_pos[0] + row[i],<br> 
				minimum.empty_tile_pos[1] + col[i], ]<br> 
			<br> 	
			if isSafe(new_tile_pos[0], new_tile_pos[1]):<br> 
				<br> 
				# Create a child node<br> 
				child = newNode(minimum.mat,<br> 
								minimum.empty_tile_pos,<br> 
								new_tile_pos,<br> 
								minimum.level + 1,<br> 
								minimum, final,)<br> 
<br> 
				# Add child to list of live nodes<br> 
				pq.push(child)<br> 

# Driver Code<br> 
<br> 
# Initial configuration<br> 
# Value 0 is used for empty space<br> 
initial = [ [ 1, 2, 3 ],<br> 
			[ 5, 6, 0 ],<br> 
			[ 7, 8, 4 ] ]<br> 

# Solvable Final configuration<br> 
# Value 0 is used for empty space<br> 
final = [ [ 1, 2, 3 ],<br> 
		[ 5, 8, 6 ],<br> 
		[ 0, 7, 4 ] ]<br> 
<br> 
# Blank tile coordinates in<br> 
# initial configuration<br> <br> 
empty_tile_pos = [ 1, 2 ]<br> <br> 
<br> <br> 
# Function call to solve the puzzle<br> <br> 
solve(initial, empty_tile_pos, final)<br> <br> 
<br> <br> 
# This code is contributed by Kevin Joshi<br> <br> 
<br> <br> 
**output**<br> <br> 
1  2  3 <br> <br>  
5  6  0  <br> <br> 
7  8  4 <br>  
<br> 
1  2  3  <br> 
5  0  6 <br>  
7  8  4 <br>  
<br> 
1  2  3 <br>  
5  8  6 <br>  
7  0  4 <br>  
<br> 
1  2  3 <br>  
5  8  6 <br>  
0  7  4 <br> 
<br> 
8 **saLesman problem**<br> 
from sys import maxsize<br> 
from itertools import permutations<br> 
V = 4<br> 
def travellingSalesmanProblem(graph, s):<br> 
    # store all vertex apart from source vertex<br> 
    vertex = []<br> 
    for i in range(V):<br> 
        if i != s:<br> 
            vertex.append(i)<br> 
            # store minimum weight Hamiltonian Cycl<br> 
        min_path = maxsize<br> 
        next_permutation=permutations(vertex)<br> 
        for i in next_permutation:<br> 
        # store current Path weight(cost)<br> 
            current_pathweight = 0<br> 
            # compute current path weight<br> 
            k = s<br> 
            for j in i:<br> 
                current_pathweight += graph[k][j]<br> 
                k = j<br> 
            current_pathweight += graph[k][s]<br> 
                # Update minimum<br> 
            min_path = min(min_path, current_pathweight)<br> 
    return min_path<br> 
                # Driver Code<br> 
if __name__ == "__main__":<br> 
# matrix representation of graph<br> 
    graph = [[0, 10, 15, 20], [10, 0, 35, 25],<br> 
            [15, 35, 0, 30], [20, 25, 30, 0]]<br> 
    s = 0<br> 
    print(travellingSalesmanProblem(graph, s))<br> 
       <br>   <br>           
**output**<br> 
80<br> 
<br> 
**part-B machine learning**<br> 
9 ** find 1`s algorithm**<br> 
import csv<br> 
hypo=['%','%','%','%','%','%']<br> 
with open('ws.csv') as csv_file:<br> 
    readcsv = csv.reader(csv_file, delimiter=',')<br> 
    data=[]<br> 
    print("\nThe given training examples are:")<br> 
    for row in readcsv:<br> 
        print(row)<br> 
        if row[len(row)-1] =='Yes':<br> 
            data.append(row)<br> 
print("\nThe positive examples are:")<br> 
for x in data:<br> 
    print(x)<br> 
TotalExamples=len(data)<br> 
i=0<br> 
j=0<br> 
k=0<br> 
print("\nThe steps of the Find-s algorithm are\n",hypo)<br> 
list =[]<br> 
p=0<br> 
d=len(data[p])-1
for j in range(d):<br> 
    list.append(data[i][j])<br> 
hypo=list<br> 
for i in range(1,TotalExamples):<br> 
    for k in range(d):<br> 
        if hypo[k]!=data[i][k]:<br> 
            hypo[k]='?'<br> 
        else:<br> 
            hypo[k]<br> 
    print(hypo)<br> 
print("\nThe maximally specific Find-s hypothesis for the given training examples is");<br> 
list=[]<br> 
for i in range(d):<br> 
    list.append(hypo[i])<br> 
print(list)<br> 
<br> 
**output**<br> 
The given training examples are:<br> 
['Sunny', 'Warm', 'Normal', 'Strong', 'Warm', 'Same', 'Yes']<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same', 'Yes']<br> 
['Rainy', 'Cold', 'High', 'Strong', 'Warm', 'Change', 'No']<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Cool', 'Change', 'Yes']<br> 
<br> 
The positive examples are:<br> 
['Sunny', 'Warm', 'Normal', 'Strong', 'Warm', 'Same', 'Yes']<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same', 'Yes']<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Cool', 'Change', 'Yes']<br> 

The steps of the Find-s algorithm are<br> 
 ['%', '%', '%', '%', '%', '%']<br> 
['Sunny', 'Warm', '?', 'Strong', 'Warm', 'Same']<br> 
['Sunny', 'Warm', '?', 'Strong', '?', '?']<br> 
<br> 
The maximally specific Find-s hypothesis for the given training examples is<br> 
['Sunny', 'Warm', '?', 'Strong', '?', '?']<br> 
<br> 
10**candidate elimination**<br> 
import csv<br> 
with open('ws.csv') as csv_file:<br> 
#with open("ws.csv") as f:
    #csv_file=csv.reader(f)<br> 
          #data=list(csv_file)<br> 
          readcsv=csv.reader(csv_file,delimiter=',')<br> 
          data=[]<br> 
          for row in readcsv:<br> 
              data.append(row)<br> 
          s=data[1][:-1]<br> 
          g=[['?' for i in range(len(s))] for j in range(len(s))]<br> 
          for i in data:<br> 
              if[-1]=="Yes":<br> 
                for j in range(len(s)):<br> 
                   if i[j]!=s[j]:<br> 
                      s[j]='?'<br> 
                      g[j][j]='?'<br> 
              elif i[-1]=="No":<br> 
                    for j in range(len(s)):<br> 
                      if i[j]!=s[j]:
                          g[j][j]=s[j]
                      else:<br> 
                            g[j][j]="?"<br> 
              print("\nSteps of Candidate Elimination Algorithm",data.index(i)+1)<br> 
              print(s)<br> 
              print(g)<br> 
          gh=[]<br> 
          for i in g:<br> 
             for j in i:<br> 
                if j!='?':<br> 
                    gh.append(i)<br> 
                    break<br> 
          print("\nFinal specific hypothesis:\n",s)<br> 
          print("\nFinal general hypothesis:\n",gh)<br> 
<br> 
**output**<br> 
<br> 
Steps of Candidate Elimination Algorithm 1<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same']<br> 
[['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?']]<br> 
<br> 
Steps of Candidate Elimination Algorithm 2<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same']<br> 
[['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?']]<br> 
<br> 
Steps of Candidate Elimination Algorithm 3<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same']<br> 
[['Sunny', '?', '?', '?', '?', '?'], ['?', 'Warm', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', 'Same']]<br> 
<br> 
Steps of Candidate Elimination Algorithm 4<br> 
['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same']<br> 
[['Sunny', '?', '?', '?', '?', '?'], ['?', 'Warm', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', 'Same']]<br> 
<br> 
Final specific hypothesis:<br> 
 ['Sunny', 'Warm', 'High', 'Strong', 'Warm', 'Same']<br> 
<br> 
Final general hypothesis:<br> 
 [['Sunny', '?', '?', '?', '?', '?'], ['?', 'Warm', '?', '?', '?', '?'], ['?', '?', '?', '?', '?', 'Same']]<br> 





