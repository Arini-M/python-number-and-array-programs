# python-number-and-array-programs

# Second Largest Element

numbers = []

n = int(input("Enter the number of elements: "))

for i in range(n):
    num = int(input("Enter element: "))
    numbers.append(num)

numbers.sort()

print("Second Largest Element:", numbers[-2])
