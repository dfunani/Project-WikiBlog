# Strings

> A **String** ('str') in python, is an immutable sequence of characters expressed between quotation marks `" ", ' ', ''' ''' """ """`. *Python Strings* belong to the [*str*](https://docs.python.org/3/library/stdtypes.html?highlight=str#str) class and contains methods and attributes which we will later covered in this topic.

## Initializing Strings

*Python Strings* can be assigned to any variable in a program. Each character in a *Python String* must be an [**ASCII**]("https://www.asciitable.com/") character, with the resulting string being immutable. This means any operations performed on a string will result in an entirely new string.
> 🎆 Implications of the immutability of *Python String*:
>>>> name = "delali"
>>>> fname = name
>>>> fname == name and fname is name
>>>> True
>>>>
>>>> name += " funani"
>>>> fname == name and fname is name
>>>> False
>>>>
> Note: A New string, *different in value and nature*, is created when the variable name is appended with another string.

### Single Line

The String is initialized with the sequence of characters spanning across exactly one line:

1. #### Double Quotes

   ```Python
   variable_name = "String Value"
   ```

2. #### Single Quotes

   ```Python
   variable_name = 'String Value'
   ```

### Multiple Lines

The String is initialized with the sequence of characters spanning across multiple lines, using triple quotes:

1. #### Triple Double Quotes

   ```Python
   variable_name = """String Value Header
   String Value Line 1
   String Value Line 2
   ..."""
   ```

2. #### Triple Single Quotes

   ```Python
   variable_name = '''String Value Header
   String Value Line 1
   String Value Line 2
   ...'''
   ```

### Escape Characters

**Escape Characters** are used to denote special printable characters such as a new line or tab or an aphostrophe within a *Python String*. A *Special Character* is identified or *Escaped* using a backslash `\`.

#### Special Characters

1. Tab:
```\t Insert a tab in the text at that point```
2. Backspace:
```\b Insert a backspace in the text at that point.```
3. New-Line:
```\n Insert a newline in the text at that point.```
4. Return/Enter:
```\r Insert a carriage return in the text at that point.```
5. Form-Feed:
```\f Insert a formfeed in the text at that point.```
6. Space:
```\s Insert a space in the text at that point.```

> Example
>>>> ```variable_name = "Hello World\n"```
>
> The Special character `\n` adds a New-Line at the end of the words `Hello World`.

#### Ambiguous Characters

With *Python Strings* using quotation marks as string indentifiers, ambiguity arises when the string being created, intends to use quotation marks or backslashes.

1. Single Quotation Mark:
```\' Insert a single quote character in the text at that point.```
2. Double Quotation Mark:
```\" Insert a double quote character in the text at that point.```
3. Backslash:
```\\ Insert a backslash character in the text at that point.```

> 🎆 **Python** allows the use of double and single quotes interchangeably, however consistency must be maintained, to ensure no ambiguity:

```Python
name = "Delali's World" # Unambiguous - No need to escape the '
name = '"Sarcasm" is unwanted' # Unambiguous - No need to escape any of the "
name = 'Delali's World' # Ambiguous - Would need to escape the '
name = 'Delali\'s World' # Unambiguous - ' is escaped
name = ""Sarcasm" is unwanted" # Ambiguous - Would need to escape the "
name = "\"Sarcasm\" is unwanted" # Unambiguous - " is escaped
```

## Operating on Strings

As discussed before, *Python Strings* are immutable however the underlying class provides methods and operations that can be applied to an instance of a **string**. Any string resulting from operations or methods applied to an initial string will be entirely different string.

### Arithmetic Operators

1. Add Strings Together - Concatenation

    ```Python
    variable_name = "String_Value_1" + "String_Value_2" # Joins (Concatenates) the 2 strings into 1
    variable_fname = "new" + variable_name + "exit" # Value of fname + Value of name + "new" + "exit"
    ```

2. Multiply String by Integer - Replication

    ```Python
    i = 1 # Positive integer [0, 1, 2, 3,...]
    variable_name = "String_Value_1" * i # Replicates the string as many times as the integer i
    ```

### String Class Methods

1. Capitalize

    Returns the string with the first letter in upper-case and the rest of the letters in lower-case.

    ```Python
    variable_name = "String_Value" # String to capitalize
    uppercase_variable_name = variable_name.capitalize() # Stores the Capitalized string to a new variable
    ```

2. Count

    Returns the string with the first letter in upper-case and the rest of the letters in lower-case.

    ```Python
    variable_name = "String_Value" # String to capitalize
    uppercase_variable_name = variable_name.capitalize() # Stores the Capitalized string to a new variable
    ```
