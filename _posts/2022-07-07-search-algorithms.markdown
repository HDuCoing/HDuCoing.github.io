---
layout: post
title:  "Search Algorithms"
date:   2022-07-07 00	
categories: jekyll update
---

Search Algorithms are extremely important for searching through data structures. It is also important to learn these algorithms in order to understand coding on a deeper level than just the output. The faster we can make our codes work with an appropriate O notation boundation. 

<h3> Binary Search </h3>
<p> 
The purpose of this basic binary search is to take a list, and the element of a list and return the index of the element. You can find my full github code for this 
<a href="https://github.com/HDuCoing/Python/blob/Default/Binary%20Search.py">here</a>
</p>
{% highlight python %}
def binary_search(the_list, item):
    lower = 0
    upper = len(the_list) - 1
    while True:
        if upper < lower:
            return -1
        middle = (lower + upper) // 2
        if the_list[middle][0] < item:
            lower = middle + 1
        elif the_list[middle][0] > item:
            upper = middle - 1
        else:
            return middle
{% endhighlight %}