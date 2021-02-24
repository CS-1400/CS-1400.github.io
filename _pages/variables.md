---
layout: default
title: Variables
---
# Variables
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
Variables are named areas of memory that we can use to store date. All variables have three things: a name, a type, and a value.
- [Python PEP8: Variable Names](https://www.python.org/dev/peps/pep-0008/#type-variable-names)

## Assignment Statements
Variable names **must** be to the left of the assignment operator; values **must** be to the right:
- :+1: ```flavor = 'chocolate chip'```
- :-1: ```'chocolate chip' = flavor```

Python Code:
{% highlight python %}
def main():

    name = 'bIaNcA'
    food = 'cookies'
    price = 4.5
    quantity = 3

    print(f"{name.capitalize()}'s favorite food is {food}, at ${price:.2f} a pop.")
    print(f"{quantity} {food} cost a total of ${(quantity * price):.2f}")

    print(f"{name.upper():>15}") # field width = 15; right-justified
    print(f"{name.lower():^15}") # field width = 15; centered
    print(f"{name.swapcase():<15}") # field width = 15; left-justified
    
if __name__ == '__main__':
    main()
{% endhighlight %}

Console Output:
{% highlight text %}
Bianca's favorite food is cookies, at $4.50 a pop.
3 cookies cost a total of $13.50
         BIANCA
    bianca     
BiAnCa
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/f-strings#main.py){: .btn }

## Escape Sequences
Escape sequences allow you to include symbols and characters inside string literals using a backslash. As an example, You cannot use a contraction with an apostrophe inside a string enclosed in single quotes. You would "escape" that symbol with a backslash: 
{% highlight python %}
print('That\'s my favorite cookie flavor!')
{% endhighlight %}
| Escape Sequence 	| Symbol 	|
|-	|-	|
| \\' 	| Single Quote 	|
| \\" 	| Double Quote 	|
| \t 	| Tab 	|
| \n 	| Newline 	|
| \\\ 	| Backslash 	|
