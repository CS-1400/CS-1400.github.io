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
- Python Docs: [The while statement](https://docs.python.org/3/reference/compound_stmts.html#the-while-statement)

## Example

<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/whileTacos?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Infinite Loops
An *infinite loop* is a common error with that occurs when a while is never given the opportunity to fail. The loop below is an infinite loop, because the **cash** variable is never decremented. Therefore, the condition never changes and will remain true.

Run the program below, and observe the infinite loop. Then, paste `cash -= taco_price` on line 6 and run the program again. 

<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/whileInfinite?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
