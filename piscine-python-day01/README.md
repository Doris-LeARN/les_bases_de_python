## EXERCISE 01
Make a function “double_return”.

It takes a Dictionary as parameter, and returns two lists. Those returned Lists must contains different values. In the first one, there is the list of the keys and the second the list of the values contained in the Dictionary parameter.

For example double_return({“a”: 1, “b”: 2})) returns
([‘a’, ‘b’], [1, 2])

## EXERCISE 02
Create a function “display_all”. It takes a Dictionary as parameters and display every elements of the Dictionary, formated as:

“(class: value)” followed by a new line

• “[class]”: must be the class of the element.

• “[value]”: its value converted into a String

For example display_all({“test”: “hello”, “t”: 43, “pi”: 3.14}) return
(str: hello)
(int: 43)
(float: 3.14)

## EXERCISE 03
Create a function “display_all”.

It takes a Dictionary as parameter and display every element of the Dictionary formated as:

“key->(class: value)” followed by a new line

For example : display_all({“test”: “hello”, “t”: 43, “pi”: 3.14}) returns
test->(str: hello)
t->(int: 43)
pi->(float: 3.14)

## EXERCISE 04
Create a function “display_all”.

It takes a Dictionary as parameter and displays every element of the Dictionary formated as:

“id->(class: value)” followed by a new line

“id” is the index, from 0 to the dictionary’s length.

Note: “=” is forbidden only for assignations, not for default parameters. Same rule for every following exercise. thismeans you cannot create or change values of variables/arguments

For example : display_all({“test”: “hello”, “t”: 43, “pi”: 3.14}) re
0->(str: hello)
1->(int: 43)
2->(float: 3.14)

## EXERCISE 5
Mandatory: Use python’s list/dict comprehension capacities

Create a function “my_count_words” which takes a list as parameter and returns a dictionnary.
The List passed as argument is filled with strings.
The returned dictionnary must be formated to respect the following rules:
• Every key is a string.
• Every value is an integer.
• The associated value is the count of occurrences of the key in the dictionary parameter.

## EXERCISE 6
Mandatory: Use reduce from functools
Create a python script which will add or subtract the values passed as arguments and based on 3 simple rules:
• If there is no arguments, then display 0.
• Else, the first value to use is the first argument.
• For each next argument, if the current value is odd, then add the next argument to the current value,
else subtract it.