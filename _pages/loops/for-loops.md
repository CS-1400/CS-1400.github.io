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
For loops are used to execute a block of code a specific number of times, or for each element of a container (such as characters in a string or objects in a list). It will only execute a finite amount of times, no more and no less. 
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

With each new iteration of the loop, the next item in the list is assigned to the loop variable before the code block is executed. The loop will end once each element in the `flavors` list has been assigned to the loop variable:
<iframe width="100%" height="350" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=flavors%20%3D%20%5B'Lemon%20Glaze',%20'Pink%20Velvet',%20'Gingersnap',%20'Molten%20Lava'%5D%0A%0Afor%20flavor%20in%20flavors%3A%0A%20%20%20%20print%28f'%7Bflavor%7D%20is%20delicious!'%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

### Range function
The program illustrated below will execute the number of times specified in the `range` function. In this example, that is exactly five times:
<iframe height="400px" width="100%" src="https://replit.com/@bianca_ruiz/forrange?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

With each new iteration of the loop, the next number from the range function is stored in the loop variable before the code block is executed. The loop will end execution once it has executed the specific number of times indicated in the `range` function:
<iframe width="100%" height="350" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=for%20number%20in%20range%285%29%3A%0A%20%20%20%20print%28f'This%20is%20iteration%20number%20%7Bnumber%2B1%7D'%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

### Enumerate
Applying the `enumerate` function to a for loop adds a number to each item in the container. In order to "catch" this addtional variable (the number), you add a second loop variable to the for loop. The `enumerate` function combined with a for loop is commonly used to store the index number of each item:


