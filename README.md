ListPlus.py
========

## Overview

ListPlus.py is Scala like list class library for Python.

### Requirements
Python >= 3.3.2

### Usage

```python
>>> from listplus import List
>>> l = List(range(1, 5))
>>> l.head
1
```

### Methods

#### get(index)

```python
>>> l = List(range(1, 5))
>>> l.get(1)
2
```

#### swap(index, moveto)

```python
>>> l = List(['a', 'b', 'c'])
>>> l.swap(0, 2)
>>> print(l)
['c', 'b', 'a']
 ```

#### forall(expr)

```python
>>> l = List(range(1, 5))
>>> l.forall('_ > 0')
True
>>> l.forall('_ > 3')
False
```

#### contains(value)

```python
>>> l = List([1, 2, 3])
>>> l.contains(2)
True
>>> l.contains(5)
False
>>> l = List(['a', 'b', 'c'])
>>> l.contains('b')
True
>>> l.contains('f')
False
```

#### apply(index)

```python
>>> l = List([1, 2, 3])
>>> l.apply(2)
3
>>> l.apply(3) is None
True
```

#### take(count)

```python
>>> l = List([1, 2, 3])
>>> l.take(2)
[1, 2]
>>> l.take(3)
[1, 2, 3]
>>> l.take(4)
[1, 2, 3]
```

#### takeRight(count)

```python
>>> l = List([1, 2, 3])
>>> l.takeRight(2)
[2, 3]
>>> l.takeRight(3)
[1, 2, 3]
>>> l.takeRight(4)
[1, 2, 3]
```

### drop(count)

```python
>>> l = List([1, 2, 3, 4, 5])
>>> l.drop(2)
[3, 4, 5]
```

### dropRight(count)

```python
>>> l = List([1, 2, 3, 4, 5])
>>> l.dropRight(2)
[1, 2, 3]
>>> l = List(['a', 'b', 'c', 'd', 'e'])
>>> l.dropRight(3)
['a', 'b']
```

### Properties

#### head
```python
>>> l = List(range(1, 5))
>>> l.head
1
```

#### tail
```python
>>> l = List(range(1, 5))
>>> l.tail
[2, 3, 4]
```

#### init
```python
>>> l = List(range(1, 5))
>>> l.init
[1, 2, 3]
```

#### last
```python
>>> l = List(range(1, 5))
>>> l.last
4
```

#### length
```python
>>> l = List([1, 2, 3, 4, 5])
>>> print(l.length)
5
```

#### min
```python
>>> l = List([1, 2, 3, 4, 5])
>>> print(l.min)
1
```

#### max
```python
>>> l = List([1, 2, 3, 4, 5])
>>> print(l.max)
5
```

#### size
```python
>>> l = List([1, 2, 3, 4, 5])
>>> print(l.size)
5
```

#### isEmpty

```python
>>> l = List()
>>> print(l.isEmpty)
True
>>> l = List([])
>>> print(l.isEmpty)
True
>>> l = List([1])
>>> print(l.isEmpty)
False
```

#### sorted
```python
>>> l = List([5, 4, 3, 2, 1])
>>> print(l.sorted)
[1, 2, 3, 4, 5]
```

#### reverse
```python
>>> l = List([5, 4, 3, 2, 1])
>>> print(l.reverse)
[1, 2, 3, 4, 5]
```

#### sum
```python
>>> l = List([1,2,3])
>>> l.sum
6
>>> l = List([])
>>> l.sum
0
```

#### product
```python
>>> l = List([1,2,3])
>>> l.product
9
>>> l = List([])
>>> l.product
0
```


