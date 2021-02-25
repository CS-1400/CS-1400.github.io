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
    print(flavor.replace('Lava','Chocolate'))   # replace string1 with string2
    print(flavor[0])            # index 0 is first character
    print(flavor[-1])           # index -1 is last character
    print(flavor[3:9])          # substring from index 3 to 8 (9 minus 1)
    print(flavor.isdigit())     # True only if ALL numbers
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

## Indexing
An index is the position of a character in a sequence (like a string). Indexing begins at 0, and is enclosed in square brackets (```flavor[0]```). Negative indexing begins at the end of the sequence, at index -1. You can access substrings by slicing with indices.

![](/assets/string-index.png)
