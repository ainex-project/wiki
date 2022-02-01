# Xenia Wiki Contribution Guide

<!--- TODO(halotroop2288) --->

## Prerequisites

- Knowledge and a copy of [Git](http://git-scm.com/)
- A [GitHub](https://github.com) account

### For testing:

You'll need MkDocs installed locally via Python to test your changes.
1. [Python 3.7+](https://www.python.org/downloads/)
  - Ensure Python gets added to your PATH

2. [MkDocs](https://www.mkdocs.org/), and [mkdocs-material](https://squidfunk.github.io/mkdocs-material/):
  - Run `python -m pip install mkdocs mkdocs-material` in your command prompt


## Instructions

-   If this is your first time contributing, be sure to read the entire page before you begin.

1.  Clone the [repo](https://github.com/xenia-project/wiki) and open it in your favorite editor.

2.  If your editor creates editor-specific files, add them to the `.gitignore` file.

3.  Write your article using Markdown. The many features of Markdown extensions can be found in the links below.
	If you'd like to use a Markdown extension not listed in [mkdocs.yml](https://github.com/xenia-project/wiki/blob/main/mkdocs.yml),
	you may add them to the list. You should ensure compatibility with other articles (so their layout does not
	accidentally change) before your changes are merged.
	- [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/extensions/arithmatex/)
	- [MkDocs Material Extensions](https://squidfunk.github.io/mkdocs-material/setup/extensions/python-markdown-extensions)

4.	[Test](#testing) and spell-check your article before it is merged.

5.  Submit a pull request to [the wiki repo](https://github.com/xenia-project/wiki/compare)


## Testing

To serve your copy of the website for testing:
1. Run `python -m mkdocs serve` in your command prompt

2. Open `127.0.0.1:8000` in your browser
   (be sure not to include `http(s)://` this will cause errors in the browser)

3. If you get any errors, read them carefully. The most common errors are broken links. You may have typed them wrong.
   - Keep in mind that `/` resolves to the `docs` folder. So, this page for example would be located at `/meta/contributing`
   - Embedded images must have extensions.
     Links to documents on this Wiki must have extensions.
     Articles on the wiki are do not need `.md` extensions (except in `mkdocs.yml`).


## Guidelines

1.	***Never*** attach files or links to content that is private to another party.<br/>
	This includes leaked documentation, piracy websites and other pirated content.
2.	If you attach a link to code on :github: GitHub in your article, make sure to get the *permalink.*<br/>
	Attaching links to branches (such as master/main) leads to dead or incorrect links down the road!


## Tips

-  [Emoji and Icons search and documentation](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#using-icons-in-templates)
