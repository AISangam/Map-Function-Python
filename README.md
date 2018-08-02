# Map-Function-Python
## Advantage of Map FunTction:
To make you understand how map function saves a lot of time while computing some functions in python please have a look at the following function. I am writing the same function which I am writing in the code to make you synchronized.  

**Please see the arguments of map function**

<a href="https://www.codecogs.com/eqnedit.php?latex=map(function,data)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?map(function,data)" title="map(function,data)" /></a>

```
#This is the equation of the circle with the x, y and radius r
def equation_circle(x,y,r):
    return x**2 + y**2 -r**2 
```
Now if you want to calculate the equation of circle for different values of x,y and r and save the result in the list, your approach would be following
```
x =[1,2,3,4,5,6]
y=[2,3,4,5,6,7]
r =[1,1,3,3,4,5]
equation=[]
for (a, b,c) in zip(x, y,r):
     output = equation_circle(a,b,c)
     equation.append(output)  
```
See the complexity of the code. Now I am implementing the same with the help of list keeping the value of x,y and r as same
```
x =[1,2,3,4,5,6]
y=[2,3,4,5,6,7]
r =[1,1,3,3,4,5]
map(equation_circle,x,y,r)
```
See we donot need any kind of loop and no zip function is required for such. It takes two arguments. One is function and other are values which we need to provide to function.
 
## Hope you understand it.
Please see the file with extention .ipynb. You can run the file in jupyter notebook by opening the file using
```
jupyter notebook
```

