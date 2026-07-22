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
