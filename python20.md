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
