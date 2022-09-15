# Python - Everything is object

![alt text](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/252/r_208403_QPSN8.jpg)

# Background Context
Now that we understand that everything is an object and have a little bit of knowledge, let’s pause and look a little bit closer at how Python works with different types of objects.

BTW, have you ever modified a variable without knowing it or wanting to? I mean:

>>> a = 1
>>> b = a
>>> a = 2
>>> b
1
>>> 
OK. But what about this?

>>> l = [1, 2, 3]
>>> m = l
>>> l[0] = 'x'
>>> m
['x', 2, 3]
>>> 



This project is a little bit different than the usual projects. The first part is only questions about Python’s specificity like “What would be the result of…”. You should read all documentation first (as usual :)), then take the time to think and brainstorm with your peers about what you think and why. Try to do this without coding anything for a few hours.

Trying examples in the Python interpreter will give you most of the answers without having to think about it. Don’t go this route. First read, then think, then brainstorm together. Only then you can test in the interpreter.

It’s important that you truly understand the reasons behind the answers of all those tasks so that you can apply the same logic to other variables and other variable types. The biggest mandatory task is the blog post and it will count for 50% of the total score of the project.

Note that during interviews for Python positions, you will most likely have to answer to these type of questions.

All your answers should be only one line in a file. No space before or after the answer.

# Resources
## Read or watch:

** 9.10. Objects and values
* 9.11. Aliasing
* Immutable vs mutable types
* Mutation (Only this chapter)
* 9.12. Cloning lists
* Python tuples: immutable but potentially changing

# Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

# General
** Why Python programming is awesome
* What is an object
* What is the difference between a class and an object or instance
* What is the difference between immutable object and mutable object
* What is a reference
* What is an assignment
* What is an alias
* How to know if two variables are identical
* How to know if two variables are linked to the same object
* How to display the variable identifier (which is the memory address in the CPython implementation)
* What is mutable and immutable
* What are the built-in mutable types
* What are the built-in immutable types
* How does Python pass variables to functions

# Requirements
## Python Scripts
** Allowed editors: vi, vim, emacs
* All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)
* All your files should end with a new line
* The first line of all your files should be exactly #!/usr/bin/python3
* A README.md file, at the root of the folder of the project, is mandatory
* Your code should use the pycodestyle (version 2.8.*)
* All your files must be executable
* The length of your files will be tested using wc

# .txt Answer Files
** Only one line
* No Shebang
* All your files should end with a new line

![alt text](https://media.giphy.com/media/wAjfQ9MLUfFjq/giphy.gif)

## Tests :heavy_check_mark:

* [tests](./tests): Folder of test files.

## Tasks :page_with_curl:

* **0. Who am I?**
  * [0-answer.txt](./0-answer.txt): What function would you use to print the type of an object?


* **1. Where are you?**
  * [1-answer.txt](./1-answer.txt): How do you get a variable's identifier (which is the memory address in the CPython implementation)?

* **2. Right count**
  * [2-answer.txt](./2-answer.txt): In the following code, do `a` and `b` point to the same object?
```
>>> a = 89
>>> b = 100
```

* **3. Right count =**
  * [3-answer.txt](./3-answer.txt): In the following code, do `a` and `b` point to the same object?
```
>>> a = 89
>>> b = 89
```

* **4. Right count =**
  * [4-answer.txt](./4-answer.txt): In the following code, do `a` and `b` point to the same object?
```
>>> a = 89
>>> b = a
```

* **5. Right count =+**
  * [5-answer.txt](./5-answer.txt): In the following code, do `a` and `b` point to the same object?
```
>>> a = 89
>>> b = a + 1
```

* **6. Is equal**
  * [6-answer.txt](./6-answer.txt): What do these 3 lines print?
```
>>> s1 = "Best School"
>>> s2 = s1
>>> print(s1 == s2)
```

* **7. Is the same**
  * [7-answer.txt](./7-answer.txt): What do these 3 lines print?
```
>>> s1 = "Best"
>>> s2 = s1
>>> print(s1 is s2)
```

* **8. Is really equal**
  * [8-answer.txt](./1-answer.txt): What do these 3 lines print?
```
>>> s1 = "Best School"
>>> s2 = "Best School"
>>> print(s1 == s2)
```

* **9. Is really the same**
  * [9-answer.txt](./9-answer.txt): What do these 3 lines print?
```
>>> s1 = "Best School"
>>> s2 = "Best School"
>>> print(s1 is s2)
```

* **10. And with a list, is it equal**
  * [10-answer.txt](./10-answer.txt): What do these 3 lines print?
```
>>> l1 = [1, 2, 3]
>>> l2 = [1, 2, 3]
>>> print(l1 == l2)
```

* **11. And with a list, is it the same**
  * [11-answer.txt](./11-answer.txt): What do these 3 lines print?
```
>>> l1 = [1, 2, 3]
>>> l2 = [1, 2, 3]
>>> print(l1 is l2)
```

* **12. And with a list, is it really equal**
  * [12-answer.txt](./12-answer.txt): What do these 3 lines print?
```
>>> l1 = [1, 2, 3]
>>> l2 = l1
>>> print(l1 == l2)
```

* **13. And with a list, is it really the same**
  * [13-answer.txt](./13-answer.txt): What do these 3 lines print?
```
>>> l1 = [1, 2, 3]
>>> l2 = l1
>>> print(l1 is l2)
```

* **14. List append**
  * [14-answer.txt](./14-answer.txt): What does this script print?
```
l1 = [1, 2, 3]
l2 = l1
l1.append(4)
print(l2)
```

* **15. List add**
  * [15-answer.txt](./15-answer.txt): What does this script print?
```
l1 = [1, 2, 3]
l2 = l1
l1 = l1 + [4]
print(l2)
```

* **16. Integer incrementation**
  * [16-answer.txt](./16-answer.txt): What does this script print?
```
def increment(n):
    n += 1

a = 1
increment(a)
print(a)
```

* **17. List incrementation**
  * [17-answer.txt](./17-answer.txt): What does this script print?
```
def increment(n):
    n.append(4)

l = [1, 2, 3]
increment(l)
print(l)
```

* **18. List assignation**
  * [18-answer.txt](./18-answer.txt): What does this script print?
```
def assign_value(n, v):
    n = v

l1 = [1, 2, 3]
l2 = [4, 5, 6]
assign_value(l1, l2)
print(l1)
```

* **19. Copy a list object**
  * [19-copy_list.py](./19-copy_list.py): Python function `def copy_list(l):` that returns a copy of a list.

* **20. Tuple or not?**
  * [20-answer.txt](./20-answer.txt): Is `a` a tuple?
```
a = ()
```

* **21. Tuple or not?**
 * [21-answer.txt](./21-answer.txt): Is `a` a tuple?
```
a = (1, 2)
```

* **22. Tuple or not?**
  * [22-answer.txt](./22-answer.txt): Is `a` a tuple?
```
a = (1)
```

* **23. Tuple or not?**
  * [23-answer.txt](./23-answer.txt): Is `a` a tuple?
```
a = (1, )
```

* **24. Who I am?**
  * [24-answer.txt](./24-answer.txt): What does this script print?
```
a = (1)
b = (1)
a is b
```

* **25. Tuple or not**
  * [25-answer.txt](./25-answer.txt): What does this script print?
```
a = (1, 2)
b = (1, 2)
a is b
```

* **26. Empty is not empty**
  * [26-answer.txt](./26-answer.txt): What does this script print?
```
a = ()
b = ()
a is b
```

* **27. Still the same**
  * [27-answer.txt](./27-answer.txt): Will the last line of this script print `139926795932424`?
```
>>> id(a)
139926795932424
>>> a
[1, 2, 3, 4]
>>> a = a + [5]
>>> id(a)
```

* **28. Same or not?**
  * [28-answer.txt](./28-answer.txt): Will the last line of this script print `139926795932424`?
```
>>> a
[1, 2, 3]
>>> id (a)
139926795932424
>>> a += [4]
>>> id(a)
```

* **29. #pythonic**
  * [100-magic_string.py](./100-magic_string.py): Python function `magic_string()` that returns the string `"BestSchool"` n times the number of iteration.

* **30. Low memory cost**
  * [101-locked_class.py](./101-locked_class.py): Python class `LockedClass` with no attributes that prevents the user from dynamically creating any new instance attributes not called `first_name`.

* **31. int 1/3**
  * [103-line1.txt](./103-line1.txt): How many `int` objects are created by the execution of the first line in this script?
  * [104-line2.txt](./104-line2.txt): How many `int` objects are created by the execution of the second line in this script?
```
a = 1
b = 1
```

* **32. int 2/3**
  * [104-line1.txt](./104-line1.txt): How many `int` objects are created by the execution of the first line in this script?
  * [104-line2.txt](./104-line2.txt): How many `int` objects are created by the execution of the second line in this script?
  * [104-line3.txt](./104-line3.txt): After the execution of line 3, is the `int` object pointed to by `a` deleted?
  * [104-line4.txt](./104-line4.txt): After the execution of line 4, is the `int` object pointed to by `b` deleted?
  * [104-line5.txt](./104-line5.txt): How many `int` objects are created by the execution of the last line in this script?
```
a = 1024
b = 1024
del a
del b
c = 1024
```

* **33. int 3/3**
  * [105-line1.txt](./105-line1.txt): Before the execution of line 2 in this script, how many `int` objects have been created and are still in memory?
```
print("I")
print("Love")
print("Python")
```
![alt text](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/70f9ea0e969dfcc407a7427aba4786d87a920494.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20220628%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220628T145801Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=28cc1540430447d619d0bde0fd16f57d694de58ae054aad768cb3f0b018d4095)


* **34. Clear strings**
  * [106-line1.txt](./106-line1.txt): How many `str` objects are created by the execution of the first line in this script?
  * [106-line2.txt](./106-line2.txt): How many `str` objects are created by the execution of the second line in this script?
  * [106-line3.txt](./106-line3.txt): After the execution of line 3, is the `str` object pointed to by `a` deleted?
  * [106-line4.txt](./106-line4.txt): After the execution of line 4, is the `str` object pointed to by `b` deleted?
  * [106-line5.txt](./106-line5.txt): How many `str` objects are created by the execution of the last line in this script?
```
a = "SCHL"
b = "SCHL"
del a
del b
c = "SCHL"
```
