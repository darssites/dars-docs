# Rule, Stylesheet, and Tags Class

These classes are used for stylizing your page without using external stylesheets.

The Rule class represents an individual Rule.
The Stylesheet class is a group of Rules.
The Tags class helps you get HTML names of dars classes. (Header = h1)

To be frank, these classes are a bit clunky and I personally recommend using an external stylesheet instead.

### Syntax

To apply a color style to all headers on level 1:

```python
style = Stylesheet()
redRule = Rule("color", "red")
style.addRule(getHTMLTag("Header"), redRule.text)
```

Which gives:

```HTML
<style>
h1 {
  color: red;
}
</style>
```
