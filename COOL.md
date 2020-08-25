# Cool stuff I love about python

## Sorting

Sorting stuff is real easy on python.

```python
# sort on some attribute
monkeys.sort(key=lambda monkey: monkey.height)

# sort on more than one attribute
monkeys.sort(key=lambda monkey: (monkey.height, monkey.age))

# reverse sort
monkeys.sort(key=lambda monkey: (monkey.height, monkey.age), reverse=True)
```

## [reduce](https://docs.python.org/3.8/library/functools.html?highlight=reduce#functools.reduce)

Forget iterating - reduce is nice and clean.

## [defaultdict](https://docs.python.org/3.8/library/collections.html#collections.defaultdict)

This thing is so cool! Tell a dict what you want by default.