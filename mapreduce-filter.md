### python内置的调出函数 map/reduce/filter用法



```python
# -*- coding: utf-8 -*-

from __future__ import unicode_literals

"""
    高阶函数map,reduce,filter
"""

import math


def format_names(s):
    return s.lower().title()


if __name__ == '__main__':
    # map
    print(map(format_names, ['adam', 'LISA', 'barT']))
    print(map(lambda s: s.lower().title(), ['adam', 'LISA', 'barT']))
    print(map(lambda x: x ** 2, xrange(1, 11)))

    # reduce
    print(reduce(lambda x, y: x + y, xrange(1, 11)))

    # filter
    print(filter(lambda x: x % 2 == 1, xrange(1, 11)))

    # 请利用filter()过滤出1~100中平方根是整数的数，即结果应该是：
    # [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
    #
    print(filter(lambda x: math.sqrt(x).is_integer(), xrange(1, 101)))

```



