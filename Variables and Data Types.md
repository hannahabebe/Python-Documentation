# Variables
  > - Python has no command for declaring a variable. It is created when the first value is assigned.
  > - Multiple values can be assigned to multiple variables in one line. `Eg., x, y, z = "Orange", "Banana", "Cherry"`
  > - Same value can be assignd to multiple variables. `Eg., x = y = z = "Orange"`
  > - The Python `print()` function is often used to output variables.
  > - Variables that are created outside of a function are known as **Global Variables**.
  > - A variable can have a short name `like x and y` or a more descriptive name `age, carname, total_volume`. 
  >   - **Rules for Python Variables:**
  >     - A variable name must start with a letter or the underscore character.
  >     - A variable name cannot start with a number. 
  >     - A variable name can only contain alpha-numeric characters and underscores `(A-z, 0-9, and _ )`.
  >     - Variable names are case-sensitive. `Eg.,a = 4 A = "Hanna" # A will not overwrite a`
  > ### Example:
  > ``` py
  >    # Legal variable names with different techniques & values
  >      myVar = 5          # camel case with int data type
  >      MyVar = "Hanna"    # pascal case with str data type
  >      my_var = 'Ruth'    # snake case with str data type
  >      _x = 5.7           # float
  >      x2 = "Tsige"
  >    # Illegal variable names
  >      2x = "Hanna"
  >      x- = 'Ruth'
  >      x 2 = "Tsige"
  >```
 > ## Unpack a Collection
  >> - If there is a collection of values in a list, tuple etc. Python allows to extract the values into variables. This is called **_Unpacking_**.
  >> ### Example:
   >>``` py
   >>   fruits = ["apple", "banana", "cherry"]
   >>   x, y, z = fruits
   >>   print(x)    # apple
   >>   print(y)    # banana
   >>   print(z)    # cherry
   >>```
 > ## Casting
  >> - It's used to specify the data type of a variable. 
  >> ### Example:
   >>``` py
   >>   x = str(3)      # x will be '3'
   >>   y = int(3)      # y will be 3
   >>   z = float(3)    # z will be 3.0
   >>```
 > ## **type()** Function
  >> - It's used to get the data type of a variable.
  >> ### Example:
   >>``` py
   >>   x = 5
   >>   y = "Hanna"
   >>   print(type(x))   # Prints <class 'int'>
   >>   print(type(y))   # Prints <class 'str'>
   >>```
 > ## Output Variables
   >> ### Example 1:
   >>``` py
   >>   x = "Python is awesome"
   >>   print(x)                  # Prints Python is awesome
   >>```
   >> ### Example 2:
   >>``` py
   >>   # Multiple variables separated by a comma:
   >>   x = "Python"
   >>   y = "is"
   >>   z = "awesome"
   >>   print(x, y, z)      # Prints Python is awesome
   >>```
   >> ### Example 3:
   >> - Without the space character after `"Python "` and `"is "`,  the result would be `"Pythonisawesome"`.
   >>``` py
   >>   # + operator to output multiple variables:
   >>   x = "Python "
   >>   y = "is "
   >>   z = "awesome"
   >>   print(x + y + z)     # Prints Python is awesome
   >>```
   >> ### Example 4:
   >>``` py
   >>   # + works as mathematical operator for numbers
   >>   x = 5
   >>   y = 2
   >>   print(x + y)          # Prints 7
   >>```
   >> - In the `print()` function, combining a string and a number with the `+` operator, Python will give you an _error_:
   >> - The best way to output multiple variables in the `print()` function is to separate them with _commas_, which even support different data types:
 > ## Global Variables
  >> - They can be used by everyone, both inside of functions and outside. 
  >> ### Example 1:
  >> - Create a variable outside of a function, and use it inside the function
  >> ``` py
  >>    x = "awesome"
  >>    def myfunc():
  >>      print("Python is " + x)       # Prints Python is awesome
  >>    myfunc()
  >> ```
  >> ### Example 2:
  >> - Create a variable inside a function (local variable), with the same name as the global variable
  >> ``` py
  >>    x = "awesome"
  >>    def myfunc():
  >>      x = "fantastic"
  >>      print("Python is " + x)       # Prints Python is fantastic
  >>    myfunc()
  >>    print("Python is " + x)       # Prints Python is awesome
  >> ```
  >> ### **global** Keyword
  >> - Normally, when a variable is created inside a function, that variable is local, and can only be used inside that function.
  >> - It's used to create a global variable inside a function.
  >> #### Example 1:
  >> - If the `global` keyword is used, the variable belongs to the global scope:
  >> ``` py
  >>    def myfunc():
  >>      global x
  >>      x = "fantastic"
  >>    myfunc()
  >>    print("Python is " + x)   # Prints Python is fantastic.
  >> ``` 
  >>  #### Example 2:
  >> - Also, use the `global` keyword to refer to the variable when changing the value of a global variable inside a function:
  >> ``` py
  >>    x = "awesome"
  >>    def myfunc():
  >>      global x
  >>      x = "fantastic"
  >>    myfunc()
  >>    print("Python is " + x)   # Prints Python is fantastic.
  >> ```     
# Data Types
  > - It is an important concept.
  > - Variables can store data of different types, and different types can do different things.
  > - How to get the data type is found in the **type() function** example.
  > - Setting the data type is found in the very first example.
  > ## Built-in Data Types:
   >> ``` py
   >>    Text Type:	str
   >>    Numeric Types:	int, float, complex
   >>    Sequence Types:	list, tuple, range
   >>    Mapping Type:	dict
   >>    Set Types:	set, frozenset
   >>    Boolean Type:	bool
   >>    Binary Types:	bytes, bytearray, memoryview
   >>    None Type:	NoneType
   >> ```
  > ## Setting the Specific Data Type
   >> ### Example 
   >>  ``` py
   >> x = str("Hanna")
   >> x = int(20)
   >> x = float(20.5)
   >> x = complex(1j)
   >> x = list(("apple", "banana", "cherry"))
   >> x = tuple(("apple", "banana", "cherry"))
   >> ```
# Links: 
 > - [Variable Reference](https://www.w3schools.com/python/python_variables.asp)
 > - [DataType Reference](https://www.w3schools.com/python/python_datatypes.asp)  
