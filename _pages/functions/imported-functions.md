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
You can access functions written in other python files ("modules") by importing the file into your own program. You import that module into your python file with an `import` statement. 
- Python Docs: [The import Statement](https://docs.python.org/3/reference/simple_stmts.html#the-import-statement)

## Import Statement
The `import` statement(s) are **always** the first line(s) of code in your program (after your docstring). No other code should be written before them.
There are three different ways to import functions from modules:
1. *import module_name*
2. *from module_name import * *
3. *from module_name import function1, function2*

## `import module_name`
- Creates a reference to the module only. 
- Function names in your program must be preceded by the module name then the dot operator.
- You can call any function inside the module. 
- This method reduces the readability of your code.

<iframe width="100%" height="400" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=import%20random%0A%0Anumber1%20%3D%20random.randint%281,10%29%0Anumber2%20%3D%20random.random%28%29%0A%0Aprint%28number1%29%0Aprint%28number2%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

## `from module_name import *`
- Creates references to all functions in a module
- Function names in your program do not need to be preceded by the module name. 
- You can call any function inside the module.
- This method clutters the namespace.

<iframe width="100%" height="400" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=from%20random%20import%20*%0A%0Anumber1%20%3D%20randint%281,10%29%0Anumber2%20%3D%20random%28%29%0A%0Aprint%28number1%29%0Aprint%28number2%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>

## `from module_name import function1, function2`
- Creates references only to the specific function(s) you list. 
- Function names in your program do not need to be preceded by the module name. 
- You can only call the functions you list in the import statement.
- This method is best practice.

<iframe width="100%" height="400" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=from%20random%20import%20randint,%20random%0A%0Anumber1%20%3D%20randint%281,10%29%0Anumber2%20%3D%20random%28%29%0A%0Aprint%28number1%29%0Aprint%28number2%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false"> </iframe>
