# Module_6_Exercises
import random
def roll_dice():
    return random.randint(1, 6)
while True:
    result = roll_dice()
    print("Dice rolled:", result)
    if result == 6:
        break
import random
def roll_dice(number_of_sides):
    return random.randint(1, number_of_sides)
sides = int(input("Enter the number of sides on the dice: "))
while True:
    result = roll_dice(sides)
    print("Dice rolled:", result)

    if result == sides:
        break
def gallons_to_liters(gallons):
    return gallons * 3.785
while True:
    gallons = float(input("Enter volume in gallons (negative number to stop): "))

    if gallons < 0:
        print("Program ended.")
        break
    liters = gallons_to_liters(gallons)
    print("Volume in liters:", liters)
def sum_of_list(numbers):
    total = 0
    for number in numbers:
        total += number
    return total
my_list = [4, 7, 12, 3, 9]
result = sum_of_list(my_list)
print("The list is:", my_list)
print("The sum of the numbers is:", result)
def remove_odd_numbers(numbers):
    even_numbers = []
    for number in numbers:
        if number % 2 == 0:
            even_numbers.append(number)
    return even_numbers
original_list = [1, 4, 7, 10, 13, 16, 19, 22]
new_list = remove_odd_numbers(original_list)
print("Original list:", original_list)
print("List without odd numbers:", new_list)
