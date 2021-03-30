---
layout: default
title: Imported Functions
parent: Functions
---
# Imported Functions
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
You can access functions written in other python files ("modules") by importing the file into your own program. You import that module into your python file with an `import` statement. The `import` statement(s) are **always** the first line(s) of code in your program (after your docstring). No other code can be written before them.
- Python Docs: [The import Statement](https://docs.python.org/3/reference/simple_stmts.html#the-import-statement)

## Structure
- The `import` statement(s) are **always** the first line(s) of code in your program (after your docstring). No other code can be written before them.
- There are three different ways to import functions from modules:
  - **import module**: imports a reference to the module. The module's function names must be fully qualified. Not the best method for imports, as it clutters the namespace and reduces readability of your code.
  - **from module import function(s)**: Imports only the function(s) listed from the module. The function names do not need to be fully qualified.
  - **from module import * **: Imports all functions from a module. The function names do not need to be fully qualified. Not the best method when considering memory usage.

## Example One
<iframe height="400px" width="100%" src="https://replit.com/@bianca_ruiz/importedfunctions?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
