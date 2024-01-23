# 🌟🔥 Basic Python Knowledge 🔥🌟 

<p align="center">
<img width="40%" src="media/213911110-aedbef38-a29f-4b6b-a65c-11608b4f75a5.gif">
<img width="40%" src="media/213911110-aedbef38-a29f-4b6b-a65c-11608b4f75a5.gif">
</p>

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

Hi everyone I am a python developer. As we all know there are times that we can easily forget the most basic stuff about programming. So I took it apon myself to write this README on most basic pythonic knowledge needed by a python developer if the need to search for the most basic stuff ever rises. Now I can find what I've been searching 1000 times over much more easier ;). Please enjoy...

<p align="center">
<img width="50%" src="media/216656963-09118229-8a9e-4af0-910c-c37f35f2e210.gif">
</p>

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">


***Table of content:*** ☕

1. [Main Data Types](#main-data-types-🔥)
    - [Numeric](#numeric)
    - [String](#string)
    - [Sequence](#sequence)
    - [Binary](#binary)
    - [Mapping](#mapping)
    - [Boolean](#boolean)
    - [Sets](#sets)
2. [Sequence type vs Iterable type](#sequence-type-vs-iterable-type-🔥)
3. [Mutable vs Immutable](#mutable-vs-immutable-🔥)
4. [Type and Length](#type-and-length-🔥)
5. [Type casting](#type-casting-🔥)
6. [Variables](#variables-🔥)
    - [LEGB Rule for Python Scope](#legb-rule-for-python-scope)
    - [Garbage collection](#garbage-collection)
7. [Conditional Statements (Control Structures)](#conditional-statements-control-structures-🔥)
    - [if](#if)
    - [elif and else](#elif-and-else)
8. [Loops](#loops-🔥)
    - [for loop](#for-loop)
        - [Usage of range with foor loop](#usage-of-range-with-foor-loop)
    - [while loop](#while-loop)
        - [Indefinite vs definite iteration](#indefinite-vs-definite-iteration)
    - [Nested Loops](#nested-loops)
9. [Iterable & Iterator](#iterable--iterator-🔥)
10. [Recursion](#recursion-🔥)
11. [Functions & Generators](#functions--generators-🔥)
    - [Generators](#generators)
12. [Lambda function](#lambda-function-🔥)
13. [Type Checking](#type-checking-🔥)
14. [Most used methods when working with sequences](#most-used-methods-when-working-with-sequences-🔥)
    - [map()](#map)
    - [zip()](#zip)
    - [filter()](#filter)
    - [reduce() (not a built-in)](#reduce-not-a-built-in)
15. [Quotient and Remainder](#quotient-and-remainder-🔥)
    - [divmod()](#divmod)
16. [is vs = (diffrences)](#is-vs--diffrences-🔥)
17. [Logical operators (and, or, not)](#logical-operators-and-or-not-🔥)
18. [Exceptions](#exceptions-🔥)
    - [Exception handling](#exception-handling)
    - [Raise exceptions](#raise-exceptions)
    - [assert keyword](#assert-keyword)
19. [with (context manager)](#with-context-manager-🔥)
    - [Managing resources](#managing-resources)
    - [with statement](#with-statement)
20. [Resources](#resources-🔥)

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

<img width="100%" src="media/238355349-7d484dc9-68a9-4ee6-a767-aea59035c12d.gif">

## Main Data Types 🔥

There are 7 main data types in python:

1. Numeric (int, Float, complex)
2. String (str)
3. Sequence (list, tuple, range)
4. Binary (bytes, bytearray, memoryview)
5. Mapping (dict)
6. Boolean (bool)
7. Sets (set, frozenset)


### Numeric

Numeric data types are used to hold numeric values.

1. int -> signd integer of unlimitid length.
2. float -> floating pricision numbers. float is accurate up to 15 decimal places.
3. complex -> compplex numbers.

**Examples:**

- int -> 25, 56, 15986
- float -> 2.3, 98.4
- complex -> 100+3j


### String

String is a sequence of characters. strings are presented by either single or double-quotes.

**Example:**

- str -> "Hello, World!", 'Python Knowledge'


### Sequence

A sequence is a positionally ordered collection of items. And you can refer to any item in the sequence by using it's index number. With index starting from 0.

1. list -> Lists are the most versatile sequence type. Lists can hold diffrent types of data. And lists are mutable(can be changed). **< list = [any, any, any, ...] >**

2. tuple -> Tuples are like lists, but they are immutable - they can't be changed. **< tuple = (any, any, any) >**

3. range -> Range is a sequence of numbers in a given range. **< range(start, stop, step) >** 

**Examples:**

- list -> [1, "arad", 5.9, True]
- tuple -> (56, "moo", 4.5, False)
- range -> range(0, 10, 2) = 0, 2, 4, 6, 8


### Binary

The decimal system employs base ten digits (0 to 9), whereas the binary system, operating in base two, uses only 0s and 1s. While decimal is widely utilized, the simplicity of binary makes it prominent in computer programming and related engineering fields.

1. bytes -> Python bytes are a sequence of integers in the range of 0-255. You can create bytes in Python using the bytes() function or a bytes literal.

2. bytearray -> An array of given bytes. This is especially useful when dealing with binary data. **< bytearray([source[, encoding[, errors]]]) >**

3. memoryview -> memoryview allow you to access the internal data of an object that supports the buffer protocol without any need to copying data first. **< memoryview(obj) >**

> [!NOTE]
> Buffer protocol provides a way to access the internal data of an object. 

**Examples:**

- bytes -> bytes([65, 66, 67]) = b'ABC'
- bytearray -> bytearray(string, "utf-8") = b'string' (since it's an array, it has indexes.)
- memoryview -> memoryview(byte_array) = now the internal data of this object is accessible.


### Mapping

Python Dictionary is an unordered sequence of data of key-value pair form. It is similar to the hash table type. Dictionaries are written within curly braces in the form key: value. It is very useful to retrieve data in an optimized way among a large amount of data. **(values are mapped to keys)**

- dict = {key: value, key: value, ...}

**Example:**

- dict -> {"first_name": "git", "last_name": "hub", "age": 42}


### Boolean

Boolean is one of Python's built-in data types. It's used to represent the truth value of an expression. It is used to see if some fact is True or False.

- bool = True, False ---> True is equal to 1 and False is equal to 0.

**Examples:**

- Sun does not exist = False
- I'm tired = True


### Sets

Sets are used to store multiple items in a single variable. A set is a collection which is **unordered**, and **unindexed**. Keep in mind that duplicate values are not allowed in sets. ***A set itself may be modified, but the elements contained in the set must be of an immutable type.***

- set -> a normal mutable set of immutable values.
- frozenset -> frozenset is in all respects exactly like a set, except that a frozenset is immutable. **< frozenset(set) >**

**Examples:**

- set -> {"foo", "bar", "baz"}
- frozenset -> frozenset({'foo', 'bar', 'baz'})

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Sequence type vs Iterable type 🔥

An iterable is a collection of objects where you can get each element one by one. Therefore, any sequence is iterable. For example, a list is iterable.

However, an iterable may not be a sequence type. For example, a set is iterable but it’s not a sequence.

Generally speaking, iterables are more general than sequence types.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Mutable vs Immutable 🔥

In programming, you have an immutable object if you can’t change the object’s state after you’ve created it. In contrast, a mutable object allows you to modify its internal state after creation. In short, whether you’re able to change an object’s state or contained data is what defines if that object is mutable or immutable.

Immutable objects are common in functional programming, while mutable objects are widely used in object-oriented programming. Because Python is a multiparadigm programming language, it provides mutable and immutable objects for you to choose from when solving a problem.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Type and Length 🔥

There are two most used built-in functions with data in python which are **type()** and **len()**.

- `type()` -> returns the type of the data it was given. Example: type(13) is int

- `len()` -> is used to get the length of sequnces(the number of data in them). Example: len(["abc", "efg"]) is 2 

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Type casting 🔥

There are times that we need to change the type of data in python. In order to do this we need to use the function of each data type on said data to change it's type.

> [!TIP]
> To make type casting work, we need to make sure that the type of data can be changed. Or let's say data is compatible with new type.

**Examples:**

1. my_list = [53, 24]
    - my tuple = tuple(mylist) -> (53, 24)

2. my_str = "666"
    - my_int = int(my_str) -> 666

3. my_dict = {"key": "value"}
    - my_int = int(my_dict) -> type error

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Variables 🔥

A Python variable is a reserved memory location to store values. In other words, a variable in a python program gives data to the computer for processing. In other words Variables are containers for storing data values.

Python is a highly object-oriented language. In fact, virtually every item of data in a Python program is an object of a specific type or class. A Python variable is a symbolic name that is a reference or pointer to an object. Once an object is assigned to a variable, you can refer to the object by that name. But the data itself is still contained within the object.


Python has no command for declaring a variable. And a variable is created the moment you first assign a value to it.

Variables do not need to be declared with any particular type, and can even change type after they have been set.

> [!NOTE]
> The type of the variable is the same as the type of data it holds in itself.

> [!NOTE]
> In order to get the type of a variable we use the ***type()*** method.

***To declare a variable we only need to write the name of the variable and then use = (assignment operator) and then write the data.***

**< variable_name = data >**

**Examples:**

- my_str = "mooooo"
- my_number = 69
- my_float = 3.14
- my_list = [1, "abc", 5.5]
- my_tuple = (95, 156)
- my_dict = {"name": "spooch", "age": 5}
- my_set = {45, 21, 85}


### LEGB Rule for Python Scope

A variable is only available from inside the region it is created. This is called scope.

The ***LEGB*** rule is a kind of name lookup procedure, which determines the order in which Python looks up names.

- **Local (or function) scope:** is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

- **Enclosing (or nonlocal) scope:** is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

- **Global (or module) scope:** is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

- **Built-in scope:** is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.


### garbage collection

When the number of references to an object drops to *zero*, it is no longer accessible. At that point, its lifetime is over. Python will eventually notice that it is inaccessible and reclaim the allocated memory so it can be used for something else. In computer lingo, this process is referred to as ***garbage collection***.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Conditional Statements (Control Structures) 🔥

A Conditional Statement(control structure) directs the order of execution of the statements in a program (referred to as the program’s control flow).

A Conditional Statement is used for decision-making in the program.

In python this is achived by usin the if statement.

### if

```bash
if <expr>:
    <statements>
```

- `<expr>` is an expression evaluated in a Boolean context.
- `<statements>` are valid Python statements, which must be indented.

If `<expr>` is true (evaluates to a value that is “truthy”), then `<statements>` are executed. If `<expr>` is false, then `<statements>` are skipped over and not executed.

Note that the colon (`:`) following `<expr>` is required. Some programming languages require `<expr>` to be enclosed in parentheses, but Python does not.

> [!WARNING]
> ***Indentation*** is a very important consept in python. So make sure to learn it right. Bad indentation can lead to program not being run properly.

**Example:**

```bash
name = "clive"

if name == "clive":     # This condition is True so the name will be printed.
    print(name)

if name == "gildarts":  # This condition is False so the name will not be printed.
    print(name)
```

Since conditions work based on boolean values it's very important to understand how booleans work. So in this example since the first if statement is True `(name == "clive") == True` then the name will be printed. But in the second if statement, since the condition is False `(name == "gildarts") == False` then the name wont be printed. The name variable is equal to **"clive"**.


### elif and else

So far we know what `if` does. But there are more to `if` statement.

`elif` and `else` are both parts of `if` statement that we can use on certian use cases.

- `elif` (else if) is used to check another condition inside the same `if` statement, instead of writing multiple `if` statements.

- `else` is to declare what to do if the `if` and `elif` statements are all False.

> [!IMPORTANT]
> There can be multiple `elif` in an `if` statement but there can be only one `else`. Plus the `else` always come's last.

**Example:**

```bash
name = input("Please enter your name: ")

if name == "clive":   # if This condition is True then (clive is back) will be printed.
    print(name, "is back")
elif name == "gildarts":  # if This condition is True then (gildarts, is a name?) will be printed.
    print(f"{name}, is a name?")
else:   # if None of the above conditions are True (Sorry I dont know you!) will be printed.
    print("Sorry I dont know you!")
```

In this example we take an input from the user then we check to see if the entered name is `"clive"`, if it's True then _(clive is back)_ will be printed. else if the entered name is `"gildarts"` then _(gildarts, is a name?)_ will be printed. else the entered name is neither `"clive"` or `"gildarts"` then _(Sorry I dont know you!)_ will be printed.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Loops 🔥

There are 2 main types of loops in python.

1. for
2. while


### for loop

A for loop is an iterator, used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string). for loop is mainly used for definite iteration.

**Syntax:**

```bash
for <var> in <iterable>:
    <statement(s)>
```

- `<iterable>` is a collection of objects(a sequence)

- The `<statement(s)>` in the loop body are denoted by indentation, as with all Python control structures, and are executed once for each item in `<iterable>`. 

- The loop variable `<var>` takes on the value of the next element in `<iterable>` each time through the loop.

> [!NOTE]
> With the `break` statement we can stop the loop before it has looped through all the items.

> [!NOTE]
> With the `continue` statement we can stop the current iteration of the loop, and continue with the next.

#### Usage of range with foor loop

To loop through a set of code a specified number of times, we can use the `range()` function,

The `range()` function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and ends at a specified number.

The `range()` function defaults to increment the sequence by 1, however it is possible to specify the increment value by adding a third parameter:

**Syntax:**

```bash
for <var> in range(x, y, z):
    <statement(s)>
```
- x -> starting point of range
- y -> ending point of range
- z -> step of range

> [!NOTE]
> If you dont have a statement for your code block yet, then you can use `pass` keyword to avoid getting errors.

```bash
for <var> in <iterable>:
    pass
```

> [!NOTE]
> The `else` keyword in a for loop specifies a block of code to be executed when the loop is finished:


### while loop

while loop is another kind of loop in python that is mainly used for indefinite iteration. With the while loop we can execute a set of statements as long as a condition is true.

**Syntax:**

```bash
while <expr>:
    <statement(s)>
```

- `<statement(s)>` represents the block to be repeatedly executed, often referred to as the body of the loop. This is denoted with indentation, just as in an if statement.

- The controlling expression, `<expr>`, typically involves one or more variables that are initialized prior to starting the loop and then modified somewhere in the loop body. 

- When a while loop is encountered, `<expr>` is first evaluated in Boolean context. If it is true, the loop body is executed. Then `<expr>` is checked again, and if still true, the body is executed again. This continues until `<expr>` becomes false, at which point program execution proceeds to the first statement beyond the loop body.

> [!NOTE]
> `continue`, `break` statements and `else` clause can be used with `while` loop as well.

#### Indefinite vs definite iteration

- With **indefinite** iteration, the number of times the loop is executed isn’t specified explicitly in advance. Rather, the designated block is executed repeatedly as long as some condition is met.

- With **definite** iteration, the number of times the designated block will be executed is specified explicitly at the time the loop starts.

### Nested Loops

***A nested loop is a loop inside a loop. The "inner loop" will be executed one time for each iteration of the "outer loop".***

**Syntax:**

```bash
for <var-a> in <iterable-a>:
    for <var-b> in <iterable-b>:
        <statement(s)>
```
<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Iterable & Iterator 🔥

- Iterable is a sequence of data which can be iterated over.
- Iterator is a functionality that which iterates over the iterable.

> [!NOTE]
> Every iterator is also an iterable, but not every iterable is an iterator in Python.


<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Recursion 🔥

In Python, it's also possible for a function to call itself! A function that calls itself is said to be recursive, and the technique of employing a recursive function is called recursion. 

_Factors you need to consider before using recursion:_

- For some problems, a recursive solution, though possible, will be awkward rather than elegant.

- Recursive implementations often consume more memory than non-recursive ones.

- In some cases, using recursion may result in slower execution time.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Functions & Generators 🔥

A function is a block of code which only runs when it is called. The idea is to put some commonly or repeatedly done tasks together and make a function so that instead of writing the same code again and again for different inputs, we can do the function calls to reuse code contained in it over and over again.

_Some Benefits of Using Functions:_

- Increase Code Readability 
- Increase Code Reusability

**Syntax:**

```bash
# Defining the function
def <function_name>(<parameter(s)>):
    <statement(s)>
    # you can use return here

# Calling the function
<function_name>(<argument(s)>)
```

- `def` -> It's the keyword that informs Python that a function is being defined.
- `<function_name>` -> A valid Python identifier that names the function.
- `<parameters>` -> An optional, number of, comma-separated parameters that may be passed to the function.
- `:` -> Punctuation that denotes the end of the Python function header (the name and parameter list).
- `<statement(s)>` -> A block of valid Python statements.

> [!NOTE]
> In orther to call a function we use the name of function followed by paranthesis () and then we pass in the arguments, for parameters we defined in function.

> [!IMPORTANT]
> The ***return*** keyword is used in function statements to return the result of function. 


### Generators

A Generator function in Python is a function that returns an iterator using the Yield keyword. Generator functions are a special kind of function that return a lazy iterator. These are objects that you can loop over like a list. However, unlike lists, lazy iterators do not store their contents in _memory_. 

**Syntax:**

```bash
# Defining the generator function
def <function_name>(<parameter(s)>):
    <statement(s)>
    yield result

# Calling the generator function one step at a time
generator = <function_name>(<argument(s)>)
next(generator)

# Calling the generator function with a for loop to get all results
generator = <function_name>(<argument(s)>)
for i in generator:
    print(i)
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Lambda function 🔥

A lambda function is a small anonymous function. It can take any number of arguments, but can only have one expression.

**Syntax:**

```bash
lambda arguments : expression
```

The expression is executed and the result is returned.

> [!IMPORTANT]
> `lambda` functions are supposed to be ***small and light weight***. Dont try to write a complicated function using `lambda`, always use a `def` function for said use cases.

> [!NOTE]
> Best usage of lambda is in built-in methods. Like -> **map(), reduce(), filter(), ...**

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Type Checking 🔥

Python is a dynamically typed language. This means that the Python interpreter does type checking only as code runs, and that the type of a variable is allowed to change over its lifetime.

In order to define types of data we can use the `typing` package.

- from typing import the_name_of_type

**Example:**

```bash
from typing import ObjectId

def return_car_object(car_id: ObjectId):  # This means that the type of id is ObjectId.
    object = collection.find_one({"_id":car_id})
    return object
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Most used methods when working with sequences 🔥

There are many built-in methods in python but some of them are usualy used more than others.

These methods are:

1. map()
2. zip()
3. reduce()
4. filter()

> [!NOTE]
> The best use cases of lambda functions are with this methods.


### map()

Python’s `map()` is a built-in function that allows you to process and transform all the items in an iterable without using an explicit for loop, a technique commonly known as mapping. `map()` is useful when you need to apply a transformation function to each item in an iterable and transform them into a new iterable. `map()` is one of the tools that support a functional programming style in Python.

**Syntax:**

*map(function, iterables)*

- function -> The function that will be executed for each iterable. This is a good case to use lambda functions.

- iterables -> A sequence, collection or an iterator object. You can send as many iterables as you like.

**Example:**

```bash
# Double all numbers using map and lambda

numbers = (1, 2, 3, 4)
result = map(lambda x: x + x, numbers)
print(list(result))

# Output
[2, 4, 6, 8]
```

### zip()

The zip() function returns a zip object, it takes iterable containers and returns a single iterator object, having mapped values from all the containers. It is used to map the similar index of multiple containers so that they can be used just using a single entity. 

If the passed iterables have different lengths, the iterable with the least items decides the length of the new iterator.

**Syntax:**

_zip(*iterables)_

- iterables ->  `zip()` can accept any type of iterable, such as files, lists, tuples, dictionaries, sets, and so on.

**Example:**

-`zip()` is so useful when we need to make a dictionary from two lists.

```bash
stocks = ['GEEKS', 'For', 'geeks']
prices = [2175, 1127, 2750]

new_dict = {stocks: prices for stocks,
			prices in zip(stocks, prices)}
print(new_dict)

# Output
{'GEEKS': 2175, 'For': 1127, 'geeks': 2750}
```

### filter()

Python’s `filter()` is a built-in function that allows you to process an iterable and extract those items that satisfy a given condition. This process is commonly known as a filtering operation. With `filter()`, you can apply a filtering function to an iterable and produce a new iterable with the items that satisfy the condition at hand.

**Syntax:**

_filter(function, iterable)_

- The first argument, function, must be a single-argument function. Typically, you provide a predicate (Boolean-valued) function to this argument. In other words, you provide a function that returns either True or False according to a specific condition.

- The second argument, iterable, can hold any Python iterable, such as a list, tuple, or set. It can also hold generator and iterator objects. An important point regarding filter() is that it accepts only one iterable.

**Example:**

```bash
numbers = [-2, -1, 0, 1, 2]
positive_numbers = filter(lambda n: n > 0, numbers)
print(list(positive_numbers))
```
In this example if a number is bigger than 0, meaning it is positive, then it will be in the output.


### reduce() (not a built-in)

Python’s `reduce()` is a function that implements a mathematical technique called folding or reduction. `reduce()` is useful when you need to apply a function to an iterable and reduce it to a single cumulative value.

> [!IMPORTANT]
> **reduce()** is not a built-in method. It is imported from functools module. *from functools import reduce*

**Syntax:**

_reduce(function, iterable)_

- function -> is the function we want to apply on the iterable.
- iterable -> an iterable containing data.

**Example:**

```bash
from functools import reduce

def my_add(a, b):
     result = a + b
     print(f"{a} + {b} = {result}")
     return result

number_list = [0, 1, 2, 3, 4]
print(reduce(my_add, numbers))

# Output
0 + 1 = 1
1 + 2 = 3
3 + 3 = 6
6 + 4 = 10
10
```

> [!NOTE]
> Python's `reduce()` function doesn't return a new sequence like `map()` and `filter()`. Instead, it returns a single value. 

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Quotient and Remainder 🔥

A ***dividend*** is a number that is divided by the divisor. The ***divisor*** is the factor that divides the dividend. The result obtained by the division process is called the ***quotient*** and the number left behind after the completion of the division is called the ***remainder***.


- The **division** operator is represented by // and can be used as follows: `quotient = a // b`

- The **modulo** operator is represented by % and helps in determining the remainder when a number is divided by another: `remainder = a % b`

**Examples:**

- 10 // 5 = 2

- 10 % 5 = 0

### divmod()

`divmod()` is a useful built-in function in Python that takes two arguments and returns a **tuple** containing the quotient and the remainder. The function’s syntax is quite simple: `divmod(x, y)`, where *x* is the **dividend**, and *y* is the **divisor**.

**Example:**

```bash
x, y = 10, 3
result = divmod(x, y)
print(result)  # Output: (3, 1)
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## is vs = (diffrences) 🔥

The `==` operator compares the value or equality of two objects, whereas the Python `is` operator checks whether two variables point to the same object in memory. 

- `==` -> Checks for value equality. Use it when you would like to know if two objects have the same value.

- `is` -> Checks for reference equality. Use it when you would like to know if two references refer to the same object. *(object id in memory)*

> [!NOTE]
> is will return True if two variables point to the same object (in memory), == if the objects referred to by the variables are equal.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Logical operators (and, or, not) 🔥

In Python, Logical operators are used on conditional statements (either True or False). They perform Logical AND, Logical OR, and Logical NOT operations.

- ***and*** -> Returns True if both the operands are true.

- ***or*** -> Returns True if either of the operands is true.

- ***not*** -> Returns True if the operand is false.


***Order of Precedence for Logical Operators***

In the case of multiple operators, Python always evaluates the expression from left to right.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## Exceptions 🔥

An Exception is an error that happens during the execution of a program.

> [!NOTE]
> Syntax error is diffrent from exceptions.

- ***Syntax Error:*** As the name suggests this error is caused by the wrong syntax in the code. It leads to the termination of the program. 

- ***Exceptions:*** Exceptions are raised when the program is syntactically correct, but the code results in an error. This error does not stop the execution of the program, however, it changes the normal flow of the program.


### Exception handling

When an error occurs, or exception as we call it, Python will normally stop and generate an error message. These exceptions can be handled using the try statement.

**`try` statement has 4 diffrent parts:**

- The **try** block lets you test a block of code for errors.

- The **except** block lets you handle the error.

- The **else** block lets you execute code when there is no error.

- The **finally** block lets you execute code, regardless of the result of the try- and except blocks.


> [!NOTE]
> We can use many **except** blockes but only one `else` and one `finally` block. 


***Syntax:***

```bash
try:
    <statements>
except < can include the type of exception >:
    <statements>
else: 
    <statements>
finally:
    <statements>
```

> [!NOTE]
>  `else` and `finally` block are optional 


### Raise exceptions

We may need to throw an exception if a condition occurs. To throw (or raise) an exception, use the **raise** keyword.

**Example:**

```bash
x = input("Please enter a number: ")
if type(x) is not int:
    raise TypeError("It's not a number!")
```


### assert keyword

Assertion is the boolean expression that checks if the statement is True or False. If the statement is true then it does nothing and continues the execution, but if the statement is False then it stops the execution of the program and throws an error.

**Syntax:**

```bash
assert condition, error_message(optional) 
```

An assert statement consists of the assert keyword, the expression or condition to test, and an optional message. The condition is supposed to always be `True`. If the assertion condition is `True`, then nothing happens, and your program continues its normal execution. On the other hand, if the condition becomes `False`, then assert halts the program by raising an AssertionError.

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

## with (context manager) 🔥

There are basically 2 kinds of operations in python:

1. ***I/O bound***
2. ***CPU bound***

*I/O bound* are operations that work based on input and output,(they dont use much of the system's resources). such as file operations or making requests to endpoints.

*CPU bound* are operations that use the system and It's cpu to run calculations. 


### Managing resources

In any programming language, the usage of external resources like file operations or database connections is very common. But these resources are limited in supply. Therefore, the main problem lies in making sure to release these resources after usage. If they are not released then it will lead to resource leakage and may cause the system to either slow down or crash. It would be very helpful if users have a mechanism for the automatic setup and teardown of resources. In Python, it can be achieved by the usage of context managers which facilitate the proper handling of resources. The with statement in Python is a quite useful tool for properly managing external resources in your programs


### with statement

In python the `with` keyword is used when working with unmanaged resources (like file streams). It allows you to ensure that a resource is **"cleaned up"** when the code that uses it finishes running, even if exceptions are thrown.

**Example:**

```bash
with open('output.txt', 'w') as f:
     f.write('Hi there!')
```

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">

<img width="100%" src="media/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif">


## Resources 🔥

In order to provide the best descriptions for readers of this document some parts of professional documents where used. you can use the links below to read more.

<img width="100%" src="media/240304586-d48893bd-0757-481c-8d7e-ba3e163feae7.png">

<p><hr></p>

**Real Python**

1. [Mutable vs immutable](https://realpython.com/python-mutable-vs-immutable-types/)

2. [Python sets](https://realpython.com/python-sets/)

3. [Python conditions](https://realpython.com/python-conditional-statements/)

4. [Python for loop](https://realpython.com/python-for-loop/)

5. [Python while loop](https://realpython.com/python-while-loop/)

6. [Python recursion](https://realpython.com/python-recursion/)

7. [Python functions](https://realpython.com/defining-your-own-python-function/#functions-in-python)

8. [Python generators](https://realpython.com/introduction-to-python-generators/)

9. [Python lambda](https://realpython.com/python-lambda/#python-lambda-and-regular-functions)

10. [Python type checking](https://realpython.com/python-type-checking/)

11. [Python map fuction](https://realpython.com/python-map-function/)

12. [Python zip fuction](https://realpython.com/python-zip-function/)

13. [Python reduce fuction](https://realpython.com/python-reduce-function/)

14. [Python filter fuction](https://realpython.com/python-filter-function/)

15. [Python assert statement](https://realpython.com/python-assert-statement/)

16. [Python scope and LEGB rule](https://realpython.com/python-scope-legb-rule/)

17. [Python with statement](https://realpython.com/python-with-statement/)



**GeekForGeeks**

1. [Python functions](https://www.geeksforgeeks.org/python-functions/)

2. [Python generators](https://www.geeksforgeeks.org/generators-in-python/)

3. [Python map fuction](https://www.geeksforgeeks.org/python-map-function/)

4. [Python zip fuction](https://www.geeksforgeeks.org/zip-in-python/)

5. [Python reduce fuction](https://www.geeksforgeeks.org/reduce-in-python/)

6. [Python logical operators](https://www.geeksforgeeks.org/python-logical-operators/)

7. [Python exception handling](https://www.geeksforgeeks.org/python-exception-handling/)

8. [Python assert keyword](https://www.geeksforgeeks.org/python-assert-keyword/)

9. [Python variables](https://www.geeksforgeeks.org/python-variables/)

10. [Python context managers](https://www.geeksforgeeks.org/context-manager-in-python/)



**W3Schools**

1. [Python conditions](https://www.w3schools.com/python/python_conditions.asp)

2. [Python for loop](https://www.w3schools.com/python/python_for_loops.asp)

3. [Python while loop](https://www.w3schools.com/python/python_while_loops.asp)

4. [Python functions](https://www.w3schools.com/python/python_functions.asp)

5. [Python lambda](https://www.w3schools.com/python/python_lambda.asp)

6. [Python map fuction](https://www.w3schools.com/python/ref_func_map.asp)

7. [Python zip fuction](https://www.w3schools.com/python/ref_func_zip.asp)

8. [Python exception handling](https://www.w3schools.com/python/python_try_except.asp)



**Others**

1. [pythontutorial: python sequences](https://www.pythontutorial.net/advanced-python/python-sequences/)

2. [cuemath: dividend, divisor, quotient, remainder formula](https://www.cuemath.com/dividend-divisor-quotient-remainder-formula/)

3. [finxter: divmod](https://blog.finxter.com/python-get-quotient-and-remainder-with-divmod/)

4. [stackoverflow: = vs is](https://stackoverflow.com/questions/132988/is-there-a-difference-between-and-is)



**Gifs & Images**

- [Source of Gifs and Images](https://github.com/Anmol-Baranwal/Cool-GIFs-For-GitHub)

<p align="center">
<img width="50%" src="media/216656956-c5f97119-4de0-4e55-8906-c2699cc43ccd.gif">
</p>