# Creating Variables
  ~ Python has no command for declaring a variable. It is created when the first value is assigned.
  
  ~ Variable names are case-sensitive.
  
  ~ Multiple values can be assigned to multiple variables in one line (Eg., x, y, z = "Orange", "Banana", "Cherry").
 
  ~ Same value can be assignd to multiple variables. (Eg., x = y = z = "Orange")
  
  ~ Variables that are created outside of a function are known as global variables.
   ### Example:
      x = 5   $integer
      y = "Hanna" $string
  ## Casting
    ~ It's used to specify the data type of a variable. 
      ### Example:
      x = str(3)    $ x will be '3'
      y = int(3)    $ y will be 3
      z = float(3)  $ z will be 3.0
   ## type() Function
    ~ It's used to get the data type of a variable.
   ## global Keyword
    ~ It's used to create a global variable inside a function.
   ### Example:
          def myfunc():
          global x
          x = "fantastic"
        myfunc()
        print("Python is " + x)   $Prints Python is Fantastic.

    
# Data Types
  ~ It is an important concept.
  ## Built-in Data Types:
    Text Type:	str
    Numeric Types:	int, float, complex
    Sequence Types:	list, tuple, range
    Mapping Type:	dict
    Set Types:	set, frozenset
    Boolean Type:	bool
    Binary Types:	bytes, bytearray, memoryview
    None Type:	NoneType
  
