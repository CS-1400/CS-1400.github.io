---
layout: default
title: Functions
---

# Functions

## Definition
A function is a prewritten block of code with a name. We call it by name to execute it. Functions optionally contain:
  - **arguments**: the function's input; data given to the function enclosed within the parenthesis.
  - **return**: the function's output; data passed back to the line of code that called it.

## Built in functions
Below is a table of functions we'll learn and use in CS-1030. For a full list of built-in functions, refer to the [Python Docs](https://docs.python.org/3/library/functions.html)

| Function 	| Description 	| Argument(s) 	| Return  |
|-	|-	|-	|- |
| ```print()``` 	| Displays strings to the console 	| String 	| N-A |
| ```input()``` 	| Prompts the user to enter text 	| String (user prompt)	| String |
| ```type()``` 	| Returns the data type of argument 	| Variable or literal value	| String (data type) |
| ```int()``` 	| Converts the argument to an integer 	| Variable or literal value	| int |
| ```float()``` 	| Converts the argument to a floating point number 	| Variable or literal value	| float |
| ```str()``` 	| Converts the argument to a string 	| Variable or literal value	| str |
| ```help()``` 	| Prints information to the console 	| function -or- type name	| Python help in console |

## Example

<div class="code-example" markdown="1">

```Python
def main():

    name = input('Hi! What\'s your name? ')
    print('Nice to meet you, ' + name)

if __name__ == '__main__':
    main()
```

</div>
[Run on Repl.it](https://repl.it/@bianca_ruiz/built-in-functions){: .btn }
