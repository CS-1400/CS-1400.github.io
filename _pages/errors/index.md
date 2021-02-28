---
layout: default
title: Errors
has_children: true
has_toc: false
---

# Errors
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
The three types of errors we encounter while programming are syntax, runtime, and logic. Each of these errors are described below, along with a small example.
- Python Docs: [Errors and Exceptions](https://docs.python.org/3/tutorial/errors.html)

## Syntax Errors
Syntax errors are caused by not following the rules of the language. Examples: beginning a variable name with a number, forgetting to close parenthesis or quotes, or misspelling keywords. The editor will usually bring these to your attention by underlining them in red.
{% highlight python %}
Print('Hello there!')       # the *p* in print should not be capitalized
{% endhighlight %}

## Runtime Errors
Runtime Errors happen during program execution and cause your program to crash. They are caused by asking the computer something it cannot do, such as division by zero or trying to access the 5th character of a four character string.
{% highlight python %}
solution = 5 / 0            # division by zero is a fatal error
{% endhighlight %}

## Logic Errors
Logic errors occur when the program runs fine, but the output is incorrect. This can be caused by incorrect algorithms, or mistyping an operator (ex: + instead of -).
{% highlight python %}
total = subtotal - tax      # the subtraction operator should be addition
{% endhighlight %}
