# dictionary python

## Dictionary in Python

In Python, a dictionary is an unordered collection of key-value pairs. Dictionaries are used to store and retrieve data using keys instead of indices like in lists or tuples. They are defined by enclosing key-value pairs in curly braces `{}`, separated by commas.

Here is an example of creating a dictionary in Python:

```python
my_dict = {"name": "John", "age": 25, "country": "USA"}

```

To access values in a dictionary, you can use the corresponding key:

```python
print(my_dict["name"])  # Output: John
print(my_dict["age"])  # Output: 25
print(my_dict["country"])  # Output: USA

```

You can also modify the values of a dictionary by assigning a new value to a specific key:

```python
my_dict["age"] = 30
print(my_dict["age"])  # Output: 30

```

If a key does not exist in the dictionary, you will get a `KeyError`. To avoid this, you can use the `get()` method, which returns `None` if the key is not found:

```python
print(my_dict.get("city"))  # Output: None

```

Dictionaries also have useful built-in methods for manipulating and accessing data. Some of the commonly used methods include `keys()`, `values()`, and `items()`:

```python
keys = my_dict.keys()
print(keys)  # Output: dict_keys(['name', 'age', 'country'])

values = my_dict.values()
print(values)  # Output: dict_values(['John', 30, 'USA'])

items = my_dict.items()
print(items)  # Output: dict_items([('name', 'John'), ('age', 30), ('country', 'USA')])

```

You can iterate over the keys, values, or items of a dictionary using a `for` loop:

```python
for key in my_dict:
    print(key)  # Output: name, age, country

for value in my_dict.values():
    print(value)  # Output: John, 30, USA

for key, value in my_dict.items():
    print(key, value)  # Output: name John, age 30, country USA

```

In summary, dictionaries in Python provide a flexible way to store and retrieve data using key-value pairs. They are commonly used for mapping and organizing data in various applications.