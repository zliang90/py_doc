### 返回一个函数对象



```python
# -*- coding: utf-8 -*-

from __future__ import unicode_literals

"""
    python中返回函数
"""


def calc_prod(lst=None):
    def f():
        return reduce(lambda x, y: x * y, lst)

    return f


if __name__ == '__main__':
    f = calc_prod(xrange(1, 5))
    print(f())

```



