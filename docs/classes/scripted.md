# Scripted Class

This class is the dars wrapper for the `<[sup/sub]></[sup/sub]>` element of HTML. NOTE: This has nothing to do with JavaScript. That's the JScript class.

### Syntax

```python
obj = Scripted("spam-o")
```

Produces:

```HTML
<sup>spam-o</sup>
```

To do a subscript, you have to set the type argument:

```python
obj = Scripted("spam-o", type="subscript")
```

```HTML
<sub>spam-o</sub>
```
