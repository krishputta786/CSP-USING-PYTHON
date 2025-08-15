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

<b>9.Find the common elements in three lists.</b>

<b>code:</b>

def common(l1,l2,l3):

    c=[]
    for i in l1:
        if i in l2 and i in l3 and i not in c:
            c.append(i)
    return c
    
l1=list(map(int,input("enter list1 elements: ").split()))

l2=list(map(int,input("enter list2 elements: ").split()))

l3=list(map(int,input("enter list3 elements: ").split()))

res=common(l1,l2,l3)

print("common elements: ",res)

<b>output:</b>

<img width="857" height="85" alt="Screenshot 2025-08-15 225706" src="https://github.com/user-attachments/assets/146f5586-e711-4296-b59f-659ae16375b5" />

<b>10.Print all even numbers between 1 and 100.</b>

<b>code:</b>

def even(n):

    for i in range(1,n+1):
        if i%2==0:
            print(i,end=' ')
            
n=int(input("enter a number: "))

even(n)

<b>output:</b>

<img width="1525" height="56" alt="Screenshot 2025-08-15 230103" src="https://github.com/user-attachments/assets/608332f0-9151-4ca1-af30-6c419af66cb3" />

<b>11. Generate the Fibonacci series up to n terms.</b>

<b>code:</b>

def fibonacci(n):

    a,b=0,1
    print(a,b,end=" ")
    for i in range(2,n):
        c=a+b
        print(c,end=" ")
        a=b
        b=c
        
n=int(input("enter a number: "))

print("Fibonacci series: ",end=" ")

fibonacci(n)

<b>output:</b>

<img width="777" height="46" alt="Screenshot 2025-08-15 231622" src="https://github.com/user-attachments/assets/d034d24f-fede-4f10-a691-69b36872e212" />

<b>12. Find the GCD of two numbers.</b>

<b>code:</b>

def gcd(a,b):

    while b!=0:
        a,b=b,a%b
    return a
    
a=int(input("enter first number: "))

b=int(input("enter second number: "))

print("GCD of",a,"and",b,"is",":",gcd(a,b))

<b>output:</b>

<img width="772" height="56" alt="Screenshot 2025-08-15 232255" src="https://github.com/user-attachments/assets/ddde0abe-7c24-403a-b290-3e005ec7f882" />

<b>13. Check whether a string is a palindrome.</b>

<b>code:</b>

def palindrome(s):

    s=s.lower().replace(" ","")
    return s==s[::-1]
    
s=input("enter a string: ")

if palindrome(s):

    print(f"{s} is palindrome")

else:

    print("f{s} is not palindrome")

<b>output:</b>

<img width="756" height="46" alt="Screenshot 2025-08-15 233021" src="https://github.com/user-attachments/assets/ef4b18e9-9fe4-4e02-ab2a-b94d79042feb" />

<b>14.Find the longest substring without repeating characters.</b>

<b>code:</b>

def longest_unique_substring(s):

    longest = ""
    n = len(s)
    for i in range(n):
        current = ""
        for j in range(i, n):
            if s[j] in current:
                break
            current += s[j]
            if len(current) > len(longest):
                longest = current
    return longest

text = input("Enter a string: ")

result = longest_unique_substring(text)

print("Longest substring without repeating characters:", result)

<b>output:</b>

<img width="744" height="43" alt="Screenshot 2025-08-15 233900" src="https://github.com/user-attachments/assets/f7f289de-cb88-4cd5-be2a-db6b6af19011" />

<b>15.Calculate the sum of digits of a number until it becomes a single digit.</b>

<b>code:</b>

def sum_to_singledigit(n):

    while n>=10:
        s=0
        while n>0:
            s+=n%10
            n//=10
        n=s
    return n

n = int(input("Enter a number: "))

result = sum_to_singledigit(n)

print("Single digit sum is:", result)

<b>output:</b>

<img width="969" height="38" alt="Screenshot 2025-08-15 234723" src="https://github.com/user-attachments/assets/626a30d9-f6c4-4065-9e13-e2340aabf916" />

<b>16. Sort a list in ascending order without using sort().</b>

<b>code:</b>

def sort_list(l):

    for i in range(len(l)):
        for j in range(i,len(l)):
            if l[i]>l[j]:
                temp=l[i]
                l[i]=l[j]
                l[j]=temp
    print(' '.join(str(i) for i in l))
    
l=list(map(int,input("enter list elements: ").split()))

print("sorted list is: ",end=' ')

sort_list(l)            

<b>output:</b>

<img width="949" height="38" alt="Screenshot 2025-08-15 235744" src="https://github.com/user-attachments/assets/384eb713-2c7d-4c64-adac-87bcf53d6810" />

<b>17.Find the sum of all elements in a list.</b>

<b>code:</b>

def list_sum(l):

    s=0
    for i in l:
        s+=i
    return s
    
l=list(map(int,input("enter list elements: ").split()))

print(f"sum of elements: {list_sum(l)}")

<b>output:</b>

<img width="659" height="39" alt="Screenshot 2025-08-16 000331" src="https://github.com/user-attachments/assets/91e7e66c-058f-4d16-a48a-014b0a5eab02" />

<b>18.Take a name as input and greet the user.</b>

<b>code:</b>

def greet(s):

    print("Hello "+s)

s=input("enter your name: ")

greet(s)

<b>output:</b>

<img width="600" height="46" alt="Screenshot 2025-08-16 000643" src="https://github.com/user-attachments/assets/2e529a76-0137-4f9a-b465-416322bdd2a5" />

<b>19.Print the first 10 natural numbers using a loop.</b>

<b>code:</b>

def num(s):

    i = 1
    while i <= s:
        print(i, end=" ")
        i += 1

s=int(input("enter a number: "))

num(s)

<b>output:</b>

<img width="491" height="39" alt="Screenshot 2025-08-16 001125" src="https://github.com/user-attachments/assets/42d8b3b1-e0cf-4889-8f46-41793bf97ad9" />

<b>20.Print all numbers divisible by 3 between 1 and 50.</b>

<b>code:</b>

def num(s):

    i = 1
    while i <= s:
        if i%3==0:
            print(i, end=" ")
        i += 1

s=int(input("enter a number: "))

num(s)

<b>output:</b>

<img width="481" height="35" alt="Screenshot 2025-08-16 001400" src="https://github.com/user-attachments/assets/7f6db8f6-ce6d-41d7-a80b-baf9d5aadf76" />
