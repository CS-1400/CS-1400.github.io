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
An index is the position of a character in a sequence (like a string). Indexing begins at 0. Negative indexing begins at the end of the sequence, at index -1. You can access substrings by slicing with indexing.

|0|1|2|3|4|5|6|7|8|9|10|
|M|o|l|t|e|n| |L|a|v|a|
|-11|-10|-9|-8|-7|-6|-5|-4|-3|-2|-1|

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky"></th>
    <th class="tg-0pky"></th>
    <th class="tg-0pky"></th>
    <th class="tg-0pky"></th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"></th>
    <th class="tg-0lax"></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">M</td>
    <td class="tg-0pky">o</td>
    <td class="tg-0pky">l</td>
    <td class="tg-0pky">t</td>
    <td class="tg-0lax">e</td>
    <td class="tg-0lax">n</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">L</td>
    <td class="tg-0lax">a</td>
    <td class="tg-0lax">v</td>
    <td class="tg-0lax">a</td>
  </tr>
  <tr>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
</tbody>
</table>
