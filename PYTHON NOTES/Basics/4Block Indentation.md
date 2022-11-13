# Block Indentation

Python uses block indentation to define control flow and loop constructs. This contributes to pythons readability.

However it requires the programmer to pay close attention to the use of whitespaces. Thus editor miscalibration could result in code that behaves in unexpected ways.

Python uses the colon symbol ```:``` and indentation for showing where the blocks of code begin and end. That is blocks in python, such as functions, loops, if clause and other constructs, have no ending identifiers. All blocks start with colon and then contain the indented lines below it.


Lets look at some examples

- function related example

```
def fun1():
    a = 2
    return a

print(fun1())

```
- if related example

```
if a = 2:
    print('2')
else:
    print(a)
```

You can also put blocks that contain single-line statement on the same line like example given below although this is not considered as a good practice

```
if a = 2: print('2')
else: print(a)
```
An empty block causes an indentation error. You can use ```pass``` to avoid indentation error caused by an empty block. 

```
def fun2():
    pass
```

Python interpreter normally assigns indentation for you but sometimes you may need to put indentation in certain cases. You can use ```Tab``` key on the keyboard to put indenation in python. ```1 Tab = 4 spaces```. You can even put 4 spaces to avoid indentation error if you don't want to use ```Tab``` or just for a change from using ```Tab``` keyword.

###### Next
[Datatypes](./5Datatypes.md)

###### Previous
[Print function](./3Print%20function.md)