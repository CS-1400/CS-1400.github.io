---
layout: default
title: Sets
parent: Data Types
---
# Sets
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Sets are a comma-separated sequence of elements, enclosed by curly braces.
- **Mutable**: Their individual elements can be changed.
- **Unique**: Each element must be unique. Duplicate values will be eliminated automatically. 
- **Unordered**: the elements are stored in no specific order. 
    - Individual elements cannot be accessed via index numbers or keys.
- There are many comparison-type actions that can be performed on sets. 
- Python Docs: [Sets](https://docs.python.org/3/tutorial/datastructures.html#sets)
- Python Docs: [Set Types](https://docs.python.org/3/library/stdtypes.html#set-types-set-frozenset)

## Examples

<iframe height="650px" width="100%" src="https://repl.it/@bianca_ruiz/sets?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
<br>
<iframe width="100%" height="450" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=flavors1%20%3D%20%7B'Lemon%20Glaze',%20'Pink%20Velvet',%20'Gingersnap',%20'Molten%20Lava'%7D%0Aflavors2%20%3D%20%7B'Molten%20Lava',%20'Birthday%20Cake'%7D%0A%0Aflavors1.add%28'Birthday%20Cake'%29%0A%0Ain_both%20%3D%20flavors1%20%26%20flavors2%0Anot_in_both%20%3D%20flavors1%20-%20flavors2%0A%0Aflavors1.discard%28'Lemon%20Glaze'%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

## Mutability
Sets are mutable, which means you can change their attributes after instantiation. 
