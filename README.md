# python-number-and-array-programs

# Second Largest Element

numbers = []

n = int(input("Enter the number of elements: "))

for i in range(n):
    num = int(input("Enter element: "))
    numbers.append(num)

numbers.sort()

print("Second Largest Element:", numbers[-2])



# Prime Number

num = int(input("Enter a number: "))

is_prime = True

if num <= 1:
    is_prime = False
else:
    for i in range(2, num):
        if num % i == 0:
            is_prime = False
            break

if is_prime:
    print(num, "is a Prime Number")
else:
    print(num, "is not a Prime Number")



# GCD of Two Numbers

num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

gcd = 1

for i in range(1, min(num1, num2) + 1):
    if num1 % i == 0 and num2 % i == 0:
        gcd = i

print("GCD =", gcd)
