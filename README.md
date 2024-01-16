Count number of even and odd elements in Python
Here, in this page you will find the program to count number of even and odd elements in python programming language. We are given with an integer array and need to print the count of even elements and odd elements.

Example
arr[] = [11, 20, 35, 40, 53]
Even Elements count = 2 (20, 40)
Odd Elements count = 3 (11, 35, 53)
Here, we will discuss the following two methods to print the count of even elements and odd elements.

Method 1 : Using Modulo operator
Method 2 : Using Bit-wise AND operator.
Let’s discuss above two methods one by one,

Method 1 :
Take two variables, countEven=0, countOdd=0.
Iterate over the array,
Increment countEven if(arr[i]%2==0)
Otherwise increment the value of countOdd by 1.
Method 1 : Code in Python
Run
arr = [1, 7, 8, 4, 5, 16, 8]
n = len(arr)
countEven = 0
countodd = 0
for i in range(0, n):
    if arr[i]%2==0 :
        countEven += 1
    else:
        countodd += 1

print("Even Elements count : " )
print(countEven)

print("Odd Elements count : ")
print(countodd)
Output :
Even Elements count :
4
Odd Elements count :
3
Related Pages
Finding Minimum scalar product of two vectors

Finding Maximum scalar product of two vectors in an array

Find all Symmetric pairs in an array 

Find maximum product sub-array in a given array

Finding Arrays are disjoint or not

Method 2 :
In this method we will use bit-wise AND operator. By doing AND of 1 with array element, if the result comes out to be 0 then the number is even otherwise odd.

Method 2 : Code in Python
Run
arr = [1, 7, 8, 4, 5, 16, 8]
n = len(arr)
countEven = 0
countodd = 0
for i in range(0, n):
    if arr[i]&1==0 :
        countEven += 1
    else:
        countodd += 1

print("Even Elements count : " )
print(countEven)

print("Odd Elements count : ")
print(countodd)
Output :
Even Elements count :
4
Odd Elements count :
3
