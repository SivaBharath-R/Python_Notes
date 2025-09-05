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


📅 More Coming Soon...

I’ll keep updating this repo with my daily learnings in Python..
