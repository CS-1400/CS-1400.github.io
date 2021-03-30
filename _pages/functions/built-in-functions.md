---
layout: default
title: Built-in Functions
parent: Functions
---
# Built-in Functions
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Built-in functions are pre-installed with the Python language. They do not need to be imported or created by the programmer. Common built-in functions are `print()`, `input()`, and `length()`
- Python Docs: [Built-in Functions](https://docs.python.org/3/library/functions.html)

## Invocation
When invoking (calling/executing) a function, you type it's name followed by opening and closing parenthesis. 
- **Arguments**: Some functions accept arguments (input), which are placed inside the parenthesis. 
- **Return Value**: Some functions produce output, and return it to its caller.

## Example
<iframe height="400px" width="100%" src="https://replit.com/@bianca_ruiz/builtin-functions?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
#### Line 1
- Function: `input`
- Arguments: `'Hi! What\'s your name? '`
- Return Value: User input is stored in the variable `name`
#### Line 2
- Function: `print`
- Arguments: n-a
- Return Value: n-a
#### Line 3
- Function: `print`
- Arguments: `f'Nice to meet you, {name.title()}.'`
- Return Value: n-a
#### Line 4
- Function: `len`
- Arguments: `name` (a variable)
- Return Value: length of variable, stored in the variable `characters`
#### Line 5
- Function: `print`
- Arguments: `f'Your name has {len(name)} characters.'`
- Return Value: n-a
