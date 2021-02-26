---
layout: default
title: Strings
parent: Data Types
---
# Strings
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Strings are simply a sequence of characters, enclosed by quotes. 
- **Immutable**: you cannot change the values of their individual characters.
- **Index numbers** allow access to individual characters. 
- Many different actions (methods and functions) can be performed on strings. 
- Python Docs: [Strings](https://docs.python.org/3/tutorial/introduction.html#strings)
- Python Docs: [Text Sequence Type](https://docs.python.org/3/library/stdtypes.html#text-sequence-type-str)

## Example

<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/strings?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Indexing
An index is the position of an element in a sequence. Indexing begins at 0 with the first element. Negative indexing begins at -1 with the last element. 

![](/assets/string-index.png)

## Slicing
A slice is a piece of a string. It is defined by a starting index, a (non-inclusive) ending index, and a step value. If any of the three arguments to the slice are missing, the defaults are as follows:
- Start: first character
- End: last character
- Step: 1 

| Start | End + 1 | Step | Code                 | Result        |
|-------|---------|------|----------------------|---------------|
| 3     | 9       |      | ```flavor[3:9]```    | 'ten La'      |
|       | 6       |      | ```flavor[:6]```     | 'Molten'      |
| 7     |         |      | ```flavor[7:]```     | 'Lava'        |
|       |         |      | ```flavor[:]```      | 'Molten Lava' |
| -1    |         | -1   | ```flavor[-1::-1]``` | 'avaL netloM' |
|       |         | 2    | ```flavor[::2]```    | 'Mle aa'      |      

<iframe height="600px" width="100%" src="https://repl.it/@bianca_ruiz/string-slicing?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

## Immutability
Once strings are created, their individual characters cannot be changed: 
{% highlight python %}
flavor = 'Molten Lava'
flavor[7] = 'l'   # this is an illegal operation  
print(flavor)
{% endhighlight %}

{% highlight console %}
Traceback (most recent call last):
  File "main.py", line 8, in <module>
    main()
  File "main.py", line 4, in main
    flavor[7] = 'l'     
TypeError: 'str' object does not support item assignment
{% endhighlight %}

Instead, reassign the **entire** string:
{% highlight python %}
flavor = 'Molten Lava'
flavor = flavor[:7] + 'l' + flavor[8:]     
print(flavor)
{% endhighlight %}

{% highlight console %}
Molten lava
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/string-immutability#main.py){: .btn }
