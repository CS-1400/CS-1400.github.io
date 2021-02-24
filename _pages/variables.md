---
layout: default
title: Variables
---
# Variables
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
Variables are named areas of memory that we can use to store date. All variables have three things: a name, a type, and a value.
- [Python PEP8: Variable Names](https://www.python.org/dev/peps/pep-0008/#type-variable-names)

## Assignment Statements
Variable names **must** be to the left of the assignment operator; values **must** be to the right:
- ```flavor = 'chocolate chip'```
- ~~```'chocolate chip' = flavor```~~

## Naming Rules
- No spaces.
- First character **must** be either an alphabetic character or an underscore.
- Can only contain alphabetic characters, numeric characters, or underscores.
- Cannot be a reserved word:

|-|-|-|-|-|-|-|
| False | class | from | or | None | continue | global |
| pass | True | def | if | raise | and | del |
| import | return | as | elif | in | try | assert |
| else | is | while | async | except | lambda | with |
| await | finally | nonlocal | yield | break | for | not |

Python Code:
{% highlight python %}
def main():
    
if __name__ == '__main__':
    main()
{% endhighlight %}

Console Output:
{% highlight text %}
Bianca's favorite food is cookies, at $4.50 a pop.
3 cookies cost a total of $13.50
         BIANCA
    bianca     
BiAnCa
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/f-strings#main.py){: .btn }

## Escape Sequences

