---
layout: default
title: Exception Handling
parent: Errors
---

# Exception Handling
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Exception handling allows programmers to deal with an error gracefully and avoid a sudden program crash. It is best practice to place error-prone code inside of try/except blocks. 
- Python Docs Wiki: [Handling Exceptions](https://wiki.python.org/moin/HandlingExceptions)

### Without exception handling
Run the program below, and enter non-numeric input at the prompt. Notice that the runtime error (exception) crashes the program.
<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/no-exception-handling?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

### With exception handling
Run the program below, and enter non-numeric input at the prompt. Compare the output with the previous program. 
<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/exception-handling?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>