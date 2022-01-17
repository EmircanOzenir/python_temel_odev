## Reverse Function

*input: [[1, 2], [3, 4], [5, 6, 7]]*

def reversy(x):
    b = []
    a = list(reversed(l))
    for i in a:
        b.append(list(reversed(i)))
    return b

print(list(reversy(l)))

*output: [[[7, 6, 5], [4, 3], [2, 1]]*