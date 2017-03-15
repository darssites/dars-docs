# Paragraph Class

This class is the dars wrapper for the `<p></p>` element in HTML. This is for displaying standard text, but also has optional markdown support.

### Syntax

Without Markdown:

```python
obj = Paragraph("paragraph text")
```

Produces:

```HTML
<p>paragraph text</p>
```

The Paragraph object also auto-parses markdown:

```python
obj = Paragraph("**formatted** _paragraph_ `text`")
```

Produces:

```HTML
<p><b>formatted</b> <i>paragraph</i> <code>text</code></p>
```

This would create way too many objects if you were to write this out with Bold, Code, and Italics objects, making this almost like a shorthand notation.
