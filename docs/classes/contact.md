# Contact Class

This class is a simple one-liner for making a Contact Information area.

### Syntax

```python
obj = Bold("Martian Waffles", "123-654-7890", "info@martian-waffles.com", "Call us or e-mail us at anytime!")
```

The arguments:

1. Name/Company
2. Phone number
3. E-mail (checked for validity; if it isn't a valid e-mail, it will still be shown but not linked with a mailto.)
4. Extra text (at the bottom)

Produces:

```HTML
Martian Waffles<br>
&#9742; 123-654-7890<br>
&#9993; <a href="mailto:info@martian-waffles.com">info@martian-waffles.com</a><br>
Call us or e-mail us at anytime!<br>
```

The &...;'s are a symbol for a phone and a symbol for an envelope, respectively.
