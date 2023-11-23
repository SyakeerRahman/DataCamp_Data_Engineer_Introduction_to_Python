# DataCamp_Data_Engineer_Introduction_to_Python

Course Description
Python is a general-purpose programming language that is becoming ever more popular for data science. Companies worldwide are using Python to harvest insights from their data and gain a competitive edge. Unlike other Python tutorials, this course focuses on Python specifically for data science. In our Introduction to Python course, you’ll learn about powerful ways to store and manipulate data, and helpful data science tools to begin conducting your own analyses. Start DataCamp’s online Python curriculum now.

### 1. Python Basics

An introduction to the basic concepts of Python. Learn how to use Python interactively and by using a script. Create your first variables and acquaint yourself with Python's basic data types.

- [ ] Hello Python!
- [ ] When to use Python?

<img width="377" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/956abae0-2efa-4a67-a21f-77505b6691f4">

- [X] The Python Interface

Hit Run Code to run your first Python code with Datacamp and see the output!

Notice the script.py window; this is where you can type Python code to solve exercises. You can hit Run Code and Submit Answer as often as you want. If you're stuck, you can click Get Hint, and ultimately Get Solution.

You can also use the IPython Shell interactively by typing commands and hitting Enter. Here, your code will not be checked for correctness so it is a great way to experiment.

```ruby
# See what happens when you hit Run Code
print(5 / 8)

print(7 + 10)
```

- [X] Any comments?

You can also add comments to your Python scripts. Comments are important to make sure that you and others can understand what your code is about and do not run as Python code.

They start with # tag. See the comment in the editor, # Division; now it's your turn to add a comment!

```ruby
# Division
print(5 / 8)

#Addition
print(7 + 10)
```

- [X] Python as a calculator

Python is perfectly suited to do basic calculations. It can do addition, subtraction, multiplication and division.
The code in the script gives some examples.
Now it's your turn to practice!

```ruby
# Addition
print(4+5)

# Subtraction
print(5-5)

# Multiplication
print(3*5)

# Division
print(10/2)
```

- [ ] Variables and Types
- [X] Variable Assignment

In Python, a variable allows you to refer to a value with a name. To create a variable x with a value of 5, you use =, like this example:
x = 5
You can now use the name of this variable, x, instead of the actual value, 5.
Remember, = in Python means assignment, it doesn't test equality

```ruby
# Create a variable savings
savings=100

# Print out savings
print(savings)
```

- [X] Calculations with variables

You've now created a savings variable, so let's start saving!
Instead of calculating with the actual values, you can use variables instead. The savings variable you created in the previous exercise with a value of 100 is available to you.
How much money would you have saved four months from now, if you saved $10 each month?

```ruby
# Create the variables monthly_savings and num_months
monthly_savings=10
num_months=4


# Multiply monthly_savings and num_months
new_savings = monthly_savings*num_months

# Add new_savings to your savings
total_savings = savings+new_savings

# Print total_savings
print(total_savings)
```

- [X] Other variable types

In the previous exercise, you worked with the integer Python data type:

int, or integer: a number without a fractional part. savings, with the value 100, is an example of an integer.
Next to numerical data types, there are three other very common data types:

float, or floating point: a number that has both an integer and fractional part, separated by a point. 1.1, is an example of a float.
str, or string: a type to represent text. You can use single or double quotes to build a string.
bool, or boolean: a type to represent logical values. It can only be True or False (the capitalization is important!).

```ruby
# Create a variable half
half=0.5

# Create a variable intro
intro="Hello! How are you?"

# Create a variable is_good
is_good=True
```

- [X] Guess the type

To find out the type of a value or a variable that refers to that value, you can use the type() function. Suppose you've defined a variable a, but you forgot the type of this variable. To determine the type of a, simply execute:
``type(a)``
We already went ahead and created three variables: a, b and c. You can use the IPython shell to discover their type. Which of the following options is correct?

<img width="336" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/acb909c7-1fea-4161-905c-e26bb0d37796">

- [X] Operations with other types

Hugo mentioned that different types behave differently in Python.
When you sum two strings, for example, you'll get different behavior than when you sum two integers or two booleans.
In the script some variables with different types have already been created. It's up to you to use them.

```ruby
monthly_savings = 10
num_months = 12
intro = "Hello! How are you?"

# Calculate year_savings using monthly_savings and num_months
year_savings=monthly_savings*num_months

# Print the type of year_savings
print(type(year_savings))

# Assign sum of intro and intro to doubleintro
doubleintro= intro+intro

# Print out doubleintro
print(doubleintro)
```

- [X] Type conversion

Using the + operator to paste together two strings can be very useful in building custom messages.
Suppose, for example, that you've calculated your savings want to summarize the results in a string.

To do this, you'll need to explicitly convert the types of your variables. More specifically, you'll need str(), to convert a value into a string. str(savings), for example, will convert the integer savings to a string.

Similar functions such as int(), float() and bool() will help you convert Python values into any type.

```ruby
# Definition of savings and total_savings
savings = 100
total_savings = 150

# Fix the printout
print("I started with $" + str(savings) + " and now have $" + str(total_savings) + ". Awesome!")

# Definition of pi_string
pi_string = "3.1415926"

# Convert pi_string into float: pi_float
pi_float=float(pi_string)
```

- [X] Can Python handle everything?

Now that you know something more about combining different sources of information, have a look at the four Python expressions below. Which one of these will throw an error? You can always copy and paste this code in the IPython Shell to find out!

<img width="443" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/c54facd2-577f-4b5d-aa89-b31ac781f316">

### 2. Python Lists

Learn to store, access, and manipulate data in lists: the first step toward efficiently working with huge amounts of data.

- [ ] Python Lists
- [X] Create a list

As opposed to int, bool etc., a list is a compound data type; you can group values together:
``
a = "is"
b = "nice"
my_list = ["my", "list", a, b]
``
After measuring the height of your family, you decide to collect some information on the house you're living in. The areas of the different parts of your house are stored in separate variables for now, as shown in the script.

```ruby
# area variables (in square meters)
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

# Create list areas
areas = [hall, kit, liv, bed, bath]
# Print areas
print(areas)
```

- [X] Create list with different types

A list can contain any Python type. Although it's not really common, a list can also contain a mix of Python types including strings, floats, booleans, etc.

The printout of the previous exercise wasn't really satisfying. It's just a list of numbers representing the areas, but you can't tell which area corresponds to which part of your house.

The code in the editor is the start of a solution. For some of the areas, the name of the corresponding room is already placed in front. Pay attention here! "bathroom" is a string, while bath is a variable that represents the float 9.50 you specified earlier.

```ruby
# area variables (in square meters)
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

# Adapt list areas
areas = ["hallway", hall, "kitchen", kit, "living room", liv, "bedroom", bed, "bathroom", bath]

# Print areas
print(areas)
```

- [X] Select the valid list

A list can contain any Python type. But a list itself is also a Python type. That means that a list can also contain a list! Python is getting funkier by the minute, but fear not, just remember the list syntax:
``
my_list = [el1, el2, el3]
``
Can you tell which ones of the following lines of Python code are valid ways to build a list?
``
A. [1, 3, 4, 2] B. [[1, 2, 3], [4, 5, 7]] C. [1 + 2, "a" * 5, 3]
``
<img width="152" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/15f21ef5-9208-4de7-88e0-a5be034cd564">

- [X] List of lists

As a data scientist, you'll often be dealing with a lot of data, and it will make sense to group some of this data.

Instead of creating a flat list containing strings and floats, representing the names and areas of the rooms in your house, you can create a list of lists. The script in the editor can already give you an idea.

Don't get confused here: "hallway" is a string, while hall is a variable that represents the float 11.25 you specified earlier.

```ruby
# area variables (in square meters)
hall = 11.25
kit = 18.0
liv = 20.0
bed = 10.75
bath = 9.50

# house information as list of lists
house = [["hallway", hall],
         ["kitchen", kit],
         ["living room", liv],
         ["bedroom", bed],
         ["bathroom", bath]]

# Print out house
print(house)

# Print out the type of house
print(type(house))
```

- [ ] Subsetting Lists
- [X] Subset and conquer

Subsetting Python lists is a piece of cake. Take the code sample below, which creates a list x and then selects "b" from it. Remember that this is the second element, so it has index 1. You can also use negative indexing.
``
x = ["a", "b", "c", "d"]
x[1]
x[-3] # same result!
``
Remember the areas list from before, containing both strings and floats? Its definition is already in the script. Can you add the correct code to do some Python subsetting?

```ruby
# Create the areas list
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

# Print out second element from areas
print(areas[1])

# Print out last element from areas
print(areas[-1])

# Print out the area of the living room
print(areas[5])
```

- [X] Subset and calculate

After you've extracted values from a list, you can use them to perform additional calculations. Take this example, where the second and fourth element of a list x are extracted. The strings that result are pasted together using the + operator:
``
x = ["a", "b", "c", "d"]
print(x[1] + x[3])
``

```ruby
# Create the areas list
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

# Sum of kitchen and bedroom area: eat_sleep_area
eat_sleep_area = areas[3] + areas[-3]

# Print the variable eat_sleep_area
print(eat_sleep_area)
```

- [X] Slicing and dicing

Selecting single values from a list is just one part of the story. It's also possible to slice your list, which means selecting multiple elements from your list. Use the following syntax:
``
my_list[start:end]
``
The start index will be included, while the end index is not.

The code sample below shows an example. A list with "b" and "c", corresponding to indexes 1 and 2, are selected from a list x:
``
x = ["a", "b", "c", "d"]
x[1:3]
``
The elements with index 1 and 2 are included, while the element with index 3 is not.

```ruby
# Create the areas list
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

# Use slicing to create downstairs
downstairs = areas[:6]

# Use slicing to create upstairs
upstairs = areas[6:]

# Print out downstairs and upstairs
print(downstairs)
print(upstairs)
```

- [X] Slicing and dicing (2)

In the video, Hugo first discussed the syntax where you specify both where to begin and end the slice of your list:
``
my_list[begin:end]``
However, it's also possible not to specify these indexes. If you don't specify the begin index, Python figures out that you want to start your slice at the beginning of your list. If you don't specify the end index, the slice will go all the way to the last element of your list. To experiment with this, try the following commands in the IPython Shell:
``
x = ["a", "b", "c", "d"]
x[:2]
x[2:]
x[:]``

```ruby
# Create the areas list
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

# Alternative slicing to create downstairs
downstairs=areas[:6]

# Alternative slicing to create upstairs
upstairs=areas[6:]
```

- [X] Subsetting lists of lists

You saw before that a Python list can contain practically anything; even other lists! To subset lists of lists, you can use the same technique as before: square brackets. Try out the commands in the following code sample in the IPython Shell:
``
x = [["a", "b", "c"],
     ["d", "e", "f"],
     ["g", "h", "i"]]
x[2][0]
x[2][:2]
x[2]`` results in a list, that you can subset again by adding additional square brackets.

What will house[-1][1] return? house, the list of lists that you created before, is already defined for you in the workspace. You can experiment with it in the IPython Shell.

<img width="191" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/6bd1babe-7a7f-471e-842c-86cc276da6a0">

- [ ] Manipulating Lists
- [X] Replace list elements

Replacing list elements is pretty easy. Simply subset the list and assign new values to the subset. You can select single elements or you can change entire list slices at once.

Use the IPython Shell to experiment with the commands below. Can you tell what's happening and why?
``
x = ["a", "b", "c", "d"]
x[1] = "r"
x[2:] = ["s", "t"]``
For this and the following exercises, you'll continue working on the areas list that contains the names and areas of different rooms in a house.

```ruby
# Create the areas list
areas = ["hallway", 11.25, "kitchen", 18.0, "living room", 20.0, "bedroom", 10.75, "bathroom", 9.50]

# Correct the bathroom area
areas[-1] = 10.50

# Change "living room" to "chill zone"
areas[4] = "chill zone"
```

- [X] Extend a list

If you can change elements in a list, you sure want to be able to add elements to it, right? You can use the + operator:
``
x = ["a", "b", "c", "d"]
y = x + ["e", "f"]``
You just won the lottery, awesome! You decide to build a poolhouse and a garage. Can you add the information to the areas list?

```ruby
# Create the areas list (updated version)
areas = ["hallway", 11.25, "kitchen", 18.0, "chill zone", 20.0,
         "bedroom", 10.75, "bathroom", 10.50]

# Add poolhouse data to areas, new list is areas_1
areas_1 = areas + ["poolhouse", 24.5]

# Add garage data to areas_1, new list is areas_2
areas_2 = areas_1 + ["garage", 15.45]
```

- [X] Delete list elements

Finally, you can also remove elements from your list. You can do this with the del statement:
``
x = ["a", "b", "c", "d"]
del(x[1])``
Pay attention here: as soon as you remove an element from a list, the indexes of the elements that come after the deleted element all change!

The updated and extended version of areas that you've built in the previous exercises is coded below. You can copy and paste this into the IPython Shell to play around with the result.
``
areas = ["hallway", 11.25, "kitchen", 18.0,
        "chill zone", 20.0, "bedroom", 10.75,
         "bathroom", 10.50, "poolhouse", 24.5,
         "garage", 15.45]``
There was a mistake! The amount you won with the lottery is not that big after all and it looks like the poolhouse isn't going to happen. You decide to remove the corresponding string and float from the areas list.

The ; sign is used to place commands on the same line. The following two code chunks are equivalent:

# Same line
command1; command2
# Separate lines
command1
command2

Which of the code chunks will do the job for us?

<img width="224" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/eb469e6a-6008-456a-8c5b-2bf84e798130">

- [X] Inner workings of lists

At the end of the video, Hugo explained how Python lists work behind the scenes. In this exercise you'll get some hands-on experience with this.

The Python code in the script already creates a list with the name areas and a copy named areas_copy. Next, the first element in the areas_copy list is changed and the areas list is printed out. If you hit Run Code you'll see that, although you've changed areas_copy, the change also takes effect in the areas list. That's because areas and areas_copy point to the same list.

If you want to prevent changes in areas_copy from also taking effect in areas, you'll have to do a more explicit copy of the areas list. You can do this with list() or by using [:].

```ruby
# Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Create areas_copy
areas_copy = areas

# Change areas_copy
areas_copy[0] = 5.0

# Print areas
print(areas)
```

### 3. Functions and Packages

You'll learn how to use functions, methods, and packages to efficiently leverage the code that brilliant Python developers have written. The goal is to reduce the amount of code you need to solve challenging problems!

- [ ] Functions
- [X] Familiar functions

Out of the box, Python offers a bunch of built-in functions to make your life as a data scientist easier. You already know two such functions: print() and type(). You've also used the functions str(), int(), bool() and float() to switch between data types. These are built-in functions as well.

Calling a function is easy. To get the type of 3.0 and store the output as a new variable, result, you can use the following:
``
result = type(3.0)``
The general recipe for calling functions and saving the result to a variable is thus:
``
output = function_name(input)``

```ruby
# Create variables var1 and var2
var1 = [1, 2, 3, 4]
var2 = True

# Print out type of var1
print(type(var1))

# Print out length of var1
print(len(var1))

# Convert var2 to an integer: out2
out2 = int(var2)
```

- [ ] Help!

Maybe you already know the name of a Python function, but you still have to figure out how to use it. Ironically, you have to ask for information about a function with another function: help(). In IPython specifically, you can also use ? before the function name.

To get help on the max() function, for example, you can use one of these calls:
``
help(max)
?max``
Use the IPython Shell to open up the documentation on pow(). Which of the following statements is true?

<img width="443" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/9fd29cd8-8052-439c-80fb-0a5852a8fb54">

- [ ] Multiple arguments

In the previous exercise, you identified optional arguments by viewing the documentation with help(). You'll now apply this to change the behavior of the sorted() function.

Have a look at the documentation of sorted() by typing help(sorted) in the IPython Shell.

You'll see that sorted() takes three arguments: iterable, key, and reverse.

key=None means that if you don't specify the key argument, it will be None. reverse=False means that if you don't specify the reverse argument, it will be False, by default.

In this exercise, you'll only have to specify iterable and reverse, not key. The first input you pass to sorted() will be matched to the iterable argument, but what about the second input? To tell Python you want to specify reverse without changing anything about key, you can use = to assign it a new value:
``
sorted(____, reverse=____)``
Two lists have been created for you. Can you paste them together and sort them in descending order?

Note: For now, we can understand an iterable as being any collection of objects, e.g., a List.

```ruby
# Create lists first and second
first = [11.25, 18.0, 20.0]
second = [10.75, 9.50]

# Paste together first and second: full
full = first + second

# Sort full in descending order: full_sorted
full_sorted = sorted(full, reverse=True)

# Print out full_sorted
print(full_sorted)
```

- [ ] Methods
- [X] String Methods

Use the upper() method on place and store the result in place_up. Use the syntax for calling methods that you learned in the previous video.
Print out place and place_up. Did both change?
Print out the number of o's on the variable place by calling count() on place and passing the letter 'o' as an input to the method. We're talking about the variable place, not the word "place"!

```ruby
# string to experiment with: place
place = "poolhouse"

# Use upper() on place: place_up
place_up = place.upper()

# Print out place and place_up
print(place)
print(place_up)

# Print out the number of o's in place
print(place.count('o'))
```

- [X] List Methods

Strings are not the only Python types that have methods associated with them. Lists, floats, integers and booleans are also types that come packaged with a bunch of useful methods. In this exercise, you'll be experimenting with:

index(), to get the index of the first element of a list that matches its input and
count(), to get the number of times an element appears in a list.
You'll be working on the list with the area of different parts of a house: areas.

```ruby
# Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Print out the index of the element 20.0
print(areas.index(20.0))

# Print out how often 9.50 appears in areas
print(areas.count(9.50))
```

- [X] List Methods (2)

Most list methods will change the list they're called on. Examples are:

append(), that adds an element to the list it is called on,
remove(), that removes the first element of a list that matches the input, and
reverse(), that reverses the order of the elements in the list it is called on.
You'll be working on the list with the area of different parts of the house: areas.

```ruby
# Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]

# Use append twice to add poolhouse and garage size
areas.append(24.5)
areas.append(15.45)

# Print out areas
print(areas)

# Reverse the orders of the elements in areas
areas.reverse()

# Print out areas
print(areas)
```

- [ ] Packages
- [X] Import package

As a data scientist, some notions of geometry never hurt. Let's refresh some of the basics.

For a fancy clustering algorithm, you want to find the circumference, 
, and area, 
, of a circle. When the radius of the circle is r, you can calculate 
 and 
 as:
As a data scientist, some notions of geometry never hurt. Let's refresh some of the basics.

For a fancy clustering algorithm, you want to find the circumference, 
, and area, 
, of a circle. When the radius of the circle is r, you can calculate 
 and 
 as:
<img width="73" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/2d8e35cf-5e54-40d1-aab7-e58b07232bd3">

In Python, the symbol for exponentiation is **. This operator raises the number to its left to the power of the number to its right. For example 3**4 is 3 to the power of 4 and will give 81.

To use the constant pi, you'll need the math package. A variable r is already coded in the script. Fill in the code to calculate C and A and see how the print() functions create some nice printouts.

In Python, the symbol for exponentiation is **. This operator raises the number to its left to the power of the number to its right. For example 3**4 is 3 to the power of 4 and will give 81.

To use the constant pi, you'll need the math package. A variable r is already coded in the script. Fill in the code to calculate C and A and see how the print() functions create some nice printouts.

```ruby
# Import the math package
import math

# Definition of radius
r = 0.43

# Calculate C
C = 2 * r * math.pi

# Calculate A
A = math.pi * r ** 2

# Build printout
print("Circumference: " + str(C))
print("Area: " + str(A))
```

- [X] Selective import

General imports, like import math, make all functionality from the math package available to you. However, if you decide to only use a specific part of a package, you can always make your import more selective:

from math import pi
Let's say the Moon's orbit around planet Earth is a perfect circle, with a radius r (in km) that is defined in the script.

```ruby
# Import radians function of math package
from math import radians

# Definition of radius
r = 192500

# Travel distance of Moon over 12 degrees. Store in dist.
dist = r * radians(12)

# Print out dist
print(dist)
```

- [X] Different ways of importing

There are several ways to import packages and modules into Python. Depending on the import call, you'll have to use different Python code.

Suppose you want to use the function inv(), which is in the linalg subpackage of the scipy package. You want to be able to use this function as follows:
``
my_inv([[1,2], [3,4]])``
Which import statement will you need in order to run the above code without an error?

<img width="254" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/6e633f4d-1a1f-4ac2-8b13-261ab4a6f509">

### 4. NumPy

NumPy is a fundamental Python package to efficiently practice data science. Learn to work with powerful tools in the NumPy array, and get started with data exploration.

- [X] NumPy

In this chapter, we're going to dive into the world of baseball. Along the way, you'll get comfortable with the basics of numpy, a powerful package to do data science.

A list baseball has already been defined in the Python script, representing the height of some baseball players in centimeters. Can you add some code here and there to create a numpy array from it?

```ruby
# Import the numpy package as np
import numpy as np

# Create list baseball
baseball = [180, 215, 210, 210, 188, 176, 209, 200]

# Create a NumPy array from baseball: np_baseball
np_baseball = np.array(baseball)

# Print out type of np_baseball
print(type(np_baseball))
```

- [X] Your First NumPy Array

You are a huge baseball fan. You decide to call the MLB (Major League Baseball) and ask around for some more statistics on the height of the main players. They pass along data on more than a thousand players, which is stored as a regular Python list: height_in. The height is expressed in inches. Can you make a numpy array out of it and convert the units to meters?

height_in is already available and the numpy package is loaded, so you can start straight away (Source: stat.ucla.edu).

```ruby
# Import numpy
import numpy as np

# Create a numpy array from height_in: np_height_in
np_height_in = np.array(height_in)

# Print out np_height_in
print(np_height_in)

# Convert np_height_in to m: np_height_m
np_height_m = np_height_in * 0.0254

# Print np_height_m
print(np_height_m)
```

- [X] Baseball players' height

The MLB also offers to let you analyze their weight data. Again, both are available as regular Python lists: height_in and weight_lb. height_in is in inches and weight_lb is in pounds.

It's now possible to calculate the BMI of each baseball player. Python code to convert height_in to a numpy array with the correct units is already available in the workspace. Follow the instructions step by step and finish the game! height_in and weight_lb are available as regular lists.

```ruby
# Import numpy
import numpy as np

# Create array from height_in with metric units: np_height_m
np_height_m = np.array(height_in) * 0.0254

# Create array from weight_lb with metric units: np_weight_kg
np_weight_kg = np.array(weight_lb) * 0.453592

# Calculate the BMI: bmi
bmi = np_weight_kg / np_height_m ** 2

# Print out bmi
print(bmi)
```

- [ ] Baseball player's BMI

The MLB also offers to let you analyze their weight data. Again, both are available as regular Python lists: height_in and weight_lb. height_in is in inches and weight_lb is in pounds.

It's now possible to calculate the BMI of each baseball player. Python code to convert height_in to a numpy array with the correct units is already available in the workspace. Follow the instructions step by step and finish the game! height_in and weight_lb are available as regular lists.

```ruby
# Import numpy
import numpy as np

# Create array from height_in with metric units: np_height_m
np_height_m = np.array(height_in) * 0.0254

# Create array from weight_lb with metric units: np_weight_kg
np_weight_kg = np.array(weight_lb) * 0.453592

# Calculate the BMI: bmi
bmi = np_weight_kg / np_height_m ** 2

# Print out bmi
print(bmi)
```

- [ ] Lightweight baseball players

To subset both regular Python lists and numpy arrays, you can use square brackets:
``
x = [4 , 9 , 6, 3, 1]
x[1]
import numpy as np
y = np.array(x)
y[1]``
For numpy specifically, you can also use boolean numpy arrays:
``
high = y > 5
y[high]``
The code that calculates the BMI of all baseball players is already included. Follow the instructions and reveal interesting things from the data! height_in and weight_lb are available as regular lists.


- [X] NumPy Side Effects

As Hugo explained before, numpy is great for doing vector arithmetic. If you compare its functionality with regular Python lists, however, some things have changed.

First of all, numpy arrays cannot contain elements with different types. If you try to build such a list, some of the elements' types are changed to end up with a homogeneous list. This is known as type coercion.

Second, the typical arithmetic operators, such as +, -, * and / have a different meaning for regular Python lists and numpy arrays.

Have a look at this line of code:
``
np.array([True, 1, 2]) + np.array([3, 4, False])``
Can you tell which code chunk builds the exact same Python object? The numpy package is already imported as np, so you can start experimenting in the IPython Shell straight away!

<img width="275" alt="image" src="https://github.com/SyakeerRahman/DataCamp_Data_Engineer_Introduction_to_Python/assets/105381652/1f1c89cc-8e51-44b2-920f-32f3b7adec7b">

- [X] Subsetting NumPy Arrays

You've seen it with your own eyes: Python lists and numpy arrays sometimes behave differently. Luckily, there are still certainties in this world. For example, subsetting (using the square bracket notation on lists or arrays) works exactly the same. To see this for yourself, try the following lines of code in the IPython Shell:
``
x = ["a", "b", "c"]
x[1]
np_x = np.array(x)
np_x[1]``
The script in the editor already contains code that imports numpy as np, and stores both the height and weight of the MLB players as numpy arrays. height_in and weight_lb are available as regular lists.

```ruby
# Import numpy
import numpy as np

# Store weight and height lists as numpy arrays
np_weight_lb = np.array(weight_lb)
np_height_in = np.array(height_in)

# Print out the weight at index 50
print(np_weight_lb[50])

# Print out sub-array of np_height_in: index 100 up to and including index 110
print(np_height_in[100:111])
```

- [ ] 2D NumPy Arrays
- [X] Your First 2D NumPy Array

Before working on the actual MLB data, let's try to create a 2D numpy array from a small list of lists.

In this exercise, baseball is a list of lists. The main list contains 4 elements. Each of these elements is a list containing the height and the weight of 4 baseball players, in this order. baseball is already coded for you in the script.

```ruby
# Import numpy
import numpy as np

# Create baseball, a list of lists
baseball = [[180, 78.4],
            [215, 102.7],
            [210, 98.5],
            [188, 75.2]]

# Create a 2D numpy array from baseball: np_baseball
np_baseball = np.array(baseball)

# Print out the type of np_baseball
print(type(np_baseball))

# Print out the shape of np_baseball
print(np_baseball.shape)
```

- [X] Baseball data in 2D form

You have another look at the MLB data and realize that it makes more sense to restructure all this information in a 2D numpy array. This array should have 1015 rows, corresponding to the 1015 baseball players you have information on, and 2 columns (for height and weight).

The MLB was, again, very helpful and passed you the data in a different structure, a Python list of lists. In this list of lists, each sublist represents the height and weight of a single baseball player. The name of this embedded list is baseball.

Can you store the data as a 2D array to unlock numpy's extra functionality? baseball is available as a regular list of lists

```ruby
# Import numpy package
import numpy as np

# Create a 2D numpy array from baseball: np_baseball
np_baseball = np.array(baseball)

# Print out the shape of np_baseball
print(np_baseball.shape)
```

- [X] Subsetting 2D NumPy Arrays

If your 2D numpy array has a regular structure, i.e. each row and column has a fixed number of values, complicated ways of subsetting become very easy. Have a look at the code below where the elements "a" and "c" are extracted from a list of lists.
```
# regular list of lists
x = [["a", "b"], ["c", "d"]]
[x[0][0], x[1][0]]
# numpy
import numpy as np
np_x = np.array(x)
np_x[:, 0]
```
For regular Python lists, this is a real pain. For 2D numpy arrays, however, it's pretty intuitive! The indexes before the comma refer to the rows, while those after the comma refer to the columns. The : is for slicing; in this example, it tells Python to include all rows.

The code that converts the pre-loaded baseball list to a 2D numpy array is already in the script. The first column contains the players' height in inches and the second column holds player weight, in pounds. Add some lines to make the correct selections. Remember that in Python, the first element is at index 0! baseball is available as a regular list of lists.

```ruby
# Import numpy package
import numpy as np

# Create np_baseball (2 cols)
np_baseball = np.array(baseball)

# Print out the 50th row of np_baseball
print(np_baseball[49,:])

# Select the entire second column of np_baseball: np_weight_lb
np_weight_lb = np_baseball[:,1]

# Print out height of 124th player
print(np_baseball[123, 0])
```

- [X] 2D Arithmetic

Remember how you calculated the Body Mass Index for all baseball players? numpy was able to perform all calculations element-wise (i.e. element by element). For 2D numpy arrays this isn't any different! You can combine matrices with single numbers, with vectors, and with other matrices.

Execute the code below in the IPython shell and see if you understand:
```
import numpy as np
np_mat = np.array([[1, 2],
                   [3, 4],
                   [5, 6]])
np_mat * 2
np_mat + np.array([10, 10])
np_mat + np_mat
```
np_baseball is coded for you; it's again a 2D numpy array with 3 columns representing height (in inches), weight (in pounds) and age (in years). baseball is available as a regular list of lists and updated is available as 2D numpy array.

```ruby
# Import numpy package
import numpy as np

# Create np_baseball (3 cols)
np_baseball = np.array(baseball)

# Print out addition of np_baseball and updated
print(np_baseball + updated)

# Create numpy array: conversion
conversion = np.array([0.0254, 0.453592, 1])

# Print out product of np_baseball and conversion
print(np_baseball * conversion)
```

- [ ] NumPy: Basic Statistics


- [X] Average versus median

You now know how to use numpy functions to get a better feeling for your data. It basically comes down to importing numpy and then calling several simple functions on the numpy arrays:
```
import numpy as np
x = [1, 4, 8, 10, 12]
np.mean(x)
np.median(x)
```
The baseball data is available as a 2D numpy array with 3 columns (height, weight, age) and 1015 rows. The name of this numpy array is np_baseball. After restructuring the data, however, you notice that some height values are abnormally high. Follow the instructions and discover which summary statistic is best suited if you're dealing with so-called outliers. np_baseball is available.

```ruby
# Import numpy
import numpy as np

# Create np_height_in from np_baseball
np_height_in = np_baseball[:,0]

# Print out the mean of np_height_in
print(np.mean(np_height_in))

# Print out the median of np_height_in
print(np.median(np_height_in))
```

- [X] Explore the baseball data

Because the mean and median are so far apart, you decide to complain to the MLB. They find the error and send the corrected data over to you. It's again available as a 2D NumPy array np_baseball, with three columns.

The Python script in the editor already includes code to print out informative messages with the different summary statistics. Can you finish the job? np_baseball is available.

```ruby
# Import numpy
import numpy as np

# Print mean height (first column)
avg = np.mean(np_baseball[:,0])
print("Average: " + str(avg))

# Print median height. Replace 'None'
med = np.median(np_baseball[:,0])
print("Median: " + str(med))

# Print out the standard deviation on height. Replace 'None'
stddev = np.std(np_baseball[:,0])
print("Standard Deviation: " + str(stddev))

# Print out correlation between first and second column. Replace 'None'
corr = np.corrcoef(np_baseball[:,0], np_baseball[:,1])
print("Correlation: " + str(corr))
```

- [ ] Blend it all together

In the last few exercises you've learned everything there is to know about heights and weights of baseball players. Now it's time to dive into another sport: soccer.

You've contacted FIFA for some data and they handed you two lists. The lists are the following:
```
positions = ['GK', 'M', 'A', 'D', ...]
heights = [191, 184, 185, 180, ...]
```
Each element in the lists corresponds to a player. The first list, positions, contains strings representing each player's position. The possible positions are: 'GK' (goalkeeper), 'M' (midfield), 'A' (attack) and 'D' (defense). The second list, heights, contains integers representing the height of the player in cm. The first player in the lists is a goalkeeper and is pretty tall (191 cm).

You're fairly confident that the median height of goalkeepers is higher than that of other players on the soccer field. Some of your friends don't believe you, so you are determined to show them using the data you received from FIFA and your newly acquired Python skills. heights and positions are available as lists

```ruby
# Import numpy
import numpy as np

# Convert positions and heights to numpy arrays: np_positions, np_heights
np_positions = np.array(positions)
np_heights = np.array(heights)

# Heights of the goalkeepers: gk_heights
gk_heights = np_heights[np_positions == 'GK']

# Heights of the other players: other_heights
other_heights = np_heights[np_positions != 'GK']

# Print out the median height of goalkeepers. Replace 'None'
print("Median height of goalkeepers: " + str(np.median(gk_heights)))

# Print out the median height of other players. Replace 'None'
print("Median height of other players: " + str(np.median(other_heights)))
```
