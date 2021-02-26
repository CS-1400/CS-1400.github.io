---
layout: default
title: Exception Handling
parent: Errors
---

# Exception Handling
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Exception handling allows programmers to deal with an error gracefully and avoid a sudden program crash. It is best practice to place error-prone code inside of try/except blocks. 
- Python Docs Wiki: [Handling Exceptions](https://wiki.python.org/moin/HandlingExceptions)

### Without exception handling
Run the program below, and enter non-numeric input at the prompt. Notice that the runtime error (exception) crashes the program.
<iframe height="400px" width="100%" src="https://repl.it/@bianca_ruiz/no-exception-handling?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>

[Watch in PythonTutor](http://www.pythontutor.com/visualize.html#code=def%20main%28%29%3A%0A%20%20%20%20%0A%20%20%20%20quantity%20%3D%20int%28input%28'How%20many%20cookies%20do%20you%20want%3F%20'%29%29%20%20%20%0A%20%20%20%20print%28f'Excellent!%20Here%20are%20your%20%7Bquantity%7D%20cookies...'%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&cumulative=false&curInstr=0&heapPrimitives=nevernest&mode=display&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false){: .btn}

### With exception handling
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
