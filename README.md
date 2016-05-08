#### pkmaspython
#####8 metaclasses
Below two are completely identical
```
class C(object):
    test = 'test'
```
and
```
C = type('C', (object,), dict(test='test'))
```

AND
```
class C(object):
    pass
```
same as 
```
class C(object, metaclass=type):
    pass
```

