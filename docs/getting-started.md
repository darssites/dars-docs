## Getting Started

Welcome to dars! This tutorial will help you to get everything set up and running.

First download Python **3** from there website [here](http://python.org/). Then, open up your favorite shell and type: `python --version`. You should see `Python [version number]`. If you don't try reinstalling.

Then, head over to dars' [project page](http://github.com/darssites/dars) and click the green "Download" button, or, if you've got git, you can clone it from `http://github.com/darssites/dars`.

Now open the folder you got and edit the `user.py` file in your favorite editor (I use [atom](http://atom.io/)). This file is where you put all of your website's code, and should look a bit like this:

    #
    # The user's code.
    #

    from classes.Paragraph import Paragraph

    def code(page):

    text = Paragraph("Mooooooo!")
    page.append(text)

    page.addDefaultStyle()

    page.close()

Although the code from `def code(page):` to `page.addDefaultStyle()` changes a lot.

## Creating a simple site

To make the very basic site, open up our `user.py` file again in your favorite editor. dars comes with a bunch of classes, each representing a single or set of HTML tags. To create a Paragraph on your site, clear out all the code from `def code(page):` to `page.addDefaultStyle()` and replace it with:

    para = Paragraph("Hello World!")
    page.append(para)

Let's walk through this. The first line creates a Paragraph object, which takes one mandatory argument, the text. I've given it the text "Hello World!".

The second line adds the para object to our site, stored in the variable "page". **Note that the order things go on your page is the order you `append()` them in.**

### Testing

dars comes bundled with a teeny-tiny development-quality webserver **for testing your code**. It's really just not good enough for production, and dars produces normal HTML code so when you've done working dev magic, you can use something high-quality like [Apache](https://httpd.apache.org/).

But until then, you can use the one that dars gave you. First, generate your code by entering the following into your favorite shell (make sure you're in the "dars" directory you downloaded!):

```text
$ python dars.py --generate
```

It should give you some info, then exit. You can then start the server with:

```text
$ python dars.py --serve
```

Which sets everything up and gets your mini-server going. You can then visit <http://localhost/> to view your page!
