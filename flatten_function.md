## Flatten function

*input = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]*

from typing import Iterable 

def flatten(a):
    for x in a:
        if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
            for sub_x in flatten(x):
                yield sub_x
        else:
            yield x

print(list(flatten(input)))

*output = [1, 'a', 'cat', 2, 3, 'dog', 4, 5]*