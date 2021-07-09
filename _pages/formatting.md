---
layout: default
title: Formatting
nav_order: 4
---

# Formatting
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
F-strings have an f at the beginning and curly braces containing expressions that will be replaced with their values. Use f-strings to format strings, ints, floats, etc.
- Python Docs: [Formatted String Literals](https://docs.python.org/3/reference/lexical_analysis.html#f-strings), [Escape Sequences](https://docs.python.org/3/reference/lexical_analysis.html#literals)

## Example

<iframe height="800px" width="100%" src="https://repl.it/@bianca_ruiz/f-strings?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Escape Sequences
Escape sequences allow you to include symbols and characters inside string literals using a backslash. As an example, You cannot use a contraction with an apostrophe inside a string enclosed in single quotes. You would "escape" that symbol with a backslash: 
{% highlight python %}
print('That\'s my favorite cookie flavor!')
{% endhighlight %}
| Escape Sequence 	| Symbol 	|
|-	|-	|
| \\' 	| Single Quote 	|
| \\" 	| Double Quote 	|
| \t 	| Tab 	|
| \n 	| Newline 	|
| \\\ 	| Backslash 	|

## Instructional Video

<iframe width="373" height="210" src="https://www.youtube.com/embed/bQQqxysLIGE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
