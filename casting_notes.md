# CASTING

In Python, there are different variable types. Some of the basic (or "primative") types are
- strings (i.e. text), created within single or double quotes
  - "Example of a string"
  - 'Another example of a string'
  - """We can use three quotes if we want
       an example of a multiline string"""
- integers (i.e. whole numbers)
- floats (i.e. numbers with decimal points)

Sometimes we will want to convert from one type to another, which is a process called __casting__. For example, the following code raises an error:
```python
>>> "3" + 3
... (ignore these lines)
TypeError: can only concatenate str (not "int") to str
```
i.e. Python doesn't support adding strings and integers.

This code does something you might not expect:
```python
# will this give me 9?
>>> "3" * 3
'333'
# Nope!
```

This is because "3" (the string) is interpreted differently from 3 (the integer). If we used 3 (the integer) we would get
```python
>>> 3 + 3
6
>>> 3 * 3
9
```
which is probably what we are expecting. As humans, we know that if we were to think of "3" as a number, the sensible number is 3.

## Cast operators

In Python:

- to cast `x` to a string, use `str(x)`. Almost anything can be cast to a string.
  - example: `str(3) # returns '3'`
  - example: `str('already a string') # returns 'already a string'`
  - example: `str(3.1415) # returns '3.1415'`
- to cast `x` to an integer, use `int(x)`. Strings that only contain digits (with a possible - sign). If Python cannot convert to an integer, we will get an error instead
  - example: `int('3')  # returns 3`
  - example: `int('-3') # returns -3`
  - example: `int(3.14) # returns 3`
  - example: `int(3.99) # returns 3. Can covert a FLOAT to an INT`
  - example: `int('3.14')   # ERROR! Cannot convert a STRING that looks like a float to an INT`
  - example: `int('Damien') # ERROR! No sensible interpretation of "Damien" and an integer`
- to cast `x` as a float, use `float(x)`
  - example: `float(3)  # returns 3.0`
  - example: `float('3') # returns 3.0`
  - example: `float('3.14') # returns 3.14`
  - example: `float('1e2')  # returns 100`
  - example: `float('Damien')  # ERROR! No interpretation of 'Damien' as a float`
  - example: `float('3.14.15') # ERROR! No interpretation of 3.14.15 as a float`

## Note on learning

Advice about casting (and learning Python in general)
- DON'T spend a lot of effort learning the various rules about what casting works and what doesn't. Most of the examples, like `int('Damien')`, are obviously wrong. More subtle examples, such as `int('1,000')` not working can be checked with the REPL.
- Along these lines, the examples above are NOT exhaustive. For example, `int('4F', 16)` is valid and evaluates to 79 (technically, it is converting a hexadecimal string to an integer). In most programming problems, it is better to learn enough to get going rather than learning all the corner cases.
  - If you need it, you'll learn it with use cases
  - If it isn't super useful because it doesn't come up (e.g. knowing that `int('3.0')` gives an error), it won't hurt you to not know it
  - If you have a question of whether "Does this cast work?" you can look on google, or just _try it_ in Jupyter or the REPL.

Because of this, I am not going to try and make the casting rules exhaustive. 
 
 
