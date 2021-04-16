---
layout: default
title: CLI Program Arguments
parent: Command Line Interface
---

# CLI Program Arguments
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Programs can be written to accept command-line arguments when they are executed. This requires the use of the `sys.argv` list. 
- The first item in this list (index 0) is always the name of the file being executed. 
- Any additional items in this list are arguments supplied on the command line.
- The module `sys` must be imported to access the `sys.argv` list.

## `argv.py`
The following program prints items in the sys.argv list. It is saved in the `/Users/bianca/test` directory.

{% highlight python %}
import sys

def main():
    # print entire argv list:
    print(f'\nargv list: {sys.argv}')
    
    # print filename stored in first element:
    print(f'Filename:  {sys.argv[0]}')
    
    # print any command-line arguments:
    for argument in sys.argv[1:]:
        print(argument)
    
if __name__ == '__main__':
    main()
{% endhighlight %}

### Navigate to directory and execute:

![](/assets/cli-argv.png)

## `addition-cli.py`
The following program accepts two integer arguments from the command line, then displays the sum. It is saved in the `/Users/bianca/test` directory.

{% highlight python %}
import sys

def main():
    try:
        number1 = int(sys.argv[1])
        number2 = int(sys.argv[2])
    except ValueError:
        print('\nYou must enter two integer arguments. Ending Execution')
        return
    
    print(f'\nThe sum is {number1 + number2}')

if __name__ == '__main__':
    main()
{% endhighlight %}

### Navigate to directory and execute:

![](/assets/cli-program-execution-2.png)

