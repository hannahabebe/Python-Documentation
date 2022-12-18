# Data Structures
- are a way of organizing data so that it can be accessed more efficiently depending upon the situation. 
- are fundamentals of any programming language around which a program is built. 
- Python helps to learn the fundamental of these data structures in a simpler way as compared to other programming languages.
  # Built-in Data Structures
    > # Lists
    >> - are used to store multiple items in a single variable.
    >> - are just like the arrays, declared in other languages which is an ordered collection of data.
    >> - Python lists are very flexible as the items in a list do not need to be of the same type.
    >> - List items are _ordered, changeable,_ and _allow duplicate values_.
    >> - are created using square brackets; it's also possible to use the `list()` constructor.
    >> - are indexed, the first item has index `[0]`, the second item has index `[1]` etc.
    >> - The `len()` function is used to determine the number of items a list has.
    >> - In Python, lists are defined as objects with the data type _'list'_. The `type()` function determines the data type of a list.
    >> ## Example:
    >> ``` py
    >>    thislist = ["apple", 5, True, 2.5, 5]       # OR thislist = list(("apple", 5, True, 2.5, 5))
    >>    print(thislist)                             # prints ["apple", 5, True, 2.5, 5]
    >>    print(len(thislist))                        # prints 5
    >>    print(type(mylist))                         # prints <class 'list'>
    >> ```
    >> ## Accessing Items
    >>> - By referring to the index number: `print(list[3])     #Prints the 4th item`
    >>> - By negative indexing: `print(list[-1])    #Prints the last item, and the 2nd last item if [-2]`
    >>> - By defining the start _(included)_ and end _(not included)_ of a range, we can specify a range of indexes: <br/>                                `print(list[2:5]) #Prints the 3rd, 4th & 5th item`
    >>> - By leaving out the start value, the range will start at the first item: <br/>                                                                       `print(list[:5] #Prints the items from the start to, but NOT including, the 5th item)`
    >>> - By leaving out the end value, the range will go on to the end of the list: <br/>                                                                  `print(list[2:] #Prints from the 3rd item to, including, the end)`
    >>> - By specifying negative indexes if we want to start the search from the end of the list: <br/>                                               `print(list[-4:-1]) #Prints the items from index -4 (included) to index -1 (last item, excluded)`
    >>> ### Example
    >>> ``` py
    >>>    thislist = ["apple", 5, True, 2.5, 5]
    >>>    print(thislist[2])                        # prints True
    >>>    print(thislist[-2])                       # prints 2.5
    >>>    print(thislist[1:4])                      # prints [5, True, 2.5]
    >>>    print(thislist[:3])                       # prints ["apple", 5, True]
    >>>    print(thislist[1:])                       # prints [5, True, 2.5, 5]
    >>>    print(thislist[-4:-1])                    # prints [5, True, 2.5]
    >>> ```
