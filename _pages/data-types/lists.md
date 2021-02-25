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
    
    flavors = ['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']

    print(len(flavors))                 # length
    print(flavors.index('Gingersnap'))  # index position of the element
    flavors.remove('Molten Lava')       # remove element from list
    print(flavors)
    flavors.append('Molten Lava')       # add element to end of list
    print(flavors)
    print(flavors[0])                   # index 0 is first element
    print(flavors[-1])                  # index -1 is last element
    print(flavors[1:3])                 # slice from index 1 to 2 (3 minus 1)

if __name__ == '__main__':
    main()
{% endhighlight %}

- Console Output:
{% highlight console %}
4
0
['Lemon Glaze', 'Pink Velvet', 'Gingersnap']
['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']
Lemon Glaze
Molten Lava
['Pink Velvet', 'Gingersnap']
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/lists-1#main.py){: .btn }



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
flavors = ['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']
flavors[2] = 'Strawberry Poptart'
print(flavors)
{% endhighlight %}
{% highlight console %}
['Lemon Glaze', 'Pink Velvet', 'Strawberry Poptart', 'Molten Lava']
{% endhighlight %}
[Run on Repl.it](https://repl.it/@bianca_ruiz/list-mutability#main.py){: .btn }
