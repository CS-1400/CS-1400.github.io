---
layout: default
title: Tuples
parent: Data Types
---
# Tuples
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Tuples are a comma-separated sequence of elements, enclosed by parenthesis (or nothing).
- **Immutable**: you cannot change their individual elements.
- **Index numbers** allow access to individual elements. 
- **Ordered**: the elements are stored in a specific order.
- There are not that many actions (methods and functions) that can be performed on tuples. 
- Python Docs: [Tuples and Sequences](https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences)
- Python Docs: [Sequence Types](https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range)

## Example

<iframe height="700px" width="100%" src="https://repl.it/@bianca_ruiz/tuples-1?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Indexing
An index is the position of an element in a sequence. The first element is at index 0. Negative indexing begins at the last element with index -1. 

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

<iframe width="100%" height="650" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=flavors%20%3D%20%28'Lemon%20Glaze','Pink%20Velvet','Gingersnap','Molten%20Lava'%29%0A%0Aanother_flavor%20%3D%20'Birthday%20Cake',%0Aflavors%20%2B%3D%20another_flavor%0A%0Atuple1%20%3D%20flavors%5B2%3A4%5D%0Atuple2%20%3D%20flavors%5B%3A3%5D%0Atuple3%20%3D%20flavors%5B1%3A%5D%0Atuple4%20%3D%20flavors%5B%3A%5D%0Atuple5%20%3D%20flavors%5B-1%3A%3A-1%5D%0Atuple6%20%3D%20flavors%5B%3A%3A2%5D&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=9&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>
[Run in Repl.it](https://repl.it/@bianca_ruiz/tuple-slicing#main.py){: .btn }

## Immutability
- Tuples are immutable, which means you cannot change their attributes after instantiation. 
- You can join one tuple to another tuple.
