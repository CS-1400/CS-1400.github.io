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
Lists are simply a comma-separated sequence of elements, enclosed by square brackets.
- **Mutable**: you can change their individual elements.
- **Index numbers** allow access to individual elements. 
- Many different actions (methods and functions) can be performed on lists. 
- Python Docs: [Lists](https://docs.python.org/3/tutorial/introduction.html#lists)
- Python Docs: [Sequence Types](https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range)

## Example

{% highlight python %}
def main():
    
    flavors = ['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']

    print(len(flavors))                 # 4
    print(flavors.index('Gingersnap'))  # 0
    flavors.remove('Molten Lava')       # ['Lemon Glaze', 'Pink Velvet', 'Gingersnap']
    print(flavors)
    flavors.append('Molten Lava')       # ['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']
    print(flavors)
    print(flavors[0])                   # Lemon Glaze
    print(flavors[-1])                  # Molten Lava
    print(flavors[1:3])                 # ['Pink Velvet', 'Gingersnap']

if __name__ == '__main__':
    main()
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/lists-1#main.py){: .btn }

## Indexing
An index is the position of an element in a sequence (like a list). The first element is at index 0. Negative indexing begins at the last element with index -1. 

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
Once lists are created, their individual elements can be changed: 

{% highlight python %}
flavors = ['Lemon Glaze', 'Pink Velvet', 'Gingersnap', 'Molten Lava']
flavors[2] = 'Strawberry Poptart'
print(flavors)
{% endhighlight %}
{% highlight console %}
['Lemon Glaze', 'Pink Velvet', 'Strawberry Poptart', 'Molten Lava']
{% endhighlight %}
[Run on Repl.it](https://repl.it/@bianca_ruiz/list-mutability#main.py){: .btn }
[Watch in PythonTutor](http://www.pythontutor.com/visualize.html#code=def%20main%28%29%3A%0A%20%20%20%20%0A%20%20%20%20flavors%20%3D%20%5B'Lemon%20Glaze',%20'Pink%20Velvet',%20'Gingersnap',%20'Molten%20Lava'%5D%0A%20%20%20%20flavors%5B2%5D%20%3D%20'Strawberry%20Poptart'%0A%20%20%20%20print%28flavors%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false){: .btn }
