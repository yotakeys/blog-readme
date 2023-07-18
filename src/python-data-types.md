### Introduction
Python is a high-level, general-purpose programming language. Its design philosophy emphasizes code readability with the use of significant indentation via the off-side rule.

Python is dynamically typed and garbage-collected. It supports multiple programming paradigms, including structured (particularly procedural), object-oriented and functional programming. It is often described as a "batteries included" language due to its comprehensive standard library.

Python consistently ranks as one of the most popular programming languages.

(Wikipedia)

In python, you can declare your varibles without specifying or declare the datatypes, every variable data types can be changed.

**In this blog, i will only covering datatypes that are commonly used or often used by me*

### Built-in data types
built in data type is a data type that has been provided and can be used by Python after installing it

- -> numeric : int, float
- -> text : str
- -> sequence : list, tuple
- -> mapping : dict
- -> boolean : bool
- -> set : set
- -> none : none


##### Integer
python data type to handle/store integer value

```py
n = int()
n = 10

print(type(n))
# print <class 'int'>

print(n + n)
# print 20

print(n * n)
# print 100
```

##### Float
python data type to handle/store float value
```py
n = float()
n = 10.5

print(type(n))
# print <class 'float'>

print(n + n)
# print 21.0

print(n * n)
# print 110.25
```

##### String
python data type to handle/store text/string value

```py
n = str()
n = "python"

print(type(n))
# print <class 'str'>

print(n + n)
# print "pythonpython"

print(n * 3)
# print "pythonpythonpython"

print(n + ' is the best')
# print "python is the best"

print(n[2])
# print "t"
```

##### Boolean
python data type to handle/store boolean value (true/false), True is 1 and false is 0
```py
n = bool()
n = True

print(type(n))
# print <class 'bool'>

if n:
    print(n)
elif not n:
    print(n)
# print True
```

##### List
python data type to handle/store sequence/many value, list can store different data types in it. you can acces value of list member using the index. List is mutable, it means you can change the value inside the list using thei ndex

```py
n = list()
n = ["python", " is", 10, " the best", [1, 2, 3]]

print(type(n))
# print <class 'list'>

print(n)
# print ['python', ' is', 10, ' the best', [1, 2, 3]]

print(n[4][1])
# print 2

print(n[0] + n[1] + n[3])
# print "python is the best"
```

##### Tuple
tuple is actually the same as list, the differences is tuple is immutable, or you can't reassign the value unlike list.

```py
n = tuple()
n = ("python", " is", 10, " the best", [1, 2, 3])

print(type(n))
# print <class 'tuple'>

print(n)
# print ('python', ' is', 10, ' the best', [1, 2, 3])

print(n[4][1])
# print 2

print(n[0] + n[1] + n[3])
# print "python is the best"

n[2] = 10
# print error "'tuple' object does not support item assignment"
```

##### Set
python data type to handle a set data, set data type can't have a duplicate value. Set data type cant be accesed using index like list or tupple, set data type usually justu used to check if the value is already present or not.

```py
x = [1,1,1,2,2,3]
n = set(x)

print(type(n))
# print <class 'set'>

print(n)
# print {1, 2, 3}

print(1 in n)
# print True
```

##### Dictionary
python data type to handle/store key-value map. in this type every value not accesed using index, but accesed using the key of value. the value can be different data types like tuple and list.

```py
n = dict()
n = {
    "key1" : "python",
    "key2" : " is the ",
    "key3" : " best",
}

print(type(n))
# print <class 'dict'>

print(n['key1'] + n['key2'] + n['key3'])
# print python is the  best

n['key1'] = {
    "key1_1": 1,
    "key1_2" : 2
}
print(n)
# print {'key1': {'key1_1': 1, 'key1_2': 2}, 'key2': ' is the ', 'key3': ' best'}
```

##### None
python data type to define null value

```py
<class 'NoneType'>
```


### Conclusion
There are so many data types in python, you can use it base on your needs.
