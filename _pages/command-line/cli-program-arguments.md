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

## argv.py
The following program prints items in the sys.argv list. It is save in the `/Users/bianca/test` directory.

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
