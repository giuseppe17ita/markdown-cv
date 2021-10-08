---
layout: default
---

Tired of using LaTeX to make your CV look pretty? Can't remember how to set margins in your TeX file? Refusing to compromise and "just use Word"?

[markdown-cv](http://elipapa.github.io/markdown-cv/) is a simple template to list all your accomplishments in a readable Markdown file. It uses CSS to style your text into a stylish web page. It can also be printed as PDF.

### what does that mean?

Write your CV like this...

<img src="img/mdown.png" style="width: 60%; -webkit-filter: drop-shadow(5px 5px 5px #222); filter: drop-shadow(5px 5px 5px #222);" >

and use [jekyll](https://jekyllrb.com/) or [github pages](https://pages.github.com/) to make it look like this..

<img src="img/output.png" style="width: 60%; -webkit-filter: drop-shadow(5px 5px 5px #222); filter: drop-shadow(5px 5px 5px #222);" >



## Usage

To start, simply [fork the markdown-cv repo](https://github.com/elipapa/markdown-cv)

![](https://help.github.com/assets/images/help/repository/fork_button.jpg)

and then [edit directly in github](https://help.github.com/articles/editing-files-in-your-repository/) the `index.md` file

![](https://help.github.com/assets/images/help/repository/edit-file-edit-button.png)

adding your skills, jobs and education.

![](https://help.github.com/assets/images/help/repository/edit-readme-light.png)

To transform your plain text CV into a beautiful looking HTML page and share it you then have two options:

### 1) Using Github Pages to publish it online

1. Delete the existing `gh-pages` branch from your fork. It will only contain this webpage. You can either use git or [the github web interface](https://help.github.com/articles/creating-and-deleting-branches-within-your-repository/#deleting-a-branch)
2. Create a new branch called `gh-pages` (which will then be a copy of master)
3. Head to *yourusername*.github.io/markdown-cv to see your CV live.

Any change you want to make to your CV from then on would have to be done on the `gh-pages` branch and will be immediately rendered by Github Pages.

### 2) Build it locally
1. [install jekyll](https://jekyllrb.com/docs/installation/) on your computer. `gem install jekyll` will do for most users.
2. Clone your fork on your computer
3. Type `jekyll serve` and you'll be able to see your CV on your local host (the default address is http://localhost:4000).
4. You can edit the `index.md` file and see changes live in your browser.

## How do I print the PDF?
Whether you used Github Pages or a local installation of Jekyll, to print a PDF just press *Print* in your browser. Print specific [CSS media queries](http://www.joshuawinn.com/css-print-media-query/) will take care of the styling.
