# Heading Class

This class is the dars wrapper for the `<h1></h1>` element of HTML.

### Syntax

```python
obj = Heading("heading text", level=3)
```

Produces:

```HTML
<h3>heading text</h3>
```

You don't have to specify the level, with just the text it will set the level to 1.

```python
obj = Heading("heading text")
```

Produces:

```HTML
<h1>Heading text</h1>
```
