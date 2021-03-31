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

## Structure
The `import` statement(s) are **always** the first line(s) of code in your program (after your docstring). No other code should be written before them.
There are three different ways to import functions from modules:
- `import module`
  - Creates a reference to the module only. 
  - Function names must be preceded by the module name then the dot operator.
  - You can call any function inside the module. 
  - This method reduces the readability of your code.
- `from module import *`
  - Creates references to all functions in a module
  - Function names do not need to be preceded by the module name. 
  - You can call any function inside the module.
  - This method clutters the namespace.
- `from module import function1, function2`
  - Creates references only to the specific function(s) you list. 
  - Function names do not need to be preceded by the module name. 
  - You can only call the functions you list in the import statement.
  - This method is best practice.

## Examples

#### import module 
{% highlight Python %}import random

random_int = random.randint(1,10) 
random_float = random.random()

print(random_int)
print(random_float)
{% endhighlight %}

#### from module import function(s)
{% highlight Python %}from random import randint, random

random_int = randint(1,10) 
random_float = random()

print(random_int)
{% endhighlight %}

#### from module import * 
{% highlight Python %}from random import *

number = randint(1,10)
number2 = random()

print(random_int)
print(random_float)
{% endhighlight %}
