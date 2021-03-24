---
layout: default
title: For Loops
parent: Loops
---
# For Loops
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
For loops are used to execute a block of code a specific number of times, or on each element of a container (such as characters in a string or objects in a list). It executes a pre-defined, finite amount of times. No more, no less.
- Python Docs: [for statements](https://docs.python.org/3/tutorial/controlflow.html#for-statements), [The for statement](https://docs.python.org/3/reference/compound_stmts.html#the-for-statement)

## Composition
This loop always begins with the `for` keyword, followed by an arbitrary variable name(s). This is followed by the `in` keyword, and either a pre-defined container variable (string, list, set, etc) -or- the `range` function:

{% highlight Python %}
for loop_variable in range(15):
    # this code block executes the specific number of times indicated in the range function argument

for loop_variable in container_variable:
    # this code block executes for each item in the container variable
{% endhighlight %}

## Examples

### Items in a container
The program illustrated below will execute for each item in the `flavors` list. Therefore, it will execute exactly four times, since there are four items in the list:
<iframe height="400px" width="100%" src="https://replit.com/@bianca_ruiz/forflavors?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

With each iteration of the loop, the next item in the list is assigned to the loop variable before the code block is executed. The loop will end once each element in the `flavors` list has been assigned to the loop variable:
<iframe width="100%" height="350" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=flavors%20%3D%20%5B'Lemon%20Glaze',%20'Pink%20Velvet',%20'Gingersnap',%20'Molten%20Lava'%5D%0A%0Afor%20flavor%20in%20flavors%3A%0A%20%20%20%20print%28f'%7Bflavor%7D%20is%20delicious!'%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

### Range function


