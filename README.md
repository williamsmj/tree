# Tree class

Arbitrary tree class. Each tree has a root label two child nodes, which
should be other Trees or None.

```
>>> t = Tree(1, None, None)
[1, [2, [4, None, None], [5, None, None]], [3, None, [6, None, None]]]
>>> print t
[1, None, None]
>>> s = t.to_list()
>>> print s
[1, None, None]
>>> t = Tree(1, Tree(2, Tree(4), Tree(5)), Tree(3, None, Tree(6)))
>>> s = t.to_list()
>>> print s
[1, [2, [4, None, None], [5, None, None]], [3, None, [6, None, None]]]
>>> t2 = Tree.from_list(s)
>>> print t2
[1, [2, [4, None, None], [5, None, None]], [3, None, [6, None, None]]]
```

Mike Williams, 2015-06-09
