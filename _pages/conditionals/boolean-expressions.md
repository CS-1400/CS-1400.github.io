---
layout: default
title: Boolean Expressions
parent: Conditionals
---

# Boolean Expressions
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
A boolean expression is any logical statement that evaluates to either `True` or `False`. They can be a comparison, an identity or membership test, or methods that return a boolean value.   

- Python Docs: [Truth Value Testing](https://docs.python.org/3/library/stdtypes.html#truth-value-testing)


## Example
<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/boolean?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Comparison Operators
`<`, `<=`, `>`, `>=`, `==`, and `!=` are comparison operators. They compare 2 values and return a `True` or `False`. They can also be "chained" together:
{% highlight python %}
name > "a"
17 < age < 26
{% endhighlight %}

## Boolean Operators
`and`, `or`, and `not` are boolean operators. They are used to change or combine the results of a boolean expression:
{% highlight python %}age < 18 or age > 65
age > 17 and age < 26{% endhighlight %}
