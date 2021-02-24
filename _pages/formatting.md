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
- [Python Docs: Formatted String Literals](https://docs.python.org/3/reference/lexical_analysis.html#f-strings)
- [Python Docs: Escape Sequences](https://docs.python.org/3/reference/lexical_analysis.html#literals)

## Example

Python Code:
{% highlight python %}
def main():

    name = 'bIaNcA'
    food = 'cookies'
    price = 4.5
    quantity = 3

    print(f"{name.capitalize()}'s favorite food is {food}, at ${price:.2f} a pop.")
    print(f"{quantity} {food} cost a total of ${(quantity * price):.2f}")

    print(f"{name.upper():>15}")    # field width = 15; right-justified
    print(f"{name.lower():^15}")    # field width = 15; centered
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
