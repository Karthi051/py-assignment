# [29-9-26] python assignment

## NAME:KARTHIKEYAN K
## REG NO:212223230101

## 1.	Print all prime numbers between input range (Ex – input 20 50, prints all prime numbers between 20 and 50).

```
n=int(input())
arr=[]
for i in range(2,n+1):
    count=0
    for j in range(2,i+1):

        if i%j==0:
            count+=1

    if count==1:
        if i>20:
            arr.append(i)

print(arr)
```

```
## output:
50
[23, 29, 31, 37, 41, 43, 47]
```

## 2.	Factorial using recursion

```
def factorial(n):

    if n==0:
        return 1 
    return n*factorial(n-1)


print(factorial(int(input("Enter the number: "))))
```

```
## output:
Enter the number: 5
120
```
## 3. Square of numbers using lambda
```
n=int(input("enter the number:"))

sqa=lambda n:  n**2

print(sqa(n))
```

```
## output:
enter the number:6
36
```

## 4. Find the second largest element in a list

```
arr=list(map(int,input().split()))

arr.sort()

print(arr[len(arr)-2])
```

```
## output:
 2 3 4 5 6 6
6
```
## 5. Count frequency of characters in a string

```
val=input()
str1=val.lower()
dic={}

for i in str1:
    if i in dic:
        dic[i]+=1
    else:
        dic[i]=1

print(dic)
```

```
## output:
hello
{'h': 1, 'e': 1, 'l': 2, 'o': 1}
```
## 6. Calculate area of a circle using math library.

```
import math

n=int(input())

cir=math.pi * n**2

print(cir)
```

```
## output:
5
78.53981633974483
```
## 7. Reverse a string without using built-in reverse

```
word=input()
str=""

for ch in range(len(word)-1,-1,-1):
    str+=word[ch]

print(str)
```

```
## output:
hello karthi
ihtrak olleh
```
## 8. Remove duplicates from a list

```
arr=list(map(int,input().split()))

arr1=[]

for ch in arr:
    if ch not in arr1:
        arr1.append(ch)

print(arr1)
```

```
## output:
1 1 2 3 4 3 4 5 5
[1, 2, 3, 4, 5]
```
## 9. Merge two dictionaries

```
dict1=eval(input())
dict2=eval(input())

dict1.update(dict2)

print(dict1)
```

```
## output:
{"a": 10, "b": 20}
{"c": 30, "d": 40}
{'a': 10, 'b': 20, 'c': 30, 'd': 40}
```
## 10. Fibonacci series using recursion

```
def fibo(a,b,n):
    if n==0:
        return 0
    print(a,end=" ")

    return fibo(b,a+b,n-1)

fibo(0,1,8)
```

```
## output:
0 1 1 2 3 5 8 13 
```
