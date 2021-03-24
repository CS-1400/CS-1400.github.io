---
layout: default
title: Conditionals
has_children: true
has_toc: false
---

# Conditionals
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Conditionals allow our programs to make choices based on the result of analyzing certain information. In more technical terms, conditionals execute alternate sets of code (branches) based on the evaluation of a boolean expression.
- Python Docs: [if Statments](https://docs.python.org/3/tutorial/controlflow.html#if-statements), [The if statement](https://docs.python.org/3/reference/compound_stmts.html#if), [Truth Value Testing](https://docs.python.org/3/library/stdtypes.html#truth-value-testing)

## Composition
1. `if`: A conditional must have only one `if` statement. It must have a boolean expression.
2. `elif`: A conditonal may have 0 to infinity `elif` statements. It must have a boolean expression.
3. `else`: A conditional may have 0 or 1 `else` statements. It must **never** have a boolean expression.
{% highlight Python %}
if (boolean-expression):
    # this code block executes only if its boolean expression is TRUE
elif (boolean-expression):
    # this code block executes only if all previous boolean expression were FALSE,
    # but this elif's boolean expression is TRUE
else:
    # This code block only executes if all previous boolean expressions were FALSE
{% endhighlight %}

## Examples 
#### if/else Statements
<iframe height="500px" width="100%" src="https://repl.it/@bianca_ruiz/simpleIfTaco?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe><br>
#### elif Statements
<iframe height="550px" width="100%" src="https://repl.it/@bianca_ruiz/elifTaco?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe><br>
#### Compound if Statement
<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/compoundIfTaco?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Python Control Structures
Conditionals are one of three program control structures. These control structures dictate the order in which a program's code executes:
- **Sequential**: Code is executed linearly, one after the other.
- **Selection**: Different block(s) of code are executed based on the results of a condition.
- [**Iteration**](../loops/): Repeating a block of code several times.

## Instructional Videos

<iframe width="373" height="210" src="https://www.youtube.com/embed/eSYeHlwDCNA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="373" height="210" src="https://www.youtube.com/embed/5pPKYWqkoek" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="373" height="210" src="https://www.youtube.com/embed/oYaGJBMoXok" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="373" height="210" src="https://www.youtube.com/embed/IBOHc87yFYw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
