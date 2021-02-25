---
layout: default
title: Data Types
has_children: true
has_toc: false
---
# Data Types
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
A specific type of data; defines the values it can represent and the actions that can be performed on it.
- [Python Docs: Built-in Types](https://docs.python.org/3/library/stdtypes.html)


## Example

{% highlight python %}
def main():

    my_float = 6.2
    my_string = 'Ruiz'

    print(f'my_float type:\t{type(my_float)}')
    print(f'my_string type:\t{type(my_string)}')

if __name__ == '__main__':
    main()
{% endhighlight %}

- Console Output:
{% highlight console %}
my_float type:  <class 'float'>
my_string type: <class 'str'>
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/data-types#main.py){: .btn }



## Built-in Types
Below is a table of data types we'll learn and use most often in CS-1030.

| Type 	| Principal Type 	| Mutability 	| Example  |
|-	|-	|-	|- |
| ```str``` 	| Sequence 	| Immutable 	| 'Ruiz', '15' |
| ```int``` 	| Numeric 	| Immutable	| 5, 10000 |
| ```float``` 	| Numeric 	| Immutable	| 8.9, 900.0 |
| ```bool``` 	|  Comparison	| Immutable	| True, False |
| ```list``` 	|  Sequence	| Mutable	| [1,2,3], ['and','or'] |
| ```tuple``` 	|  Sequence	| Immutable	| (1,2,3), ('and','or) |
| ```dict``` 	|  Mapping	| Mutable	| {'flavor': 'sugar', 'frosting': 'almond'} |
| ```range``` 	|  Sequence	| Immutable	| range(10) |
