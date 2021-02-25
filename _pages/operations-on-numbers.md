---
layout: default
title: Operations on Numbers
---

# Operations on Numbers
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
The Python interpreter will automatically evaluate all expressions. The evaluation follows the normal "PEMDAS" order of operations.
- Python Docs: [Numeric Types](https://docs.python.org/3/library/stdtypes.html#numeric-types-int-float-complex)
- Python Docs: [Operator Precedence](https://docs.python.org/3/reference/expressions.html#operator-precedence)
- Python Module: [math](https://docs.python.org/3/library/math.html)
- Python Module: [statistics](https://docs.python.org/3/library/statistics.html)
- Python Module: [random](https://docs.python.org/3/library/random.html)

## Example

{% highlight python %}
import math
import statistics as st
from random import randint

def main():

    print(4 / 2)                # 2.0
    print(5 // 2)               # 2
    print(5 % 2)                # 1
    print((5 + 2) * 2)          # 14

    print(int(5.6))             # 5
    print(float(8))             # 8.0

    print(math.gcd(4,16))       # 4
    print(math.sqrt(9))         # 3.0
    print(st.mean([5,10,15]))   # 10
    print(randint(5,15))        # any random integer from 5 through 15

if __name__ == '__main__':
    main()
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/operations-on-numbers#main.py){: .btn }
