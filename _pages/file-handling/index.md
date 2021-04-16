---
layout: default
title: File Handling
has_children: true
has_toc: false
---

# File Handling
{: .no_toc }
## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Description
Variables store data during the execution of the program, but "disapear" when the program ends. Data saved in files will persist beyond the execution of the program. Python provides methods for programmers to read, write, and modify file contents.
- Python Docs: [Reading and Writing Files](https://docs.python.org/3/tutorial/inputoutput.html#reading-and-writing-files)

## File Streams
In order to read or write file data, you must always do three things in order:
1. Open the file.
2. Perform some processing,
3. Close the file.

Additionaly, your file stream can only go in one direction. This means that you cannot write to a file you open for reading, and vice versa. You specify how you are going to use the file when you open it by indicating the file mode:
- "**r**" mode: Opens the file for reading only.
- "**w**" mode: Opens the file for writing only.
- "**a**" mode: Allows the programmer to add additional data to the end of a file.


## Instructional Videos

<iframe width="373" height="210" src="https://www.youtube.com/embed/QDYIMoA9EOg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<iframe width="373" height="210" src="https://www.youtube.com/embed/vu4QfAhWN7E" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
