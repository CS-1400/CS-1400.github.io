---
layout: default
title: Strings
parent: Data Types
---
# Strings
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Strings are simply a sequence of characters, enclosed by quotes. Each individual character can be accessed individually by using *index numbers*. Many different actions (aka methods) can be performed on Strings. 
- [Python Docs: Strings](https://docs.python.org/3/tutorial/introduction.html#strings)
- [Python Docs: Built-in Types: str](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)


## Example

{% highlight python %}
def main():
    
    flavor = 'Molten Lava'

    print(len(flavor))          # length

    print(flavor.index('L'))    # index position of the substring
    print(flavor.count('a'))    # how many times substring appears in string
    print(flavor.replace('Lava','Chocolate'))   # replace 1st string with 2nd string

    print(flavor[0])            # index 0 is first character
    print(flavor[-1])           # index -1 is last character
    print(flavor[3:9])          # substring beginning at index 3, ending at 8 (9-1)

    print(flavor.isdigit())     # True if only numbers

    print(f'|{flavor.lower():^15}|{flavor.upper():<15}|{flavor.swapcase():<15}|')


if __name__ == '__main__':
    main()
{% endhighlight %}

- Console Output:
{% highlight console %}
11
7
2
Molten Chocolate
M
a
ten La
False
|  molten lava  |MOLTEN LAVA    |mOLTEN lAVA    |
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/strings#main.py){: .btn }
