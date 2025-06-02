# EX 6B KNAPSACK PROBLEM
## DATE:
## AIM:
To demonstrate a python program using dynamic programming for 0/1 knapsack problem.


## Algorithm
1.If there are no items or capacity is 0.

2.Return 0 (no value can be added).

3.Check the weight of the current item:

4.If it's more than the remaining capacity, skip it and move to the next item.

5.If the item can fit:

6.Include it: Add its value and reduce the weight from total capacity.

7.Exclude it: Move to the next item without including it.

8.Return the maximum of the two choices (include or exclude).

## Program:
```
# Developed by: Dharani P
# Register Number: 212222220011



def knapSack(W, wt, val, n):
  
    if n==0 or W==0:
        return 0
    if(wt[n-1]>W):
        return knapSack(W,wt,val,n-1)
    else:
        return max(val[n-1] + knapSack(W-wt[n-1],wt,val,n-1) , knapSack(W,wt,val,n-1))
    

x=int(input())
y=int(input())
W=int(input())
val=[]
wt=[]
for i in range(x):
    val.append(int(input()))
for y in range(y):
    wt.append(int(input()))

n = len(val)
print('The maximum value that can be put in a knapsack of capacity W is: ',knapSack(W, wt, val, n))
```

## Output:
![447235265-0df9aee2-97e1-4d62-b2e7-bd0e60e21868](https://github.com/user-attachments/assets/bd2f18cd-7023-403e-a2e8-c5a807c24080)



## Result:
Thus the program was executed successfully for finding the maximum value that can be put in a knap sack of capacity .
