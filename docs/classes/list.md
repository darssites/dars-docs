# List Class

This class is the dars wrapper for the `<[o/u]l><li></li></[o/u]l>` element of HTML.

### Syntax

```python
obj = List("spam-o", "bacon", "waffles", "...and many more!")
```

Produces:

```HTML
<ul>
  <li>spam-o</li>
  <li>bacon</li>
  <li>waffles</li>
  <li>...and many more!</li>
</ul>
```

You can provide any amount of strings as list items. To make a numbered list (ordered) you can do:

```python
obj = List("spam-o", "bacon", "waffles", "...and many more!", ordered=True)
```

Which produces:

```HTML
<ol>
  <li>spam-o</li>
  <li>bacon</li>
  <li>waffles</li>
  <li>...and many more!</li>
</ol>
```

You can also customize the text before the list item (the "bullet"). A list of types:

Unordered List Types:

1. disc (default)
2. circle
3. square
4. none

Ordered List Types:

1. 1 (number the items) (default)
2. A (uppercase alphabet the items)
3. a (lowercase alphabet the items)
4. I (uppercase roman numerals)
5. i (lowercase roman numerals)


```python
obj = List("spam-o", "bacon", "waffles", "...and many more!", type="square")
```

```HTML
<ul style="list-style-type:square">
  <li>spam-o</li>
  <li>bacon</li>
  <li>waffles</li>
  <li>...and many more!</li>
</ul>
```
