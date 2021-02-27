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

<iframe width="800" height="600" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=flavors%20%3D%20%5B'Lemon%20Glaze',%20'Pink%20Velvet',%20%0A'Gingersnap',%20'Molten%20Lava'%5D%0A%0Alength%20%3D%20len%28flavors%29%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0Ag_index%20%3D%20flavors.index%28'Gingersnap'%29%0Aflavors.remove%28'Molten%20Lava'%29%20%20%20%20%20%20%20%0Aflavors.append%28'Molten%20Lava'%29%20%20%20%20%20%0Afirst_element%20%3D%20flavors%5B0%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0Alast_element%20%3D%20flavors%5B-1%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0Aflavors_slice%20%3D%20flavors%5B1%3A3%5D%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%0A&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=9&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>
[Run in Repl.it](https://repl.it/@bianca_ruiz/lists-1#main.py){: .btn }

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

<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/list-slicing?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Mutability
Lists are mutable, which means you can change their individual elements after instantiation. 

<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/list-mutability?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

[Watch in PythonTutor](http://www.pythontutor.com/visualize.html#code=def%20main%28%29%3A%0A%20%20%20%20%0A%20%20%20%20flavors%20%3D%20%5B'Lemon%20Glaze',%20'Pink%20Velvet',%20'Gingersnap',%20'Molten%20Lava'%5D%0A%20%20%20%20flavors%5B2%5D%20%3D%20'Strawberry%20Poptart'%0A%20%20%20%20print%28flavors%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false){: .btn }
