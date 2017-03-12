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
