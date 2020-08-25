# Snippets of code to solve problems

## Joining together url parts

There's no built in library that handles it nicely, and I don't like doing a "{}/{}/{}".format() solution.

```python
# If you have a bunch of part sof a url, say:
a = ['http://www.something.com/', '/some/part/of/path', 'anotherthing/', 'thing.html']
# and you want to join it all together:
# (from https://stackoverflow.com/a/11326230/295741) 
def urljoin(*args):
    """
    Joins given arguments into an url. Trailing but not leading slashes are
    stripped for each argument.
    """

    return "/".join(map(lambda x: str(x).rstrip('/'), args))
```
