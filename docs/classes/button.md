# Button Class

This class is the dars wrapper for the `<button></button>` element of HTML.

### Syntax

```python
obj = Button("spam-o", onclick="hello()")
```

Produces:

```HTML
<button onclick="hello()">spam-o</button>
```

You can also easily make the link go somewhere:

```python
obj = Button("spam-o", href="http://example.com/")
```

```HTML
<a href="http://example.com/">
  <button>spam-o</button>
</a>
```
