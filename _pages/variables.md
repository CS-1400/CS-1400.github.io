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


## Assignment Statements
Variable names **must** be to the left of the assignment operator; values **must** be to the right:
- ```flavor = 'chocolate chip'```
- ~~```'chocolate chip' = flavor```~~

## Naming Rules
- [Python PEP8: Variable Names](https://www.python.org/dev/peps/pep-0008/#type-variable-names)
- No spaces.
- First character **must** be either an alphabetic character or an underscore.
- Can only contain alphabetic characters, numeric characters, or underscores.
- Cannot be a reserved word:

|--------|----------|----------|--------|
| None   | continue | global   | pass   |
| True   | def      | if       | raise  |
| and    | del      | import   | return |
| as     | elif     | in       | try    |
| assert | else     | is       | while  |
| async  | except   | lambda   | with   |
| await  | finally  | nonlocal | yield  |
| break  | for      | not      | or     |
| False  | class    | from     |        |

## Reassignment
When a value is *bound* to a variable, it is not permanent. Python code is executed sequentially, and keeps no record of prior variable values:

{% highlight python %}
def main():

    # I buy 3 cookies at Crumbl:
    cookies = 3
    print('Three cookies: nom nom nom')
    # I buy one more cookie:
    cookies += 1
    print('Fourth cookie: nom nom nom')
    # I buy one last cookie:
    cookies += 1
    print('Fifth cookie: nom nom nom')
    # The value of cookie is now 5:
    print(f'I ate {cookies} cookies!!')

if __name__ == '__main__':
    main()
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/variables#main.py){: .btn }
