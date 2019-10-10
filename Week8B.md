Given an integer, *n*, one can convert this number to alternate formats. Integers are in Decimal format, 
however it can also be represended in **Octal**, **Hexadecimal**, and **Binary**. 

In python you can use the string's **.format()** function to do this conversion.

More parameters can be included within the curly braces of our syntax. Use the format code syntax {*field_name*:*conversion*}, where *field_name* specifies the index number of the argument to the str.format() method, and *conversion* refers to the conversion code of the data type.

Types of possible conversions:
```
s – strings
d – decimal integers (base-10)
f – floating point display
c – character
b – binary
o – octal
x – hexadecimal with lowercase letters after 9
X – hexadecimal with uppercase letters after 9
e – exponent notation
```

Syntax :
```
# To limit the precision 
print ("My average of this {0} was {1:.2f}%".format("semester", 78.234876))
```

Errors and Exceptions you may see:
```
ValueError : Error occurs during type conversion in this method.
```

# Goal
Randomly generate 10 integers *n<sub>i</sub>* between 0 and 100 and print the following values for each integer:
1. Decimal
2. Octal
3. Hexadecimal (capitalized)
4. Binary

The four values must be printed on a single line in the order specified above. Each value should be space-padded to match the width of the binary value of *n*.

# Input
*none*

# Output
Print 10 lines where each line *i* contains the respective decimal, octal, capitalized hexadecimal, and binary values of the randomly generated number *n*. Each printed value must be formatted be clearly spaced and aligned in each column ending in the binary values all aligned to the right as shown in the sample output below.

You can add formatting within the curly brackes to give additional format rules such as:
```
'{:>15}'.format('Python') > '         Python' # right justified string up to 15 chracters 
'{:<15}'.format('Python') > 'Python.        ' # left justified string up to 15 characters
'{:<15b}'.format(10)      > '1010.          ' # left justified binary number for 10 up to 15 characters
'{0:>11} {1:>5b}'.format('Python', 10) > '     Python  1010' # right justified first value in format up to 11 characters and right justified binary number for 10 up to 5 characters with a space between.
```

Point is, there is a lot of quirkyness and you may have to play around with the numbers to get it formatted properly

This website has additional info on formatting: https://www.w3resource.com/python/python-format.php

# Sample Output of non-random values
```
 Decimal Octal Hex Binary
    1     1     1     1
    2     2     2    10
    3     3     3    11
    4     4     4   100
    5     5     5   101
    6     6     6   110
    7     7     7   111
    8    10     8  1000
    9    11     9  1001
   10    12     A  1010
   11    13     B  1011
   12    14     C  1100
   13    15     D  1101
   14    16     E  1110
   15    17     F  1111
   16    20    10 10000
   17    21    11 10001
   ```
