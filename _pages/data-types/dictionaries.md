---
layout: default
title: Dictionaries
parent: Data Types
---
# Dictionaries
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
A dictionary is a collection of key-value pairs enclosed by curly braces ({}). A colon (:) separates each key from its value.
- **Mutable**: you can change their size, keys, and values.
- **Keys** allow access to individual values. (instead of index numbers)
- Many different actions (methods and functions) can be performed on dictionaries. 
- Python Docs: []()
- Python Docs: []()

## Example

<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/lists-1?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Keys
meow. 

|-----|-----|-----|-----|
|meow |meow |meow |meow |

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

<iframe></iframe>

## Mutability
meow: 

<iframe></iframe>

[Watch in PythonTutor](){: .btn }
