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
Tuples are a comma-separated sequence of elements, enclosed by parenthesis.
- **Immutable**: you cannot change their individual elements.
- **Index numbers** allow access to individual elements. 
- **Ordered**: the elements are stored in a specific order.
- Many different actions (methods and functions) can be performed on tuples. 
- Python Docs: []()
- Python Docs: [Sequence Types](https://docs.python.org/3/library/stdtypes.html#sequence-types-list-tuple-range)

## Example

<iframe> </iframe>
[Run in Repl.it](https://repl.it/@bianca_ruiz/){: .btn }

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

<iframe> </iframe>
[Run in Repl.it](https://repl.it/@bianca_ruiz/list-slicing#main.py){: .btn }

## Immutability
Tuples are immutable, which means you cannot change their attributes after instantiation. 

<iframe></iframe>

[Watch in PythonTutor](){: .btn }
