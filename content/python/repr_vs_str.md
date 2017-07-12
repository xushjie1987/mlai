Title: __repr__ vs. __str__  
Slug: repr_vs_str  
Summary: __repr__ vs. __str__ in Python.    
Date: 2016-01-23 12:00  
Category: Python  
Tags: Basics    
Authors: Chris Albon  

Want to learn more? I recommend these Python books: [Python for Data Analysis](http://amzn.to/2ljV9wY), [Python Data Science Handbook](http://amzn.to/2m0mgMB), and [Introduction to Machine Learning with Python](http://amzn.to/2mjYiwK).

## Preliminaries


```python
import datetime
```

## Create A Simple Object


```python
class Regiment(object):

    def __init__(self, date=datetime.datetime.now()):
        self.date = date

    def __repr__(self):
        return date

    def __str__(self):
        return str(date)
```

`__repr__` is for the developer. It is string representation of the object and the code needed to reproduce the object.

`__str__` is the output for the end user. It prints what the user wants to see.