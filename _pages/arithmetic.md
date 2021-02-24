---
layout: default
title: Arithmetic & Operators
---

# Arithmetic & Operators
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
Python will evaluate expressions containing numeric values (operands) and operators. The evaluation follows the normal "PEMDAS" order of operations.
- [Python Docs: Numeric Types](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)
- [Python Docs: Operator Precedence](https://docs.python.org/3/reference/expressions.html#operator-precedence)

## Example

### Python Code:
{% highlight python %}
def main():

    print(4 / 2)        # Python automatically "widens" ints on division to floats
    print(5 / 2)
    print(5 // 2)       # floor division yeilds the quotient, drops the remainder
    print(5 % 2)        # modulus yeilds the remainder, drops the quotient
    print((5 + 2) * 2)
    print(5 + 2 * 2)

if __name__ == '__main__':
    main()
{% endhighlight %}

### Console Output
{% highlight text %}
2.0
2.5
2
1
14
9
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/arithmetic-operators#main.py){: .btn }



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
