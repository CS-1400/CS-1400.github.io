---
layout: default
title: Lists
parent: Data Types
---
# Lists
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Lists are simply a comma-separated sequence of elements, enclosed by square brackets. Each element can be accessed individually by using **index numbers**. Many different actions (aka methods) can be performed on Lists. Lists are also **mutable**, which means you can change their individual characters.
- Python Docs: [Lists](https://docs.python.org/3/tutorial/introduction.html#lists)
- Python Docs: [Sequence Types](https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range)


## Example

{% highlight python %}
def main():
    

if __name__ == '__main__':
    main()
{% endhighlight %}

- Console Output:
{% highlight console %}

{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/strings#main.py){: .btn }



## Indexing
An index is the position of an element in a sequence (like a list). The first element is at index 0.. Negative indexing begins at the last element with index -1. 

![](/assets/list-index.png)

## Slicing
A slice is a piece of a sequence. It is defined by a starting index, a (non-inclusive) ending index, and a step value. If any of the three arguments to the slice are missing, the defaults are as follows:
- Start: first character
- End: last character
- Step: 1 

| Begin | End + 1 | Step | Code                  | Result                                                            |
|-------|---------|------|-----------------------|-------------------------------------------------------------------|
| 2     | 4       |      | ```flavors[2:4]```    | ```['Gingersnap', 'Molten Lava']```                               |
|       | 3       |      | ```flavors[:3]```     | ```['Lemon Glaze', 'Pink Velvet', 'Gingersnap']```                |
| 1     |         |      | ```flavors[1:]```     | ```['Pink Velvet', 'Gingersnap', 'Molten Lava']```                |
|       |         |      | ```flavors[:]```      | ```['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']``` |
| -1    |         | -1   | ```flavors[-1::-1]``` | ```['Molten Lava', 'Gingersnap', 'Pink Velvet', 'Lemon Glaze']``` |
|       |         | 2    | ```flavors[::2]```    | ```['Lemon Glaze', 'Gingersnap']```                               |   

{% highlight python %}
flavors = ['Lemon Glaze','Pink Velvet','Gingersnap','Molten Lava']
print(flavors[2:4])
print(flavors[:3])
print(flavors[1:])
print(flavors[:])
print(flavors[-1::-1])
print(flavors[::2])
{% endhighlight %}
[Run on Repl.it](https://repl.it/@bianca_ruiz/list-slicing#main.py){: .btn }

## Mutability
Once strings are created, their individual elements can be changed: 

{% highlight console %}

{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/string-immutability#main.py){: .btn }
