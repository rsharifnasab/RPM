---
title: "Beamer Presentation with Pandoc and Markdown"
subtitle: "A quick way to prepare slides"
author: "Amir Shabani - 9413088021"
institute: "University of Qom"
date: "Sunday, December 29, 2019"
theme: "metropolis"
linkcolor: blue
---

# Table of Contents

1. [What are Beamer, Pandoc, and Markdown?](#what-are-beamer-pandoc-and-markdown)
2. [The Philosophy of Markdown](#the-philosophy-of-markdown)
3. [Markdown Syntax](#markdown-syntax)
	1. [Typography](#typography)
	2. [Lists](#lists)
	3. [Links](#links)
	4. [Images](#images)
	5. [Code and Syntax Highlighting](#code-and-syntax-highlighting)
	6. [Tables](#tables)
	7. [Blockquotes](#blockquotes)
4. [Installing and running](#installing-and-running)
5. [References](#references)

# What are Beamer, Pandoc, and Markdown?
- **Beamer**

	Beamer is a LaTeX **document class** for creating presentation slides, with a wide range of templates and a set of features for making slideshow effects.

	It supports pdfLaTeX, LaTeX + dvips, LuaLaTeX and XeLaTeX. The name is taken from the German word "Beamer" as a pseudo-anglicism for "video projector".

# What are Beamer, Pandoc, and Markdown?
- **Pandoc**

	Pandoc is a free and open-source **document converter**, widely used as a writing tool (especially by scholars) and as a basis for publishing workflows. It was created by John MacFarlane, a philosophy professor at the University of California, Berkeley.

# What are Beamer, Pandoc, and Markdown?
- **Markdown**

	Markdown is a lightweight **markup language** with plain text formatting syntax. Its design allows it to be converted to many output formats, but the original tool by the same name only supports **HTML**. Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor.

# The Philosophy of Markdown

*Markdown* is intended to be as **easy-to-read** and **easy-to-write** as is feasible.

Readability, however, is emphasized above all else. A markdown-formatted document should be *publishable* as-is, as plain text, without looking like it's been marked up with tags or formatting instructions.

# Typography

`*italic* | _italic_` becomes *italic*

`**bold** | __bold__` becomes **bold**

`**_bold and italic_**` becomes **_bold and italic_**

`~~strikethrough~~` becomes ~~strikethrough~~

`**_~~mixed~~_**` becomes **_~~mixed~~_**

# Lists

`**Ordered List**`

`1. Item 1`

`2. Item 2`

`3. Item 3`

**Ordered List**

1. Item 1
2. Item 2
3. Item 3

# Lists

`**Unordered List**`

`- Item 1`

`- Item 2`

`- Item 3`

**Unordered List**

- Item 1
- Item 2
- Item 3

# Links

`<https://pandoc.org>` becomes <https://pandoc.org>

`[Pandoc](https://pandoc.org)` becomes [Pandoc](https://pandoc.org)

# Images

`![alternative text](address to image)`

![latex](latex.png)

# Code and Syntax Highlighting

~~~~~~
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
~~~~~~

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

# Code and Syntax Highlighting

~~~~~~
```python
string = "Python syntax highlighting"
print(string)
```
~~~~~~

```python
string = "Python syntax highlighting"
print(string)
```

# Tables

~~~~~~
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| col 1 is      | left-aligned  |    $1 |
~~~~~~

becomes

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| col 1 is      | left-aligned  |    $1 |

# Blockquotes

~~~~~~
> This is a block quote.
~~~~~~

&nbsp;

> Since the initial description of Markdown contained ambiguities and unanswered questions, the implementations that appeared over the years have subtle differences and many come with syntax extensions. 

# Installing and Running

1. Install `LaTex` and `Pandoc`
2. Run this command:

```sh
pandoc input.md -t beamer -o output.pdf 
```

# References

[**R Markdown** from RStudio](https://garrettgman.github.io/rmarkdown/authoring_pandoc_markdown.html)

[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
