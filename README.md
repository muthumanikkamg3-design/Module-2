# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
~~~
a=16
print(bin(a))

~~~

## Output
<img width="1456" height="275" alt="image" src="https://github.com/user-attachments/assets/616ff551-08bf-4dac-ac7f-47c54f7a57ce" />

## Result
Thus, the program has been successfully executed


# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program

~~~
def result(a, b):
    modulo_value = a % b
    return modulo_value

a=int(input())
b=int(input())
print("modulo is", result(a, b))
~~~

## Output:

<img width="1451" height="357" alt="image" src="https://github.com/user-attachments/assets/5dc63a1d-1bec-4c45-96f8-955cb0f803c8" />

## Result
The program to return two values modulo is successful.


# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
~~~
a=int(input("a=")) 

b=int(input("b=")) 

f=lambda a,b: a+b 

print(f(a,b))
~~~
## Output
<img width="1451" height="343" alt="image" src="https://github.com/user-attachments/assets/f505e1d6-b116-46bf-9e75-0ecee0c7426b" />

## Result
Thus, the program has been successfully executed.


# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
~~~
n = int(input("Enter number of rows: "))

for i in range(n):
    num = 1

    for s in range(n - i - 1):
        print(" ", end="")

    for j in range(i + 1):
        print(num, end=" ")
        num = num * (i - j) // (j + 1)

    print()

~~~
## Sample Output
<img width="1453" height="526" alt="image" src="https://github.com/user-attachments/assets/39a4bb0d-480a-4f1d-9663-8a027ec88a99" />

## Result
Thus, the program has been successfully executed



## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
~~~
num = int(input())

temp = num
rev = 0

while temp > 0:
    rev = rev * 10 + temp % 10
    temp = temp // 10

if rev == num:
     print("The given number {} is a Palindrome".format(num))
else:
     print("The given number {} is not a Palindrome".format(num))
~~~
## Output
<img width="1460" height="333" alt="image" src="https://github.com/user-attachments/assets/8b238a74-8c62-46cd-abf9-f6c0a587c0dd" />

## Result
Thus, the program has been successfully executed .
