---
layout: default
title: Errors
---

# Errors
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Definition
The three types of errors we encounter while programming are syntax, runtime, and logic. Each of these errors are described below, along with a small example.
- [Python Docs: Errors and Exceptions](https://docs.python.org/3/tutorial/errors.html)

## Syntax Erros
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

## Exception Handling
It is always best practice to place error-prone code inside of try/except blocks. When an error occurs it will be handled gracefully, instead of crashing.

### No exception handling
{% highlight python %}
def main():
    
    quantity = int(input('How many cookies do you want? '))   
    print(f'Excellent! Here are your {quantity} cookies...')

if __name__ == '__main__':
    main()
{% endhighlight %}
- Console output when user enters 'y' instead of a number:
{% highlight console %}
How many cookies do you want? y
Traceback (most recent call last):
  File "main.py", line 7, in <module>
    main()
  File "main.py", line 3, in main
    quantity = int(input('How many cookies do you want? '))   
ValueError: invalid literal for int() with base 10: 'y'
{% endhighlight %}
[Run on Repl.it](https://repl.it/@bianca_ruiz/no-exception-handling#main.py){: .btn .mr-4}[Watch in PythonTutor](http://www.pythontutor.com/visualize.html#code=def%20main%28%29%3A%0A%20%20%20%20%0A%20%20%20%20quantity%20%3D%20int%28input%28'How%20many%20cookies%20do%20you%20want%3F%20'%29%29%20%20%20%0A%20%20%20%20print%28f'Excellent!%20Here%20are%20your%20%7Bquantity%7D%20cookies...'%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false){: .btn}

### Proper exception handling
{% highlight python %}
def main():
    
    while True:
        try:
            quantity = int(input('How many cookies do you want? '))
            break
        except:
            print('Please enter a whole number\n')
            continue
    
    print(f'\nExcellent! Here are your {quantity} cookies...')

if __name__ == '__main__':
    main()
{% endhighlight %}
- Console output when user enters 'y' instead of a number:
{% highlight console %}
How many cookies do you want? y
Please enter a whole number

How many cookies do you want? 
{% endhighlight %}

[Run on Repl.it](https://repl.it/@bianca_ruiz/exception-handling#main.py){: .btn .mr-4}[Watch in PythonTutor](http://www.pythontutor.com/visualize.html#code=def%20main%28%29%3A%0A%20%20%20%20%0A%20%20%20%20while%20True%3A%0A%20%20%20%20%20%20%20%20try%3A%0A%20%20%20%20%20%20%20%20%20%20%20%20quantity%20%3D%20int%28input%28'How%20many%20cookies%20do%20you%20want%3F%20'%29%29%0A%20%20%20%20%20%20%20%20%20%20%20%20break%0A%20%20%20%20%20%20%20%20except%3A%0A%20%20%20%20%20%20%20%20%20%20%20%20print%28'Please%20enter%20a%20whole%20number%5Cn'%29%0A%20%20%20%20%20%20%20%20%20%20%20%20continue%0A%20%20%20%20%0A%20%20%20%20print%28f'%5CnExcellent!%20Here%20are%20your%20%7Bquantity%7D%20cookies...'%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false){: .btn}
