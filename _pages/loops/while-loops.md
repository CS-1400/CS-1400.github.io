---
layout: default
title: While Loops
parent: Loops
---
# While Loops
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
While loops are used to execute a block of code until a condition fails.
- Python Docs: [The while statement](https://docs.python.org/3/reference/compound_stmts.html#the-while-statement)

## Examples

<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/whileTacos?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
<br>
<iframe width="100%" height="350" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=count%20%3D%205%0A%0Awhile%20count%20%3E%200%3A%0A%20%20%20%20print%28count%29%0A%20%20%20%20count%20-%3D%201%0A%20%20%20%20%0Aprint%28'Blast%20Off!'%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

## Infinite Loops
An *infinite loop* is a common error with that occurs when a condition is never given the opportunity to fail. The loop below is an infinite loop, because the **cash** variable is never decremented. Therefore, the condition never changes and will remain true.

Run the program below, and observe the infinite loop. Then, paste `cash -= taco_price` on line 6 and run the program again. 

<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/whileInfinite?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
