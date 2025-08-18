PROGRAM STATEMENT-1

1. Program to find the sum of digits

num = int(input("Enter a number: "))
s = 0
while num > 0:
    s += num % 10
    num //= 10
print("Sum of digits:", s)

<img width="893" height="158" alt="image" src="https://github.com/user-attachments/assets/0b0d6cac-7a36-4fc8-84f8-6db94f635011" />

PROGRAM STATEMENT-2

2. Program to find the sum of array elements

arr = [10, 20, 30, 40]
print("Sum of array elements:", sum(arr))

<img width="885" height="75" alt="image" src="https://github.com/user-attachments/assets/f3ace52b-099f-4fd6-a8e9-39d37fc286eb" />

PROGRAM STATEMENT-3

3. Program to merge array elements

arr1 = [1, 2, 3]
arr2 = [4, 5, 6]
merged = arr1 + arr2
print("Merged Array:", merged)

<img width="886" height="137" alt="image" src="https://github.com/user-attachments/assets/6fde88c0-23c3-4cd8-acb0-8ddc2a7dee82" />

PROGRAM STATEMENT-4

4. Program to find the factorial of a number
n = int(input("Enter a number: "))
fact = 1
for i in range(1, n+1):
    fact *= i
print("Factorial:", fact)

<img width="741" height="99" alt="image" src="https://github.com/user-attachments/assets/71d0c5dd-2c58-4660-a28c-69363511132a" />

PROGRAM STATEMENT-5

5. Program to check Armstrong number

num = int(input("Enter number: "))
power = len(str(num))
s = sum(int(digit)**power for digit in str(num))
if s == num:
    print("Armstrong number")
else:
    print("Not Armstrong")

<img width="886" height="193" alt="image" src="https://github.com/user-attachments/assets/e1bee6dc-5410-4532-839b-c008b8477158" />

PROGRAM STATEMENT-6

6. Program for counting the digits in a number

num = int(input("Enter a number: "))
count = len(str(num))
print("Number of digits:", count)

<img width="885" height="145" alt="image" src="https://github.com/user-attachments/assets/fa57a98b-7477-4db1-b672-67a16aadbece" />

PROGRAM STATEMENT-7

7. Program to append elements to the list

lst = [1, 2, 3]
lst.append(4)
print("Updated list:", lst)

<img width="885" height="138" alt="image" src="https://github.com/user-attachments/assets/11379b36-e051-4f30-a2d3-c8fd1acfb4bc" />

PROGRAM STATEMENT-8

8. Merge two sorted lists into one sorted list without using sort()

a = [1, 3, 5]
b = [2, 4, 6]
i = j = 0
merged = []
while i < len(a) and j < len(b):
    if a[i] < b[j]:
        merged.append(a[i]); i += 1
    else:
        merged.append(b[j]); j += 1
merged.extend(a[i:])
merged.extend(b[j:])
print("Merged sorted list:", merged)

<img width="898" height="218" alt="image" src="https://github.com/user-attachments/assets/acf0de87-e590-4272-8c85-24c785191a09" />

PROGRAM STATEMENT-9

9. Find the common elements in three lists

a = [1, 2, 3, 4]
b = [2, 3, 5]
c = [3, 2, 6]
common = list(set(a) & set(b) & set(c))
print("Common elements:", common)

<img width="884" height="188" alt="image" src="https://github.com/user-attachments/assets/c13de8d7-323b-4e8a-84ba-b75f4466df11" />

10. Print all even numbers between 1 and 100

for i in range(2, 101, 2):
    print(i, end=" ")

<img width="890" height="151" alt="image" src="https://github.com/user-attachments/assets/14f16d25-d7d8-4093-b40d-ac33417369c1" />

PROGRAM STATEMENT-11

11. Generate the Fibonacci series up to n terms

n = int(input("Enter number of terms: "))
a, b = 0, 1
for _ in range(n):
    print(a, end=" ")
    a, b = b, a + b
<img width="890" height="202" alt="image" src="https://github.com/user-attachments/assets/b4c9f36c-6a99-4496-822f-3e035a5bbd3d" />

PROGRAM STATEMENT-12

12. Find the GCD of two numbers

import math
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
print("GCD is:", math.gcd(a, b))

<img width="884" height="182" alt="image" src="https://github.com/user-attachments/assets/6b97c09f-b8a1-4ebb-ae5d-db81320f5fcb" />

PROGRAM STATEMENT-13

13. Check whether a string is a palindrome

s = input("Enter a string: ")
if s == s[::-1]:
    print("Palindrome")
else:
    print("Not Palindrome")

<img width="884" height="208" alt="image" src="https://github.com/user-attachments/assets/252618e2-cafc-44bf-be47-1e19219e183c" />

PROGRAM STATEMENT-14

14. Find the longest substring without repeating characters

s = input("Enter a string: ")
start = 0
max_len = 0
used = {}
for i, ch in enumerate(s):
    if ch in used and start <= used[ch]:
        start = used[ch] + 1
    else:
        max_len = max(max_len, i - start + 1)
    used[ch] = i
print("Longest substring length:", max_len)

<img width="880" height="241" alt="image" src="https://github.com/user-attachments/assets/2e5d502c-5220-45c1-b2a2-828b4893e921" />

PROGRAM STATEMENT-15

15. Calculate the sum of digits of a number until it becomes a single digit

num = int(input("Enter a number: "))
while num >= 10:
    s = 0
    while num > 0:
        s += num % 10
        num //= 10
    num = s
print("Single digit sum:", num)

<img width="889" height="214" alt="image" src="https://github.com/user-attachments/assets/a0b89317-9737-442b-9c31-b64a0215bc68" />

PROGRAM STATEMENT-16

16. Sort a list in ascending order without using sort()

lst = [5, 2, 9, 1, 6]
for i in range(len(lst)):
    for j in range(i+1, len(lst)):
        if lst[i] > lst[j]:
            lst[i], lst[j] = lst[j], lst[i]
print("Sorted list:", lst)

<img width="881" height="153" alt="image" src="https://github.com/user-attachments/assets/9a29fbfe-5c15-4ef6-bf7e-f9cac1305f51" />

PROGRAM STATEMENT-17

17. Find the sum of all elements in a list

lst = [10, 20, 30, 40]
s = 0
for i in lst:
    s += i
print("Sum of elements:", s)

<img width="887" height="191" alt="image" src="https://github.com/user-attachments/assets/c3413973-d013-4210-8430-820378e576c2" />

PROGRAM STATEMENT-18

18. Take a name as input and greet the user

name = input("Enter your name: ")
print("Hello,", name + "!")

<img width="891" height="139" alt="image" src="https://github.com/user-attachments/assets/ec4d45b4-f91d-49b6-b2b6-2e5aa16290ae" />

PROGRAM STATEMENT-19

19. Print the first 10 natural numbers using a loop

for i in range(1, 11):
    print(i, end=" ")

<img width="881" height="199" alt="image" src="https://github.com/user-attachments/assets/a38df834-320e-46cd-a5a8-f21a9e76db4d" />

PROGRAM STATEMENT-20

20. Print all numbers divisible by 3 between 1 and 50

for i in range(1, 51):
    if i % 3 == 0:
        print(i, end=" ")

<img width="887" height="226" alt="image" src="https://github.com/user-attachments/assets/dd2db337-4e67-4996-9e52-843e8e207c5b" />

