# Link Class

This class is the dars wrapper for the `<a></a>` element of HTML.

### Syntax

```python
obj = Link("Google", target="http://google.com/")
```

Produces:

```HTML
<a href="http://google.com">Google</a>
```


You can also really easily add an onclick javascript function to said link:

```python
obj = Link("Google", target="http://google.com/", function="coolKids()")
```

Produces:

```HTML
<a href="http://google.com" onclick="coolKids()">Google</a>
```


And if you don't specify a target, the link won't go anywhere:

```python
obj = Link("Google", function="coolKids()")
```

Produces:

```HTML
<a href="#" onclick="coolKids()">Google</a>
```
