# Image Class

This class is the dars wrapper for the `<img src="" alt="" />` element of HTML.

### Syntax

```python
obj = Image("http://example.com/spam.jpg", "The Face of True Beauty")
```

The first argument is the image's source, and the second is the alternate description text if the image fails to load.

Produces:

```HTML
<img src="http://example.com/spam.jpg" alt="The Face of True Beauty" />
```

You can also specify the width and height to scale the image to. If only the width or the height is provided, it will scale the other to keep the original Aspect Ratio.

```python
obj = Image("http://example.com/spam.jpg", "The Face of True Beauty", height=2000)
```

```HTML
<img src="http://example.com/spam.jpg" alt="The Face of True Beauty" height="2000"/>
```
