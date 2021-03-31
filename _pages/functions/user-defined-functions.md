---
layout: default
title: User-defined Functions
parent: Functions
---
# User-defined Functions
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
User-defined functions are custom functions defined by a programmer. They are used to organize code and reduce repetitive code. After a function is defined, they can be executed by calling their name. Functions are not executed when they are defined.

## Composition
{% highlight Python %}
def function_name(parameter1, parameter2):
    # function code indented under definition
    # more function code
    # even more function code

function_name(argument1, argument2)
{% endhighlight %}

## Example
The example program below accepts the user's height and weight, calculates the BMI, then displays the result to the console. Step through the program and observe what is happening in memory to better understand how user-defined functions work.

The program consists of 3 seperate functions (`main`, `calculate_bmi`, `calculate_inches`). These three functions organize the code and make the main algorithm more readable. There are no commands or variables occupying the global space, all code is inside functions (this is always best practice when programming).

As you step through the execution of the program, notice that some functions have return values, some do not. Also notice that some functions accept arguments, but some don't. It all depends on how the programmer defines the function. 
- Note: Parameter **names** in the function definition do not need to match argument names in the calling statement. **Quantity** must match, though.

Also notice that functions are only executed when they are called by their name, not when they are initially defined. 
<iframe width="100%" height="800" frameborder="1" src="https://pythontutor.com/iframe-embed.html#code=def%20calculate_bmi%28lbs,%20inches%29%3A%0A%20%20%20%20return%20703%20*%20lbs%20/%20%28inches%20**%202%29%0A%0Adef%20calculate_inches%28height%29%3A%0A%20%20%20%20return%20int%28height%5B0%5D%29%20*%2012%20%2B%20int%28height%5B1%5D%29%0A%0Adef%20main%28%29%3A%0A%20%20%20%20weight%20%3D%20int%28input%28%22Enter%20weight%20in%20pounds%3A%20%22%29%29%0A%20%20%20%20height%20%3D%20input%28%22Enter%20height%20as%20feet,inches%20%28no%20spaces%29%3A%20%22%29.split%28','%29%0A%0A%20%20%20%20inches%20%3D%20calculate_inches%28height%29%0A%20%20%20%20BMI%20%3D%20calculate_bmi%28weight,%20inches%29%0A%0A%20%20%20%20print%28f'%5CnBMI%3A%20%7BBMI%3A.1f%7D'%29%0A%0Aif%20__name__%20%3D%3D%20'__main__'%3A%0A%20%20%20%20main%28%29&codeDivHeight=400&codeDivWidth=350&cumulative=false&curInstr=0&heapPrimitives=nevernest&origin=opt-frontend.js&py=3&rawInputLstJSON=%5B%22120%22,%225,4%22%5D&textReferences=false"> </iframe>

## Passing Arguments
When arguments passed to a function are immutable (strings, integers, etc), a copy of the value of the argument is assigned to the function parameter. When the data type of an argument passed to a function parameter is mutable, a reference to the actual argument is passed. This can cause unwanted side effects.
### Functions as "Black Boxes"
