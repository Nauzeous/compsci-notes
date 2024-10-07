Data stored and used in computer programs can take on many forms known as ==data types==

different data types require different amounts of memory, and there is many different data types

it is important to use correct data types to optimise program performance

5 main data types
- Integer - 5
- Float/Real - 2.4
- Boolean - True
- Character - 'S'
- String - 'asdfg'

the names of these main data types may vary between languages, but all languages support these types

Different languages support various different types with different names and uses, but most languages allow more complex data types, known as ==composite data types== to be constructed from the 5 primitive types.

### integer
the integer data type represents a positive or negative whole number
- -15
- 90
- 21
- 0
- -1

### real/float
the real data type represents all decimal numbers that **can be expressed as a fraction** such as 
-  6.5
- 0.123456789
- -1.3
- 12.0
it is important to note that integers can be expressed as floats (all integers can be floats but not all floats are integers

### Character
The character data type represents a single (alphanumeric) character or symbol
- A
- ;
- ~
- 3
- d

### String
The string data type represents a ==collection of characters==
"asdfhjkl!;#"

### Boolean
the boolean data type can be used to represent one of two values associated with boolean algebra, ==*true* or *false*==, 1 or 0

## Casting data types

most languages allow data types to be converted to another, known as ==casting==

If someone enters the letter "1", it is treated as the character "1", and not the number 1

You would have to convert the character to an integer before using it in arithmetic

Each language has different syntax for casting (python syntax will be used in exam)

str(2) = "2"
int("51") = 51
float("2.71") = 2.71

## Bonus data types
data types can be customised more in depth with some languages, allowing for specified lengths of the data type, and ranges
s - signed - includes negative numbers and positive numbers
u - unsigned - includes only positive numbers
most data types except byte are assumed to be signed unless stated otherwise

eg.
-sbyte |  -128 - 127 | 1 byte 
-byte |  0 - 255 | 1 byte
-short | -32,768 - 32,767 | 2 bytes
-ushort | 0 - 65,535 | 2 bytes
-int | signed 2<sup>32</sup> | 4 bytes
-uint | unsigned 2<sup>32</sup> | 4 bytes
-long | signed 2<sup>64</sup>  | 8 bytes
