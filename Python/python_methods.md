

## String Methods  

| Method          | Description                                                                                   |
| :-------------- | :-------------------------------------------------------------------------------------------- |
| capitalize( )   | Converts the first character to upper case                                                    |
| casefold( )     | Converts string into lower case                                                               |
| center( )       | Returns a centered string                                                                     |
| count( )        | Returns the number of times a specified value occurs in a string                              |
| encode( )       | Returns an encoded version of the string                                                      |
| endswith( )     | Returns true if the string ends with the specified value                                      |
| expandtabs( )   | Sets the tab size of the string                                                               |
| find( )         | Searches the string for a specified value and returns the position of where it was found      |
| format( )       | Formats specified values in a string                                                          |
| format_map( )   | Formats specified values in a string                                                          |
| index( )        | Searches the string for a specified value and returns the position of where it was found      |
| isalnum( )      | Returns True if all characters in the string are alphanumeric                                 |
| isalpha( )      | Returns True if all characters in the string are in the alphabet                              |
| isascii( )      | Returns True if all characters in the string are ascii characters                             |
| isdecimal( )    | Returns True if all characters in the string are decimals                                     |
| isdigit( )      | Returns True if all characters in the string are digits                                       |
| isidentifier( ) | Returns True if the string is an identifier                                                   |
| islower( )      | Returns True if all characters in the string are lower case                                   |
| isnumeric( )    | Returns True if all characters in the string are numeric                                      |
| isprintable( )  | Returns True if all characters in the string are printable                                    |
| isspace( )      | Returns True if all characters in the string are whitespaces                                  |
| istitle( )      | Returns True if the string follows the rules of a title                                       |
| isupper( )      | Returns True if all characters in the string are upper case                                   |
| join( )         | Joins the elements of an iterable to the end of the string                                    |
| ljust( )        | Returns a left justified version of the string                                                |
| lower( )        | Converts a string into lower case                                                             |
| lstrip( )       | Returns a left trim version of the string                                                     |
| maketrans( )    | Returns a translation table to be used in translations                                        |
| partition( )    | Returns a tuple where the string is parted into three parts                                   |
| replace( )      | Returns a string where a specified value is replaced with a specified value                   |
| rfind( )        | Searches the string for a specified value and returns the last position of where it was found |
| rindex( )       | Searches the string for a specified value and returns the last position of where it was found |
| rjust( )        | Returns a right justified version of the string                                               |
| rpartition( )   | Returns a tuple where the string is parted into three parts                                   |
| rsplit( )       | Splits the string at the specified separator, and returns a list                              |
| rstrip( )       | Returns a right trim version of the string                                                    |
| split( )        | Splits the string at the specified separator, and returns a list                              |
| splitlines( )   | Splits the string at line breaks and returns a list                                           |
| startswith( )   | Returns true if the string starts with the specified value                                    |
| strip( )        | Returns a trimmed version of the string                                                       |
| swapcase( )     | Swaps cases, lower case becomes upper case and vice versa                                     |
| title( )        | Converts the first character of each word to upper case                                       |
| translate( )    | Returns a translated string                                                                   |
| upper( )        | Converts a string into upper case                                                             |
| zfill( )        | Fills the string with a specified number of 0 values at the beginning                         |

## Int and Float Methods

| Method                                                  | Description                                                                                            |
| :------------------------------------------------------ | :----------------------------------------------------------------------------------------------------- |
| \_\_abs\_\_(self, /)                                    | Absolute value                                                                                         |
| \_\_bool\_\_(self, /)                                   | Returns true if != 0                                                                                   |
| \_\_int\_\_(self, /)                                    | Returns                                                                                                |
| \_\_float\_\_(self, /)                                  | Returns                                                                                                |
| is\_integer(self, /)                                    | Return True if the float is an integer.                                                                |
| \_\_add\_\_(self, value, /)                             | Return self+value.                                                                                     |
| \_\_sub\_\_(self, value, /)                             | Return self-value.                                                                                     |
| \_\_mul\_\_(self, value, /)                             | Return self\*value.                                                                                    |
| \_\_truediv\_\_(self, value, /)                         | Return self/value.                                                                                     |
| \_\_floordiv\_\_(self, value, /)                        | Return self//value.                                                                                    |
| \_\_mod\_\_(self, value, /)                             | Return self%value                                                                                      |
| \_\_divmod\_\_(self, value, /)                          | Returns a pair of numbers (a tuple) consisting of their quotient and remainder.                        |
| \_\_pow\_\_(self, value, mod=None, /)                   | Three parameters base, exponent and modulus(optional)                                                  |
| \_\_round\_\_(self, ndigits=None, /)                    | Return the Integral closest to x, rounding half toward even.                                           |
| \_\_trunc\_\_(self, /)                                  | Return the Integral closest to x between 0 and x.                                                      |
| \_\_neg\_\_(self, /)                                    | Returns -self                                                                                          |
| \_\_pos\_\_(self, /)                                    | Returns +self                                                                                          |
| as\_integer\_ratio(self, /)                             | Returns a tuple of two integers, whose ratio is equal to the Fraction and with a positive denominator. |
| \_\_ceil\_\_(self, /)                                   | Return the ceiling as an Integral.                                                                     |
| \_\_floor\_\_(self, /)                                  | Return the floor as an Integral.                                                                       |
| \_\_eq\_\_(self, /)                                     | Return self=value                                                                                      |
| \_\_gt\_\_(self, /)                                     | Return self>value                                                                                      |
| \_\_lt\_\_(self, /)                                     | Return self<value                                                                                      |
| \_\_ge\_\_(self, /)                                     | Return self>=value                                                                                     |
| \_\_le\_\_(self, /)                                     | Return self<=value                                                                                     |
| \_\_ne\_\_(self, /)                                     | Return self!=value                                                                                     |
| \_\_eq\_\_(self, /)                                     | Return self=value                                                                                      |
| hex(self, /)                                            | Return a hexadecimal representation of a floating-point number.                                        |
| bit\_length(self, /)                                    | Number of bits necessary to represent self in binary.                                                  |
| bit\_length(self, /)                                    | Number of bits necessary to represent self in binary.                                                  |
| to\_bytes(self, /, length, byteorder, \*, signed=False) | Return an array of bytes representing an integer.                                                      |
| x.imag  x.real                                          | real and imaginary parts of a complex number                                                           |
| x.numerator  x.denominator                              | for an integer not a float                                                                             |

## List Methods  

| Method     | Description                                                                  |
| :--------- | :--------------------------------------------------------------------------- |
| append( )  | Adds an element at the end of the list                                       |
| clear( )   | Removes all the elements from the list                                       |
| copy( )    | Returns a copy of the list                                                   |
| count( )   | Returns the number of elements with the specified value                      |
| extend( )  | Add the elements of a list (or any iterable), to the end of the current list |
| index( )   | Returns the index of the first element with the specified value              |
| insert( )  | Adds an element at the specified position                                    |
| pop( )     | Removes the element at the specified position                                |
| remove( )  | Removes the first item with the specified value                              |
| reverse( ) | Reverses the order of the list                                               |
| sort( )    | Sorts the list                                                               |
