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

📅 More Coming Soon...

I’ll keep updating this repo with my daily learnings in Pytho
