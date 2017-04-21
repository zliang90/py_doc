### 高阶函数

---

&gt;&gt; 什么叫高阶函数？

高阶函数，就是能够将函数作为另一个函数的参数



```py
# -*- coding: utf-8 -*-

from __future__ import unicode_literals

"""
    高阶函数，将函数作为参数
"""


def add(x, y, f):
    return f(x) + f(y)


if __name__ == '__main__':
    print(add(-9, 10, abs))
```



