# Strings
- Python string is a sequence of characters, and each character can be individually accessed using its index.

- You can create strings by enclosing text in both forms of quotes - single quotes or double quotes:
```python
variable_name = "String Data"
```
Example:
```python
str = "Dwip"
print("string is ", str)
```
### Indexing
- The position of every character placed in the string starts from the 0th position and step by step it ends at length-1 position.

```python
txt = "Hello, welcome to my world."
x = txt.index("welcome")
print(x)
```
Output:
```
7
```

### Slicing
- Slicing refers to obtaining a sub-string from the given string. The following code will include index 1, 2, 3, and 4 for the variable named var_name.

- Slicing of the string can be obtained by the following syntax:
```python
string_var[int_start_value:int_stop_value:int_step_value]
```
```python
var_name = "Dwipendu"
print(var_name[1:5])
```
Output:
```
wipe
```
- Here start and step value are considered 0 and 1 respectively if not mentioned by the programmer.

### isalnum() Method
- Returns True if all the characters in the string are alphanumeric, else False:
```python
string_variable = "Company12"
print(string_variable.isalnum())
```
Output:
```
True
```
### isalpha() Method
- Returns True if all the characters in the string are alphabets:
```python
string_variable = "Dwip"
print(string_variable.isalpha())
```
Output:
```
True
```
### isdecimal() Method
- Returns True if all the characters in the string are decimals:
```python
string_variable = "1234"
print(string_variable.isdecimal())
```
Output:
```
True
```
### isdigit() Method
- Returns True if all the characters in the string are digits:
```python
string_variable = "1234"
print(string_variable.isdigit())
```
Output:
```
True
```
### islower() Method
- Returns True if all characters in the string are lower case:
```python
string_variable = "dwip"
print(string_variable.islower())
```
Output:
```
True
```
### isspace() Method
- Returns True if all characters in the string are whitespaces:
```python
string_variable = " "
print(string_variable.isspace())
```
Output:
```
True
```
### isupper() Method
- Returns True if all characters in the string are upper case:
```python
string_variable = "DWIP"
print(string_variable.isupper())
```
Output:
```
True
```
### lower() Method
- Converts a string into lower case equivalent:
```python
string_variable = "DWIP"
print(string_variable.lower())
```
Output:
```
dwip
```
### upper() Method
- Converts a string into upper case equivalent:
```python
string_variable = "dwip"'
string_variable.upper()
```
output
```
DWIP
```
### strip() Method
- It removes leading and trailing spaces in the string:

```python
string_variable.strip()
```

```python
txt = "     Dwip     "
x = txt.strip()
print(x)
```
Output:
```
Dwip
```
```python
txt = "!!!Dwip!!!"
x = txt.strip()
print(x)
```
Output:
```
Dwip
```
## Python String Methods table Sheet

### String Basics

```python
s = "Hello World"
```

| Operation      | Example   | Result          |
| -------------- | --------- | --------------- |
| Length         | `len(s)`  | `11`            |
| Indexing       | `s[0]`    | `'H'`           |
| Slicing        | `s[0:5]`  | `'Hello'`       |
| Step slicing   | `s[::2]`  | `'HloWrd'`      |
| Reverse string | `s[::-1]` | `'dlroW olleH'` |


### Changing Case

| Method     | Example          | Result          |
| ---------- | ---------------- | --------------- |
| Lowercase  | `s.lower()`      | `'hello world'` |
| Uppercase  | `s.upper()`      | `'HELLO WORLD'` |
| Capitalize | `s.capitalize()` | `'Hello world'` |
| Title Case | `s.title()`      | `'Hello World'` |
| Swap Case  | `s.swapcase()`   | `'hELLO wORLD'` |


### Whitespace and Stripping

| Method         | Example            | Result |
| -------------- | ------------------ | ------ |
| Strip (ends)   | `'  hi  '.strip()` | `'hi'` |
| LStrip (left)  | `'  hi'.lstrip()`  | `'hi'` |
| RStrip (right) | `'hi  '.rstrip()`  | `'hi'` |


### Searching & Replacing

| Method     | Example               | Result          |
| ---------- | --------------------- | --------------- |
| Find       | `s.find("o")`         | `4`             |
| Index      | `s.index("o")`        | `4`             |
| Replace    | `s.replace("o", "0")` | `'Hell0 W0rld'` |
| Count      | `s.count("l")`        | `3`             |
| Startswith | `s.startswith("He")`  | `True`          |
| Endswith   | `s.endswith("ld")`    | `True`          |


### Splitting and Joining

| Method | Example                | Result               |
| ------ | ---------------------- | -------------------- |
| Split  | `s.split(" ")`         | `['Hello', 'World']` |
| Join   | `' '.join(['a', 'b'])` | `'a b'`              |


### Testing Strings

| Method          | Example              | Result |
| --------------- | -------------------- | ------ |
| Is alpha        | `'abc'.isalpha()`    | `True` |
| Is digit        | `'123'.isdigit()`    | `True` |
| Is alphanumeric | `'abc123'.isalnum()` | `True` |
| Is lowercase    | `'abc'.islower()`    | `True` |
| Is uppercase    | `'ABC'.isupper()`    | `True` |
| Is space        | `'   '.isspace()`    | `True` |


### Formatting Strings

| Method   | Example                | Result       |
| -------- | ---------------------- | ------------ |
| f-string | `f"Hi {name}"`         | `'Hi Alice'` |
| format() | `'Hi {}'.format(name)` | `'Hi Alice'` |

