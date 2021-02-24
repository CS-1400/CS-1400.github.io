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
There are three types of errors we encounter while programming: syntax, runtime, and logic. 
- [Python Docs: ]()

## Syntax Erros
Syntax errors are caused by not following the rules of the language. Examples: beginning a variable name with a number, forgetting to close parenthesis or quotes, or misspelling keywords. The editor will usually bring these to your attention by underlining them in red.
- ```Print('Hello there!')``` (The *p* in print shouldn't be capitalized)

## Runtime Errors
Runtime Errors happen during program execution, and cause your program to crash. They are caused by asking the computer something it cannot do, such as division by zero or trying to access the 5th character of a four character string.
- ```print(5 / 0)```

## Logic Errors
Logic errors occur when the program runs fine, there are no obvious errors, but the output is incorrect. This can be caused by incorrect algorithms, or mistyping an operator (ex: + instead of -).
- ```total = subtotal - tax```  (The subtraction operator should be an addition operator)

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
Console output when user enters 'y' instead of a number:


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
Console output when user enters 'y' instead of a number:


[Run on Repl.it](https://repl.it/@bianca_ruiz/#main.py){: .btn }
