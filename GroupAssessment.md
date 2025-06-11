# Assessment

This document contains Object Oriented Programming: Introduction to Python Programming II practical lab exercises using Python. The exercises contains input and output of Python programs on comparisons, conditionals statement, loops,  lists, and Input

Getting Started: To retain our code and enable us to work through the exercises in the lab, we created a new Python file called: lab_week_2.py. The code is written on the file and executed to see the output using the print() function. 

# Week 2

## 1. Comparisons and Conditionals
comparison operators are use compare two or more values and conditionals help manage the sequence of a program according to these comparisons.     

### Exercise 1: Comparison Operators  
When working with Comparison statement, its always returns a Boolean value, either True or False or Yes or No is some cases. 

We check for a comparison of values using different operators to return an output of TRUE or FALSE. These are; 

| Operator | Meaning |
| ------ | ------ |
| <  | (less than) |
| >  | (greater than) |
| == | (equal)  |
| != | (not equal | 
| <= | (less than or equal to) | 
| >= | (greater than or equal to) | 

```python
#Exercise 1: Comparison Operators 
print("\n1. Comparisons and Conditionals\n".upper())

print("Exercise 1: Comparison Operators".title())

print("\nGreater Than (>)\n") #Greater Than (>)
x = 6
y = 4
is_true_greaterThan = x > y #True --> x is greater than y
is_false_greaterThan = x > 7 #False --> x is not greater than 7
print(f"{x} > {y} is {is_true_greaterThan}") 
print(f"{x} > 7 is {is_false_greaterThan}")

print("\nLess Than (<)\n") #Less Than (<)
x = 3
y = 4
is_true_lessThan = x < y # True --> 3 is Less than y
is_false_lessThan = x < 2 #False --> x is Less than 2
print(f"{x} < {y} is {is_true_lessThan}") 
print(f"{x} < 2 is {is_false_lessThan}")

print("\nEqual To (==)\n") #Equal To (==)
x = 4
y = 4
is_true_equalTo = x == y #False --> x is equal to y
is_false_equalTo = x == 2 #False --> x is not Equal to 2
print(f"{x} == {y} is {is_true_equalTo}") 
print(f"{x} == 2 is {is_false_equalTo}")

print("\nNot Equal to (!=)\n") #Not Equal to (!=)
x = 4
y = 3
is_true_notEqual = x != y #True --> x is not equal to y
is_false_notEqual = x != 4 #False --> x is Equal to 4
print(f"{x} != {y} is {is_true_notEqual}") 
print(f"{x} != 4 is {is_false_notEqual}")

print("\nLess Than or Equal to (<=)\n") #Less Than or Equal to (<=)
x = 3
y = 5
is_true_lessEqual = x <= y #True --> x is Less Than y
is_false_lessEqual = x <= 2 #False --> x is not Less than or Equal to 2
print(f"{x} <= {y} is {is_true_lessEqual}") 
print(f"{x} <= 2 is {is_false_lessEqual}")

print("\nGreater Than or Equal to (>=)\n") #Greater Than or Equal to (>=)
x = 5
y = 5
is_true_greaterEqual = x >= y #True --> x is Equal to y
is_false_greaterEqual = x >= 7 #False --> x is not Greater than or Equal to 7
print(f"{x} >= {y} is {is_true_greaterEqual}") 
print(f"{x} >= 7 is {is_false_greaterEqual}")
```
Output when run:

``` console
1. COMPARISONS AND CONDITIONALS

Exercise 1: Comparison Operators

Greater Than (>)

6 > 4 is True
6 > 7 is False

Less Than (<)

3 < 4 is True
3 < 2 is False

Equal To (==)

4 == 4 is True
4 == 2 is False

Not Equal to (!=)

4 != 3 is True
4 != 4 is False

Less Than or Equal to (<=)

3 <= 5 is True
3 <= 2 is False

Greater Than or Equal to (>=)

5 >= 5 is True
5 >= 7 is False

```

### Exercise 2: Logical Operators  
This is use to combine two or more comparison [operators](https://files.uws.aula.education/e2dacca08b52e9c50b1a0db0e04acca0practical_week_2.pdf), evalute them to return TRUE or FALSE. 

Python has three logical operators: - 
- The and operator returns True if both operands are True. 
- The or operator returns True if at least one operand is True. 
- The not-operator returns True if the operand is False and vice versa.

```python
#Exercise 2: Logical Operators 
print("\nExercise 2: Logical Operators".title()) 

age = 15
'''print("Please enter your Age = ")
age = int(input())'''
age_range_and = (age > 20) and (age < 30) # True --> age is greater than 20 and less than 30
print(f"\nWow! Age Range: AND is  {age_range_and}")


age_range_or = (age > 20) or (age < 30) # True --> age is greater than 20 or less than 30
print(f"Wow! Age Range: OR is  {age_range_or}")


age_range_not = not((age > 20) and (age < 30)) # True --> age is greater than 20 or less than 30
print(f"Wow! Age Range: NOT is  {age_range_not}")

#Exercise 3: if – Conditionals 
print("\nExercise 3: if – Conditionals".title()) 

print("\n1St conditional".title())
age = 19 
age_group = "child" 

if age > 18:                #conditional expression
    age_group = "adult"     #True --> Execute code if condition is met

print(f"The age group is {age_group}")  #Remaining code to execute

#When age is changed to below 18
print("\n2nd conditional".title())
age = 16
age_group = "child" 
if age > 18: 
    age_group = "adult" 

print(f"The age group is {age_group}")


#Exercise 4: if – else Conditionals 
print("\n#Exercise 4: if – else Conditionals".title())

print("\n1st conditional".title())
wind_speed = 30 
if wind_speed < 10: 
    print("It is a calm day") 
else: 
    print("It is a windy day") 

#When wind_speed is changed to below 10
print("\n2nd conditional".title())
wind_speed = 8
if wind_speed < 10: 
    print("It is a calm day") 
else: 
    print("It is a windy day") 

#Exercise 5: if – elif - else Conditionals 
print("\nExercise 5: if – elif - else Conditionals\n".title())

grade = 55 

if grade < 50: 
    print("You Failed") 
elif grade < 60: 
    print("You Passed") 
elif grade < 70: 
    print("You got a Good Pass") 
else: 
    print("You got an Excellent Pass")


#Exercise 6: Summary Tasks
print("\nExercise 6: Summary Tasks\n".title())

print("Task Compare Temperatures:\n") #Task Compare Temperatures: 
temperature1 = 35
temperature2 = 15

if temperature1 == temperature2:
    print("The Weather is Cool")
else:
    print("The Temperature is not stable")

#2. Python Lists 
print("\n2. Python Lists\n".upper()) 

#Exercise 1: Creating a list 
print("Exercise 1: Creating a list\n".title())

integer_list = [1, 2, 3, 4, 5] 
string_list = ["apple", "banana", "orange", "grape"] 
empty_list = [] 
list_with_different_types = [1, "two", 3.0, True] 
person_1_age = 20 
person_2_age = 30 

# creating a list based on variables 
age_list = [person_1_age, person_2_age]  
list_within_a_list = [["red", "green", "blue"], ["yellow", "orange", "purple"]] 

print("\nTask:\n") #Task: 

city_list = [ "Glasgow", "London", "Edinburgh" ]

#Exercise 2: Accessing a list 
print("\nExercise 2: Accessing a list\n".title())

second_item = string_list[1] # will store "banana" in second_item 
print(f"Second Item on the list = {second_item}")

'''does_not_exist_item = string_list[5] #code for out of range index
print(f"This an Error display {does_not_exist_item}")'''

print("\nSlicing List")
slicing_list = string_list[0:2] # will return ["apple", "banana"] 
print(f"This is called slicing a list {slicing_list}")

last_item = string_list[-1] # will store "grape" in last_item 
print(f"The last item is {last_item}")

print("\nTask:\n") #Task: 

third_item = city_list[2] #Will print Edinburgh
print(f"The Third item is {third_item}")

slicing_last = city_list[1:3] # will return ["London", "Edinburgh"] 
print(f"This will slice {slicing_last}")


#Exercise 3: Modifying a list 
print("\nExercise 3: Modifying a list\n".upper())

string_list[0] = "pear" #changing the first item in a list to pear
print(f"The modified string list is {string_list}")

string_list.append("orange") #append --> Add Item to a list  
print(f"The string list with orange is {string_list}")

print("\nTask:\n") #Task: 

city_list.append("Manchester") #Add item to the list
print(f"The City list with Manchester is {city_list}")

city_list[1] = "Birmingham"     #Changing the second item in a list 
print(f"The modified City list is {city_list}")

#Exercise 4: Summary Task
print("\nExercise 4: Summary Task\n".upper())

print(f"Task Create, Access and Modify Lists:\n")       #Task Create, Access and Modify Lists: 

colours = ["red", "blue", "black", "yellow"]
print(f"Colour list are {colours}")

second_colours = colours[1] #Second colour on the list
print(f"The second colour on the list is {second_colours}")

colours[0] = "brown"    #Modify the first colour to Brown
print(f"The modified list is {colours}")

print(f"The Colour list length is {len(colours)}")

colour_name = "red"
if colour_name in colours:
    print("Red is in the list")
else:
    print("No Red Colour")

selected_colours = colours[1:3]     #Selected colour on the list
print(f"Selected Colours are {selected_colours}")


#Python Loops
print("\nPython Loops".upper()) 

#Exercise 1: While Loops
print("\nExercise 1: While Loops\n".title())  

i = 0 
while i < 5: 
    print(i) 
    i += 1  #This means "i = i + 1"

#Exercise 2: For Loops
print("\nExercise 2: For Loops\n")      
print("\nThe fruit are: ")
for fruit in string_list: #For loop created a new variable fruit to access the item in the list
    print(fruit.capitalize()) 

#Task: Create a for loop that prints each item in the city_list list.
print("\nThe states are: ")
for state in city_list:
    print(state)


#Exercise 3: Loop Keywords: Range, break and continue
print("\n#Exercise 3: Loop Keywords: Range, break and continue")

range(0, 5) # will return [0, 1, 2, 3, 4] 
range(5) # will return [0, 1, 2, 3, 4] 
range(0, 5, 2) # will return [0, 2, 4] because the third parameter is the step size 
range(5, 0, -1) # will return [5, 4, 3, 2, 1] 

for i in range(5): #Where i is the variable which is current number
    print(i) 

print("\nBreak")

for i in range(5): 
    if i == 3: 
        break 
    print(i) 

print("\nContinue")

for i in range(5): 
    if i == 2: 
        continue 
    print(i) 

#Exercise 4: Summary Tasks 
print("\nExercise 4: Summary Tasks")

numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

for even in numbers:
    if even % 2 == 0:    #modulus operator --> it means num is divisible by 2 (making it even).
        print(f"{even} is even")

#Task – Sum of Squares
print("\n#Task – Sum of Squares")

sum_of_squares = 0
for square in range(1,6): # range of number through 1 to 5
    sum_of_squares += square ** 2 #Adds the square of each number to sum_of_squares
    print ("The sum of square = ", sum_of_squares) 

#Task – Countdown: 
print("\nTask – Countdown:")

countdown = 10 
while countdown > 0: 
    print(countdown) 
    countdown -= 1  #This means "countdown = countdown - 1"

print("Liftoff!")

'''
#4.  Obtaining User Input 
print("\n4.  Obtaining User Input \n")

#Example: Entering a basic string 

user_input = input("Enter something: ") 
print("You entered:", user_input) 

#Example: Entering a number 

age = input("How old are you? ") 
# Convert the age to an integer 
age = int(age) 
next_year_age = age + 1 
print("Next year, you'll be", next_year_age, "years old.") 

#Task: User Input and Conditional Statements 
print("\nTask: User Input and Conditional Statements ")

age = input("User's age: ")
age = int(age)

if age < 18:
    print("You are a minor")
elif age <= 65: 
    print("You are an adult")
else:
    print("You are a senior citizen")
'''

#Task: Temperature Converter 
print("Task: Temperature Converter ")

temp_unit = input("Enter the unit of temperature you want to convert (C, K, F): ").strip().upper()  # Taking user input for temperature unit

celsius_input = input("Please input your temperature = ")

celsius_input = int(celsius_input)

degree_f = (celsius_input * 1.8) + 32 # Converting to Fahrenheit
degree_k = celsius_input + 273.15

my_output = f"Welcome to the Temperature Converter! \n\nThe temperature you have entered is {celsius_input} degree Celsius.\n\nConverted Temperatures: \n{celsius_input} degree Celsius is equal to {degree_f} degree Fahrenheit. \n{celsius_input} degree Celsius is equal to {degree_k} degree Kelvin. \n\n Thank you for using the Temperature Converter!"

print(my_output)