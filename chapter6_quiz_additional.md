# Chapter 6: Dictionaries and Sets - Additional 20 Multiple Choice Questions

## Questions 21-40

---

### Question 21
What will be the output of the following code?
```python
d = {'a': 1, 'b': 2, 'c': 3}
print(list(d.values()))
```

A) `['a', 'b', 'c']`  
B) `[1, 2, 3]`  
C) `[('a', 1), ('b', 2), ('c', 3)]`  
D) `{'a': 1, 'b': 2, 'c': 3}`

**Correct Answer: B**  
**Explanation:** The `values()` method returns a view of the dictionary's values (not keys). Converting it to a list gives `[1, 2, 3]`.

---

### Question 22
Which of the following is an immutable collection of unique values?

A) `list`  
B) `set`  
C) `frozenset`  
D) `dict`

**Correct Answer: C**  
**Explanation:** A `frozenset` is an immutable version of a set that cannot be modified after creation. Regular sets are mutable.

---

### Question 23
What happens when you try to add a duplicate element to a set?

A) A `DuplicateError` is raised  
B) The element is added again  
C) The duplicate is silently ignored  
D) The set is converted to a list

**Correct Answer: C**  
**Explanation:** Sets only contain unique values. Adding a duplicate has no effect—the set remains unchanged without raising an error.

---

### Question 24
What is the output of this code?
```python
numbers = [1, 2, 2, 3, 3, 3]
unique = set(numbers)
print(len(unique))
```

A) `6`  
B) `3`  
C) `2`  
D) `1`

**Correct Answer: B**  
**Explanation:** Converting the list to a set removes duplicates, leaving unique values: `{1, 2, 3}`, which has length 3.

---

### Question 25
Which dictionary method returns a value and removes the key-value pair from the dictionary?

A) `remove()`  
B) `pop()`  
C) `delete()`  
D) `get()`

**Correct Answer: B**  
**Explanation:** The `pop()` method removes a key and returns its associated value. If the key doesn't exist, it raises a `KeyError`.

---

### Question 26
What will be printed by this code?
```python
colors = {'red', 'green', 'blue'}
print('red' in colors)
```

A) `True`  
B) `False`  
C) `KeyError`  
D) `undefined`

**Correct Answer: A**  
**Explanation:** The `in` operator checks for membership in a set. Since 'red' is in the set, it returns `True`.

---

### Question 27
What is the result of this set operation?
```python
{1, 2, 3} - {2, 3, 4}
```

A) `{1, 2, 3, 4}`  
B) `{2, 3}`  
C) `{1}`  
D) `{4}`

**Correct Answer: C**  
**Explanation:** The `-` operator performs set difference, returning elements in the left set that are not in the right set. Only 1 is exclusive to the left set.

---

### Question 28
Which statement correctly creates an empty dictionary?

A) `d = {}`  
B) `d = dict()`  
C) `d = {'': ''}`  
D) Both A and B

**Correct Answer: D**  
**Explanation:** Both `{}` and `dict()` create empty dictionaries. The notation `{'': ''}` creates a dictionary with one empty string key.

---

### Question 29
What does the following dictionary comprehension produce?
```python
{x: x**2 for x in range(1, 4)}
```

A) `[1, 4, 9]`  
B) `{1: 1, 2: 4, 3: 9}`  
C) `{'1': 1, '2': 4, '3': 9}`  
D) `(1, 4, 9)`

**Correct Answer: B**  
**Explanation:** This dictionary comprehension creates a dictionary with keys 1-3 mapped to their squares: `{1: 1, 2: 4, 3: 9}`.

---

### Question 30
What is the output?
```python
d = {'name': 'Alice', 'age': 25}
print(d.get('grade', 'A'))
```

A) `'A'`  
B) `None`  
C) `KeyError`  
D) `'Alice'`

**Correct Answer: A**  
**Explanation:** The `get()` method returns the value for a key if it exists, or a default value ('A') if it doesn't. Since 'grade' doesn't exist, it returns 'A'.

---

### Question 31
What will this code output?
```python
s1 = {1, 2, 3}
s2 = {2, 3, 4}
print(s1 & s2)
```

A) `{1, 2, 3, 4}`  
B) `{2, 3}`  
C) `{1, 4}`  
D) `{}`

**Correct Answer: B**  
**Explanation:** The `&` operator performs set intersection, returning elements common to both sets: `{2, 3}`.

---

### Question 32
Which method removes an element from a set but does NOT raise an error if the element doesn't exist?

A) `remove()`  
B) `discard()`  
C) `pop()`  
D) `delete()`

**Correct Answer: B**  
**Explanation:** The `discard()` method removes an element if it exists but silently does nothing if it doesn't. The `remove()` method would raise a `KeyError`.

---

### Question 33
What is the difference between a set and a frozenset?

A) Sets can contain any data type; frozensets cannot  
B) Sets are mutable; frozensets are immutable  
C) Frozensets are faster than sets  
D) There is no difference

**Correct Answer: B**  
**Explanation:** A `frozenset` is immutable and cannot be modified after creation. Regular sets are mutable and allow adding/removing elements.

---

### Question 34
What does this code print?
```python
text = 'hello world'
unique_chars = set(text)
print(len(unique_chars))
```

A) `11`  
B) `10`  
C) `8`  
D) `7`

**Correct Answer: C**  
**Explanation:** The string has 11 characters, but the set removes duplicates: 'h', 'e', 'l', 'o', ' ', 'w', 'r', 'd' = 8 unique characters.

---

### Question 35
What will be the result of this dictionary method call?
```python
d = {'a': 1, 'b': 2}
d.update({'c': 3, 'a': 10})
print(d)
```

A) `{'a': 1, 'b': 2, 'c': 3}`  
B) `{'a': 10, 'b': 2, 'c': 3}`  
C) `{'a': 1, 'b': 2}`  
D) `Error`

**Correct Answer: B**  
**Explanation:** The `update()` method inserts new key-value pairs and updates existing ones. The key 'a' is updated from 1 to 10.

---

### Question 36
What is the output of this set operation?
```python
{1, 2, 3} ^ {2, 3, 4}
```

A) `{1, 2, 3, 4}`  
B) `{1, 4}`  
C) `{2, 3}`  
D) `{}`

**Correct Answer: B**  
**Explanation:** The `^` operator performs symmetric difference, returning elements in either set but not in both: `{1, 4}`.

---

### Question 37
Which of the following statements is True about dictionary keys?

A) Keys must be strings  
B) Keys must be unique and immutable  
C) Keys can be any data type  
D) Keys can be lists or dictionaries

**Correct Answer: B**  
**Explanation:** Dictionary keys must be immutable (strings, numbers, tuples) and unique. Mutable types like lists and dictionaries cannot be keys.

---

### Question 38
What does `{1, 2} <= {1, 2, 3}` evaluate to?

A) `True`  
B) `False`  
C) `Error`  
D) `None`

**Correct Answer: A**  
**Explanation:** The `<=` operator checks if the left set is a subset of the right set. `{1, 2}` is a subset of `{1, 2, 3}`, so it returns `True`.

---

### Question 39
What will this code print?
```python
d = {'x': 10, 'y': 20, 'z': 30}
for key, value in d.items():
    if value > 15:
        print(key)
```

A) `x y z`  
B) `y z`  
C) `y` (on separate lines) `z`  
D) `20 30`

**Correct Answer: C**  
**Explanation:** The loop iterates through key-value pairs and prints keys where the value is greater than 15. Both 'y' (20) and 'z' (30) satisfy this condition.

---

### Question 40
What will happen when you execute this code?
```python
s = {1, 2, 3, 4, 5}
s.pop()
print(len(s))
```

A) `5`  
B) `4`  
C) `Error`  
D) `0`

**Correct Answer: B**  
**Explanation:** The `pop()` method removes an arbitrary element from the set. Since one element is removed, the length decreases from 5 to 4.

---

## Summary

These 20 additional questions cover:
- Dictionary methods and operations (get, pop, update, items, values)
- Set operations (union |, intersection &, difference -, symmetric difference ^)
- Set methods (add, remove, discard, pop, clear)
- Dictionary and set comprehensions
- Immutability and uniqueness constraints
- Set comparisons and subset/superset relationships
- Practical applications and edge cases

**Total: 40 multiple choice questions on Chapter 6**
