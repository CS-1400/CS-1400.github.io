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
- **Mutable**: you can change any of their attributes.
- **Keys**, like index numbers, allow access to individual values. Keys must be unique and immutable.
- Many different actions (methods and functions) can be performed on dictionaries. 
- Python Docs: [Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)
- Python Docs: [Mapping Types](https://docs.python.org/3/library/stdtypes.html#typesmapping)

## Example
<iframe width="800" height="600" frameborder="0" src="http://pythontutor.com/iframe-embed.html#code=snowboard%20%3D%20%7B'brand'%3A'arbor','model'%3A'cadence','length'%3A147%7D%0A%0Alength%20%3D%20len%28snowboard%29%20%20%20%20%20%20%20%20%20%20%20%20%20%23%20how%20many%20key%3Avalue%20pairs%0Amy_brand%20%3D%20snowboard%5B'brand'%5D%20%20%20%20%20%20%20%23%20access%20a%20value%20by%20its%20key%0Asnowboard%5B'model'%5D%20%3D%20'clovis'%20%20%20%20%20%20%20%23%20edit%20existing%20value%0Asnowboard%5B'color'%5D%20%3D%20'wood'%20%20%20%20%20%20%20%20%20%23%20add%20new%20item%20to%20dictionary%0Asnowboard.pop%28'length'%29%20%20%20%20%20%20%20%20%20%20%20%20%20%23%20remove%20a%20key/value%20item%20%20%20%20%20%0A%0Afor%20key,%20value%20in%20snowboard.items%28%29%3A%0A%20%20%20%20print%28f'The%20snowboard%5C's%20%7Bkey%7D%20is%20%7Bvalue%7D'%29%0A%20%20%20%20%0Asnowboard_alias%20%3D%20snowboard%20%20%20%20%20%20%20%20%20%23%20create%20alias%20to%20snowboard%0Asnowboard_copy%20%20%3D%20snowboard.copy%28%29%20%20%23%20create%20copy%20of%20snowboard%0A%0Asnowboard_alias.clear%28%29%20%20%20%20%20%20%20%20%20%20%20%20%20%23%20what%20happens%20to%20the%20alias%0Aprint%28snowboard%29%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%23%20also%20happens%20to%20the%20original%0Aprint%28snowboard_copy%29%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%23%20but%20doesn't%20affect%20copies&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>


## Keys
Keys must be immutable data types!  

## Header



## Mutability
meow: 

<iframe></iframe>

[Watch in PythonTutor](){: .btn }
