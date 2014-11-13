## Phylosophy

Things should be short and easy to understand.

### Which code should be within `utils.py`

We should have only code that is intended to be used in many places, that is, if a section of code is only
used in a view and nowhere else, it's better to keep it in that view and not in `utils.py`. However, when a section 
of code is used in several views, it qualifies for being under `utils.py`

## Table of contents

* Urls


## URLS 

Simple tips on how to define URLS.


### Use `/` slash at the end of the URL

Incorrect example 

```python 
r'^(?P<slug>[-\w]+)/settings$'
```

Correct example
```python 
r'^(?P<slug>[-\w]+)/settings/$'
```