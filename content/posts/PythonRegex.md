---
title: "PythonRegex"
date: 2021-06-19T21:19:02+05:30
draft: false
author: prajjwal
description: "Guide to emoji usage in Hugo"
---

How To Use RegEx library:

* To import

```python
import re
```

* compile the pattern

```python
obj = re.compile(r'pattern')
# group in pattern can be represnted by '()' and anything in betwwen these paraentheses will create a group with the whole pattern being a pattern 
# e.g. (451)-(1234)


```
* search the string 

```python
search_obj = obj.search(string to be searched)#first occurence
search_obj = obj.findall(string to be searched)#All occurences


```

* to get the first match

```python
search_obj.group()

# if integer is passed in the group method then it gives the interger number group match

```

* to get all matches

```python
search_obj.find_all()

```

##### Table of patterns

```python
'\d' -> Digit
'?' -> matches a group(or element) one or zero time
'*' -> matches a group(or element) zero or more time
'+' -> matches a group(or element) one or more time 
'\w' -> word character
'\s' -> space characters
'\D' -> Not digit
'\W' -> Not Word
'\S' -> Not space
'{number of occurence}' -> Is used to get desired number of repetetions 
'{min, max}' -> Number of occurence in between(including) min and max with greedy(first occurence of maximum) matching 
'{min, max}?' -> Number of occurence in between(including) min and max with non-greedy(first occurence of minimum) matching 
'[anything]' -> equivalent to '(a|n|y|t|h|i|n|g)' group containing individual letters 
'^[anything]' -> equivalent to '(a|n|y|t|h|i|n|g)' group except these individual letters 

```

