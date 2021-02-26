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

## Description
Variables are named areas of memory that we can use to store data. The Python interpreter categorizes all variables as **Objects**. All objects have three things: a name, a type, and a value.


## Assignment Statements
Assignment statements *bind* a value with a name. Variable names **must** be to the left of the assignment operator; values **must** be to the right:
- ```flavor = 'chocolate chip'```
- ~~```'chocolate chip' = flavor```~~

## Naming Rules
- [Python PEP8: Variable Names](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names)
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

<iframe src="https://trinket.io/embed/python/caaba677fb" width="100%" height="600" frameborder="0" marginwidth="0" marginheight="0" allowfullscreen></iframe>

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

[Run on Repl.it](https://repl.it/@bianca_ruiz/variables#main.py){: .btn .mr-4}
[Watch on PythonTutor](http://www.pythontutor.com/visualize.html#code=def%20main%28%29%3A%0A%0A%20%20%20%20%23%20I%20buy%203%20cookies%20at%20Crumbl%3A%0A%20%20%20%20cookies%20%3D%203%0A%20%20%20%20print%28'Three%20cookies%3A%20nom%20nom%20nom'%29%0A%20%20%20%20%23%20I%20buy%20one%20more%20cookie%3A%0A%20%20%20%20cookies%20%2B%3D%201%0A%20%20%20%20print%28'Fourth%20cookie%3A%20nom%20nom%20nom'%29%0A%20%20%20%20%23%20I%20buy%20one%20last%20cookie%3A%0A%20%20%20%20cookies%20%2B%3D%201%0A%20%20%20%20print%28'Fifth%20cookie%3A%20nom%20nom%20nom'%29%0A%20%20%20%20%23%20The%20value%20of%20cookie%20is%20now%205%3A%0A%20%20%20%20print%28f'I%20ate%20%7Bcookies%7D%20cookies!!'%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false){: .btn }
