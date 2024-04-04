# This is Python Tutorial

This is our first program in python


```python
print("Hellow World")
```

    Hellow World
    

$a=b+c$

# Variables


```python
x = 3
```


```python
%whos
```

    Variable   Type    Data/Info
    ----------------------------
    x          int     3
    


```python
print(type(x))
```

    <class 'int'>
    


```python
x = 5.7
```


```python
%whos
```

    Variable   Type     Data/Info
    -----------------------------
    x          float    5.7
    


```python
print(type(x))
```

    <class 'float'>
    


```python
abcd = 556.32
```


```python
%whos
```

    Variable   Type     Data/Info
    -----------------------------
    abcd       float    556.32
    x          float    5.7
    


```python
a,b,c,d,f = 3,5,6.0,7.2,-3
```


```python
%whos
```

    Variable   Type     Data/Info
    -----------------------------
    a          int      3
    abcd       float    556.32
    b          int      5
    c          float    6.0
    d          float    7.2
    f          int      -3
    x          float    5.7
    


```python
del abcd
```


```python
%whos
```

    Variable   Type     Data/Info
    -----------------------------
    a          int      3
    b          int      5
    c          float    6.0
    d          float    7.2
    f          int      -3
    x          float    5.7
    


```python
print(abcd)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[17], line 1
    ----> 1 print(abcd)
    

    NameError: name 'abcd' is not defined



```python
c = 2+4j
```


```python
print(type(c))
```

    <class 'complex'>
    


```python
s = "hellow how are you"
```


```python
print(type(s))
```

    <class 'str'>
    

# Operators


```python
sumOfaAndb =a+b
```


```python
print(sumOfaAndb)
```

    8
    


```python
type(sumOfaAndb)
```




    int




```python
type(a+d)
```




    float




```python
s1="hellow"
s2="world"
s=s1+s2
print(s)
```

    hellowworld
    


```python
startingTimeOfTheCourse=2.0
```


```python
%whos
```

    Variable                  Type       Data/Info
    ----------------------------------------------
    a                         int        3
    b                         int        5
    c                         complex    (2+4j)
    d                         float      7.2
    f                         int        -3
    s                         str        hellowworld
    s1                        str        hellow
    s2                        str        world
    startingTimeOfTheCourse   float      2.0
    sumOfaAndb                int        8
    x                         float      5.7
    

# Bool


```python
a=True
b=True
c=False
```


```python
%whos
```

    Variable                  Type     Data/Info
    --------------------------------------------
    a                         bool     True
    b                         bool     True
    c                         bool     False
    d                         float    7.2
    f                         int      -3
    s                         str      hellowworld
    s1                        str      hellow
    s2                        str      world
    startingTimeOfTheCourse   float    2.0
    sumOfaAndb                int      8
    x                         float    5.7
    


```python
print(a and b)
print(a and c)
print(b and c)
```

    True
    False
    False
    


```python
d=a or c
print(d)
```

    True
    


```python
not(a)
```




    False




```python
not(c)
```




    True




```python
not (a and b) or (c or d)
```




    True



# Comparisons


```python
print(2<3)
```

    True
    


```python
c=2<3
print(c)
print(type(c))
```

    True
    <class 'bool'>
    


```python
d=3==4
print(d)
```

    False
    


```python
3==3.0
```




    True




```python
x=4
y=9
z=8.3
r=-3
```


```python
(x<y) and (z<y) or (r==x)
```




    True




```python
print((not(2!=3)and True) or (False and True))
```

    False
    

# Functions


```python
print(round(4.345))
```

    4
    


```python
print(round(4.556789,3))
```

    4.557
    


```python
print(divmod(27,5))
```

    (5, 2)
    


```python
G=divmod(34,9)
print(G)
type(G)
```

    (3, 7)
    




    tuple




```python
G[0]
```




    3




```python
G[1]
```




    7




```python
isinstance(3,int)
```




    True




```python
isinstance(3.0,int)
```




    False




```python
isinstance(3.0,(int,float))
```




    True




```python
isinstance(2+4j,(int,float,complex,str))
```




    True




```python
2**4
```




    16




```python
pow(2,4)
```




    16




```python
pow(2,4,7)
```




    2




```python
x=input("Enter a number :")
```

    Enter a number : 22
    


```python
type(x)
```




    str




```python
x=int(x)
```


```python
type(x)
```




    int




```python
print(x-4)
```

    18
    


```python
a=float(input("Enter a real number :"))
```

    Enter a real number : 14
    


```python
type(a)
```




    float




```python
pow??
```


    [1;31mSignature:[0m [0mpow[0m[1;33m([0m[0mbase[0m[1;33m,[0m [0mexp[0m[1;33m,[0m [0mmod[0m[1;33m=[0m[1;32mNone[0m[1;33m)[0m[1;33m[0m[1;33m[0m[0m
    [1;31mDocstring:[0m
    Equivalent to base**exp with 2 arguments or base**exp % mod with 3 arguments
    
    Some types, such as ints, are able to use a more efficient algorithm when
    invoked using the three argument form.
    [1;31mType:[0m      builtin_function_or_method



```python
help(pow)
```

    Help on built-in function pow in module builtins:
    
    pow(base, exp, mod=None)
        Equivalent to base**exp with 2 arguments or base**exp % mod with 3 arguments
        
        Some types, such as ints, are able to use a more efficient algorithm when
        invoked using the three argument form.
    
    

# Control Flow


```python
a=int(input())
b=int(input())
if a>b:
    print(a)
    print("I am still inside if condition")
if b>a:
    print(b)
```

     22
     4
    

    22
    I am still inside if condition
    


```python
a=int(input())
b=int(input())
if a>b:
    print(a)
else:
    print(b)
```

     10
     45
    

    45
    


```python
a=int(input())
b=int(input())
if a==b:
    print("Equal")
elif a>b:
    print("A")
else:
    print("B")
print("Not in if")
```

     10
     5
    

    A
    Not in if
    


```python
a=9
b=10
print("A") if a>b else print ("==") if a==b else print ("B")
```

    B
    


```python

```
