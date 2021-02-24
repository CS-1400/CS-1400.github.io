---
layout: default
title: Functions
---

# Functions
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
A function is a prewritten block of code with a name. We call it by name to execute it. Functions optionally contain:
  - **arguments**: the function's input; data given to the function enclosed within the parenthesis.
  - **return**: the function's output; data passed back to the line of code that called it.
See: [Python Docs: Built-in Functions](https://docs.python.org/3/library/functions.html)


## Example

{% highlight python %}
def main():

    name = input('Hi! What\'s your name? ')
    print('Nice to meet you, ' + name)

if __name__ == '__main__':
    main()
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/built-in-functions#main.py){: .btn }



## Built-in Functions
Below is a table of functions we'll learn and use most in CS-1030. 


| Function 	| Description 	| Argument(s) 	| Return  |
|-	|-	|-	|- |
| ```print()``` 	| Displays strings to the console 	| String 	| N-A |
| ```input()``` 	| Prompts the user to enter text 	| String (user prompt)	| String |
| ```type()``` 	| Returns the data type of argument 	| Variable or literal value	| String (data type) |
| ```int()``` 	| Converts the argument to an integer 	| Variable or literal value	| int |
| ```float()``` 	| Converts the argument to a floating point number 	| Variable or literal value	| float |
| ```str()``` 	| Converts the argument to a string 	| Variable or literal value	| str |
| ```help()``` 	| Interactive help in the console 	| function -or- type name	| (see description) |
