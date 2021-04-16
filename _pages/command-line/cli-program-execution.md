---
layout: default
title: CLI Program Execution
parent: Command Line Interface
---

# CLI Program Execution
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
You can easily execute your Python programs directly from the command line. First, navigate to the directory the `.py` file is stored. Then, use the `python3` command to execute the file.

## Example: `addition.py`
The following program is saved in `/Users/bianca/test/addition.py`. It prompts the user for two numbers using the `input()` function, then displays the sum:

{% highlight python %}
def main():
    try:
        number1 = int(input('Enter 1st number: '))
        number2 = int(input('Enter 2nd number: '))
    except:
        print('\nYou must enter two integer arguments. Ending Execution')
        return
    
    print(f'\nThe sum is {number1 + number2}')

if __name__ == '__main__':
    main()
{% endhighlight %}

### Navigate to directory and execute:


