---
layout: default
title: Formatting
---

# Formatting
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
Formatted string literals (aka f-strings) are string literals that have an f at the beginning and curly braces containing expressions that will be replaced with their values. Use f-strings to format strings, ints, floats, etc.
- [PEP 498](https://www.python.org/dev/peps/pep-0498/)
- [Python Docs: Formatted String Literals](https://docs.python.org/3/reference/lexical_analysis.html#f-strings)

## Example

{% highlight python %}
def main():

    name = 'Bianca'
    food = 'cookies'
    price = 4.5
    quantity = 3

    print(f"{name}'s favorite food is {food}, at ${price:.2f} a pop.")
    print(f"{quantity} cookies cost a total of ${(quantity * price):.2f}")

if __name__ == '__main__':
    main()
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/f-strings#main.py){: .btn }



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
| ```help()``` 	| Interactive help in the console 	| function -or- type name	| (see description) |
