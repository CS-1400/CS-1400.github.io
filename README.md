CS-1030 

{% capture some_var %}
```Python
print("Learn to Code")
```
{% endcapture %}
{% assign some_var = some_var | markdownify %}
{% include fix_linenos.html code-some_var %}
