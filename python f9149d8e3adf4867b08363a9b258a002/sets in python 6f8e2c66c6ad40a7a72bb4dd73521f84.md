# sets in python

## Sets in Python

In Python, a set is an unordered collection of unique elements. Sets are used to store multiple items in a single variable, where duplicates are not allowed. They are defined by enclosing elements in curly braces `{}`, separated by commas.

Sets can be useful for various operations such as removing duplicates from a list, performing mathematical set operations like union, intersection, and difference, and testing membership of an element.

Here is an example of creating a set in Python:

```python
my_set = {1, 2, 3, 4, 5}

```

To add elements to a set, you can use the `add()` method:

```python
my_set.add(6)
print(my_set)  # Output: {1, 2, 3, 4, 5, 6}

```

To remove elements from a set, you can use the `remove()` method:

```python
my_set.remove(3)
print(my_set)  # Output: {1, 2, 4, 5, 6}

```

Sets can also be created using the `set()` function:

```python
another_set = set([7, 8, 9])
print(another_set)  # Output: {7, 8, 9}

```

You can perform various set operations such as union, intersection, and difference using built-in methods or operators:

```python
set_1 = {1, 2, 3}
set_2 = {3, 4, 5}

union = set_1.union(set_2)
print(union)  # Output: {1, 2, 3, 4, 5}

intersection = set_1.intersection(set_2)
print(intersection)  # Output: {3}

difference = set_1.difference(set_2)
print(difference)  # Output: {1, 2}

```

In summary, sets in Python are an important data structure for storing unique elements and performing set operations.