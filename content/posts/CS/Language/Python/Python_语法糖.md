---
title: ' Python： 语法糖'
date: 2023-10-17T10:59:04+08:00
image: ""
tags:  ["skill","Python",sssss"Tutorial"]
description:  'Python 语法笔记'
categories: 
   - "CodeLanguage"

   
---



# Python 语法糖

##  装饰器

Python 中一个著名的语法糖就是装饰器。装饰器是一种闭包（即函数嵌套函数），其作用在于拓宽原函数的功能，可以在不对原函数作任何修改的情况下，拓宽函数的功能，同时有效避免重复代码，增加了代码的可读性。

下面以除法作简单示例，在除法中除数不能为零，所以在两数相除前应当检查除数是否为零：
1. 只使用函数

```Python
def check(b):
   if b == 0；
       return False
   else:
       return True

def division(a, b):
   if check(b):
       return a/b
   else:
       print("Divisor cannot be zero!")
```

2. 装饰器用法

```python
def check(func):
   def wrapper(*args, **kwargs):
      if args[1] == 0
         print("Divisor cannot be zero!")
         return None
      else:
         return func(*args, **kwargs)
   return wrapper


@check
def division(a, b):
   return a/b
```