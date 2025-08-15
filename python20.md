<b>1. Program to find the sum of digits.</b>

<b>code:</b>

def sum_of_digits(n):

    s=0
    for i in n:
        s+=int(i)
    return s
    
n=input("enter a number: ")

print(f"sum of digits: {sum_of_digits(n)}")

<b>output:</b>

<img width="772" height="57" alt="Screenshot 2025-08-15 213732" src="https://github.com/user-attachments/assets/58445734-94b2-4eff-8db5-437c07f4d0ae" />

<b>2.Program to find the sum of array elements.</b>

<b>code:</b>

import array as arr

elements = arr.array('i', map(int, input("Enter array elements: ").split()))

total = 0
for num in elements:
    total += num

print(f"Sum of array elements is: {total}")

<b>output:</b>

<img width="570" height="41" alt="Screenshot 2025-08-15 214454" src="https://github.com/user-attachments/assets/272c99d2-8260-4033-bfb3-786ceb52ea29" />

<b>3.Program to merge array elements.</b>

<b>code:</b>

import array as arr

m=arr.array('i')

n=int(input("enter number of arrays: "))

for i in range(n):
    ele=arr.array('i',map(int,input(f"enter array{i+1} elements: ").split()))
    m.extend(ele)

print("merged: ",m)

<b>output:</b>

<img width="610" height="107" alt="Screenshot 2025-08-15 215512" src="https://github.com/user-attachments/assets/a25b8391-3f66-4586-8110-2ee217046deb" />

<b>4)Program to find factorial of the given number?</b>

<b>code:</b>

def factorial(n):

    if n < 0:
        return "Factorial not defined for negative numbers."
    fact = 1
    for i in range(1, n+1):
        fact *= i
    return fact

n = int(input("Enter a number: "))

print(f"The factorial of {n} is: {factorial(n)}")

<b>output:</b>

<img width="628" height="40" alt="Screenshot 2025-08-15 103844" src="https://github.com/user-attachments/assets/7fdc2ca4-4951-4b04-aa6a-029b4339521c" />

<b>5.Program to check Armstrong number.</b>

<b>code:</b>

def armstrong_or_not(n):

    l=len(str(n))
    s=0
    temp=n
    while(n!=0):
        r=n%10
        s+=pow(r,l)
        n//=10
    return s==temp
    
n=int(input("enter a number: "))

if armstrong_or_not(n):

    print("It is armstrong number")
else:

    print("It is not armstrong number")


<b>output:</b>

<img width="562" height="44" alt="Screenshot 2025-08-15 220826" src="https://github.com/user-attachments/assets/08b92f06-8c59-4575-b983-d557c1d3143e" />

<b>6.program for counting the digits in a number.</b>

<b>code:</b>

def no_of_digits(n):

    if n==0:
        return 1
    count=0
    n=abs(n)
    while n>0:
        count+=1
        n//=10
    return count
    
n=int(input("enter a number: "))

print(f"The number of digits are: {no_of_digits(n)}")

<b>output:</b>

<img width="703" height="55" alt="Screenshot 2025-08-15 221822" src="https://github.com/user-attachments/assets/d8f78d87-e2f4-4c15-a0e2-149bf6ecbf15" />

<b>7.Program to append elements to the list.</b>

<b>code:</b>

def append_ele(n):

    l=[]
    for i in range(n):
        ele=int(input(f"enter ele{i+1}: "))
        l+=[ele]
    return l
    
n=int(input("enter number of elements to add: "))

print(f"The list elements are: {append_ele(n)}")

<b>output:</b>

<img width="918" height="139" alt="Screenshot 2025-08-15 223331" src="https://github.com/user-attachments/assets/56c87f21-6ef1-4b0a-a92c-b47e47aab1f5" />

<b>8.Merge two sorted lists into one sorted list without using sort().</b>

<b>code: </b>

def sort_list(l1,l2):

    l3=[]
    i,j=0,0
    while i<len(l1) and j<len(l2):
        if l1[i]<l2[j]:
            l3.append(l1[i])
            i+=1
        else:
            l3.append(l2[j])
            j+=1
    while i<len(l1):
        l3.append(l1[i])
        i+=1
    while j<len(l2):
        l3.append(l2[j])
        j+=1
    return l3

l1=list(map(int,input("enter list1 elements: ").split()))

l2=list(map(int,input("enter list1 elements: ").split()))

res=sort_list(l1,l2)

print("merged sorted list: ",res)

<b>output:</b>

<img width="721" height="54" alt="Screenshot 2025-08-15 224712" src="https://github.com/user-attachments/assets/1c2aea4c-476e-40b1-9e2b-5aa6b7368330" />

<b>

