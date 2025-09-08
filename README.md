Python Full Stack Learning Journey
Welcome to my daily learning repository!
I’m currently training at Codegnan to become a Python Full Stack Developer, and here I document everything I learn — with definitions, examples, and outputs.

 Day 1 – Python Strings
 
What is a String?
A string in Python is a sequence of characters enclosed in single quotes (' '), double quotes (" "), or triple quotes (''' ''').
text1 = 'Hello'
text2 = "World"
text3 = '''Python'''
# Output: Hello, World, Python

String Operations

Concatenation (+) → Joining strings
a = "Hello"
b = "World"
print(a + " " + b)
# Output: Hello World


Repetition (*) → Repeating strings
text = "Hi "
print(text * 3)
# Output: Hi Hi Hi


Indexing & Slicing → Accessing parts of a string
word = "Python"
print(word[0])     # Output: P
print(word[-1])    # Output: n
print(word[0:4])   # Output: Pyth

String Methods
text = "  Hello World  "
print(text.upper())      # Output: HELLO WORLD
print(text.lower())      # Output: hello world
print(text.strip())      # Output: Hello World
print(text.find("World"))   # Output: 8
print(text.index("World"))  # Output: 8
print(text.count("l"))      # Output: 3

 Key Difference:
find() returns -1 if substring not found.
index() throws an error if substring not found.


DAY-2 - Python: Lists


1. Characteristics of Lists
- Ordered collection of elements
- Allows heterogeneous data types (numbers, strings, etc.)
- Mutable (can be modified after creation)
- Allows duplicate values
- Defined using square brackets [ ]

example = [10, "Python", 3.14, True]
print(example)   # Output: [10, 'Python', 3.14, True]


2. Operations on Lists
Some basic operations are: Concatenation, Repetition, Adding & Removing elements.
- Concatenation (+):
a = [1, 2]; b = [3, 4]
print(a + b)   # Output: [1, 2, 3, 4]

- Repetition (*):
x = [7, 8]
print(x * 2)   # Output: [7, 8, 7, 8]


3. Accessing Elements
Lists can be accessed using indexing and slicing.
numbers = [10, 20, 30, 40, 50]
print(numbers[0])    # Output: 10
print(numbers[-1])   # Output: 50
print(numbers[1:4])  # Output: [20, 30, 40]


4. Built-in Functions
- len(): Returns number of elements.
nums = [1, 2, 3]
print(len(nums))   # Output: 3

- max(): Returns maximum element.
marks = [85, 92, 78]
print(max(marks))   # Output: 92

- min(): Returns minimum element.
marks = [85, 92, 78]
print(min(marks))   # Output: 78

- sum(): Returns sum of elements.
nums = [1, 2, 3]
print(sum(nums))   # Output: 6


5. List Methods
- append(): Adds an element at the end.
fruits = ["apple"]
fruits.append("banana")
print(fruits)   # Output: ['apple', 'banana']

- insert(): Inserts element at index.
fruits = ["apple", "banana"]
fruits.insert(1, "cherry")
print(fruits)   # Output: ['apple', 'cherry', 'banana']

- extend(): Adds another list.
a = [1, 2]
b = [3, 4]
a.extend(b)
print(a)   # Output: [1, 2, 3, 4]

- remove(): Removes first occurrence.
nums = [1, 2, 2, 3]
nums.remove(2)
print(nums)   # Output: [1, 2, 3]

- pop(): Removes element by index (last by default).
nums = [10, 20, 30]
nums.pop()
print(nums)   # Output: [10, 20]

- clear(): Removes all elements.
nums = [1, 2, 3]
nums.clear()
print(nums)   # Output: []

- index(): Returns index of value.
fruits = ["apple", "banana"]
print(fruits.index("banana"))   # Output: 1

- count(): Counts occurrences of value.
nums = [1, 2, 2, 3]
print(nums.count(2))   # Output: 2


6. Sorting and Reversing
- sort(): Sorts in ascending order.
numbers = [4, 2, 1, 3]
numbers.sort()
print(numbers)   # Output: [1, 2, 3, 4]

- reverse(): Reverses order of elements.
numbers = [1, 2, 3, 4]
numbers.reverse()
print(numbers)   # Output: [4, 3, 2, 1]


7. Copying Lists
original = [1, 2, 3]
copy1 = original.copy()
print(copy1)   # Output: [1, 2, 3]
copy2 = original[:]
print(copy2)   # Output: [1, 2, 3]



DAY-3


Tuples in Python

Definition
A tuple is an immutable sequence type in Python that allows you to store a collection of ordered elements. Once a tuple is created, its elements cannot be modified (i.e., they cannot be added, removed, or changed).

Characteristics of Tuples
- Ordered: Elements have a defined order, and you can access elements by index.
- Immutable: Once created, elements cannot be changed, added, or removed.
- Allow Duplicates: A tuple can have multiple occurrences of the same element.
- Can store elements of different data types (int, float, string, etc.).
  
Properties of Tuples
- Defined using parentheses () or just by separating items with commas.
- The length of a tuple is fixed.
- Tuples are hashable if all elements are hashable, which makes them usable as keys in dictionaries.
  
Tuple Operations

Creation
# Creating tuples
tuple1 = (1, 2, 3)
tuple2 = ("apple", "banana", "cherry")
tuple3 = (1, "hello", 3.14)
empty_tuple = ()
single_element_tuple = (5,)  # Note the comma

# Accessing Elements
fruits = ("apple", "banana", "cherry")
print(fruits[0])    # Output: apple
print(fruits[-1])   # Output: cherry

# Slicing
numbers = (1, 2, 3, 4, 5)
print(numbers[1:4])   # Output: (2, 3, 4)
print(numbers[:3])    # Output: (1, 2, 3)

# Tuple Concatenation
tuple1 = (1, 2, 3)
tuple2 = (4, 5)
combined = tuple1 + tuple2
print(combined)    # Output: (1, 2, 3, 4, 5)

# Repetition
tuple1 = ("a", "b")
repeated = tuple1 * 3
print(repeated)    # Output: ('a', 'b', 'a', 'b', 'a', 'b')

# Membership Test
fruits = ("apple", "banana", "cherry")
print("banana" in fruits)    # Output: True
print("grape" in fruits)     # Output: False

# Tuple Unpacking
person = ("John", 25, "Engineer")
name, age, profession = person
print(name)         # Output: John
print(age)          # Output: 25
print(profession)   # Output: Engineer

# Length of Tuple
numbers = (1, 2, 3, 4, 5)
print(len(numbers))    # Output: 5

# Why Use Tuples?
- Faster than lists due to immutability.
- Protect data from accidental modifications.
- Can be used as dictionary keys if elements are hashable.
  
Example Program: Basic Tuple Operations
# Example Program to demonstrate tuple operations

# Creating tuples
fruits = ("apple", "banana", "cherry", "apple")
numbers = (1, 2, 3, 4, 5)

# Accessing elements
print("First fruit:", fruits[0])

# Slicing
print("Fruits from index 1 to 3:", fruits[1:3])

# Concatenation
combined = fruits + ("grape", "mango")
print("Combined tuple:", combined)

# Repetition
print("Repeated tuple:", ("hello",) * 2)

# Membership test
print("Is 'banana' in fruits?", "banana" in fruits)

# Tuple unpacking
name, age, profession = ("Alice", 30, "Developer")
print("Name:", name)
print("Age:", age)
print("Profession:", profession)

# Length of a tuple
print("Number of numbers:", len(numbers))
```


📅 More Coming Soon...

I’ll keep updating this repo with my daily learnings in Python..
