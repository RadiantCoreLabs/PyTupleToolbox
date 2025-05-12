# PyTupleToolbox 🐍

A beginner-friendly guide to Python tuples! Learn the basics, practice examples, and master immutable sequences with simple explanations.

## What is a Tuple?
A **tuple** is an ordered, immutable (unchangeable) collection of items in Python. It's similar to a list, but once created, its elements cannot be modified.

```python
# Example Tuple
my_tuple = (1, "apple", 3.14)
Key Features ✨
Immutable: Elements cannot be added, removed, or changed after creation.

Ordered: Items have a fixed position (indexed like lists).

Heterogeneous: Can store different data types (e.g., int, str, float).

Faster than lists: Useful for fixed data that shouldn’t change.

Basic Operations
1. Creating Tuples
python
empty_tuple = ()
single_item_tuple = ("hello",)  # Note the comma!
mixed_tuple = (1, "python", True)
2. Accessing Elements
python
print(mixed_tuple[0])  # Output: 1
print(mixed_tuple[-1]) # Output: True (last item)
3. Slicing Tuples
python
numbers = (10, 20, 30, 40)
print(numbers[1:3])  # Output: (20, 30)
4. Tuple Packing/Unpacking
python
# Packing
coordinates = (4.2, 9.1)

# Unpacking
x, y = coordinates
print(x)  # Output: 4.2
Why Use Tuples?
Safety: Protect data from accidental changes.

Performance: Faster iteration than lists.

Use Cases: Storing constants, returning multiple values from functions, dictionary keys (if hashable).

Common Methods
Method	Description	Example
count()	Returns occurrences of a value.	(1, 2, 2).count(2) → 2
index()	Returns first index of a value.	(1, 2, 3).index(2) → 1
Example: Returning Multiple Values
python
def get_user():
    return ("Alice", 25, "alice@example.com")

name, age, email = get_user()
