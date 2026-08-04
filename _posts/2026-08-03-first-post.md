---
layout: post
title: Markdown Syntax
date: 2026-08-03 12:52
description: Markdown is the preferred format for agents to read text files.
tags: technical
categories: technology
---
Markdown is the preferred format for agents and humans to read text files. This page  details how to the write a markdown file. 

## What is Markdown?
Markdown is a lightweight mark up language that you can use ot add formatting elements to plaintext documents. It was created in 2004. 

The approach is not to be a WYSIWYG editor. Instead the text is marked up with simple symbols such that the original text should be easy to read, but still allows for formatting to be applied. 

When markdown files are read they are processed or parsed, to take the markdown text and output it as HTML. At this point the text can be viewed in a web browser or combined with a stylesheet. 

## How does Markdown Processing Work
This is effectively a four part process: 

1. Create a Markdown file using a text editor or a dedicated markdown application. The file has a ```.md``` or ```.markdown``` extension. 
2. Open the markdown file in a markdown application. 
3. Use the markdown application to convert the markdown file to a HTML document. 
4. View the HTML file in a web browser or use the mark down application to convert it to another file format such as a PDF. 

## Why use markdown? 
Markdown is a fast and easy way to take notes, create content for a website and produce print-ready documents. 

It doesn't take long to learn the markdown syntax and once you know how to use it, you can write using markdown just about everywhere. Most people use markdown to create content for the web but it can genuinely be used for anything. 
***
### Web
Markdown was designed for the internet so it comes as no surprise that there are plenty of applications specifically designed for creating website content. [Jekyll](https://www.jekyllrb.com) is a common package for building static websites based off markdown files. Jekyll essentially converts markdown files in to pretty websites. The other advantage of Jekyll is that it is supported by github pages where this is published. 

There are other platforms that can be used for more complex sites, or CMS systems. But the beauty with this approach is the simplicity. 
***
### Notes
Markdown is an ideal language for taking notes. While Evernote and Onenote do not currently support markdown, most other platforms do. e.g. Obsidian and Notable. 
***
### LLM's
Many large language models use markdown as their default code for rendering files as it has a good balance of formatting and readability.
***
### Books
There are tools e.g. [Leanpub](https://leanpub.com/) that will convert markdown files in to electronic books in PDF, EPUB or mobi formal and you can upload them to kindle direct to publish the files in to direct books. It is also worth noting that tools such as Obsidian have this functionality built in. 
***
### Presentations
Although markdown may not be the preferred tool for creating presentations there are even tools for converting markdown files in to presentations. 

## Warnings
One of the most confusing aspects of markdown is that every application implements a slightly different version of markdown, and these variants or dialects are commonly referred to as flavours.

The original specifications for markdown can be found on [John Gruber's website](https://daringfireball.net/projects/markdown/).

# Let's get in to the syntax
If you need to display a special character you can use the escape character ```\```. Here is an example \#. 

### Headings
Use `#` symbols for headings, from H1 to H6.

```
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
There are some rules. You should always put a space after the ```#```. It is also best practice to have a blank link before and after the heading to ensure that the text renders correctly. 
***
### Paragraph's
The best practices when using paragraphs is just to place a new line, and keep lines left aligned. You should not use tabs for spaces as there are alternative ways to mark indentations. 
***
### Emphasis
```
*italic* or _italic_
**bold** or __bold__
***bold italic***
~~strikethrough~~
```
- *Italic*
- **Bold**
- ***Bold and italic***
- ~~Strike through~~-

***

### Lists
There are various types do lists these include: 
* Unordered lists
* Ordered lists
* Task lists

These will render differently depending on the renderer.

**Unordered list**
```
- Item one
- Item two
  - Nested item
* Alternative bullet style
```
Here is and example:
* Item 1
* Item 2
  * Indented item

**Ordered list**
```
1. First item
2. Second item
   1. Nested item
```
Here is an example: 
1. First item
2. Second item
   1. Nested item

**Task list**
```
- [x] Completed task
- [ ] Incomplete task
```
Here is an example: 
- [x] Completed task
- [ ] Incomplete task
***
### Links and Images
```
[Link text](https://example.com)
[Link with title](https://example.com "Title text")

![Alt text](image.png)
![Alt text](image.png "Image title")
```
***
### Hyperlinks

**Inline link**
```
[Visit Example](https://example.com)
```

**Reference-style link**
Useful for reusing the same link or keeping long URLs out of the text.
```
[Visit Example][1]

[1]: https://example.com "Optional title"
```

**Automatic / bare links**
```
<https://example.com>
<email@example.com>
```

**Linking to a file in the same repo (relative link)**
```
[See my Linux notes](Linux.md)
[Back to README](README.md)
```

**Linking to a heading/section (anchor link)**
Headings automatically get an id: lowercase, spaces become hyphens, punctuation removed.
```
[Jump to Tables section](#tables)
```

**Image as a link**
```
[![Alt text](image.png)](https://example.com)
```
***
### Code

**Inline code**
```
Use `code` like this.
```

**Code block with syntax highlighting**
````
```python
def hello():
    print("Hello, world!")
```
````
Here is an example of formatted code.:
```python
def hello():
    print("Hello, world!")
```

***
### Blockquotes
```
> This is a quote.
>
> > Nested quote.
```
> This is an example of a block quote. 

> > This is a nested quote.

Block quotes can be on multiple paragraphs. Here is an example. 

> This is a multi line block quote. 
>
> See it is continuing...

### Horizontal Rule
```
---
```

### Tables
```
| Column 1 | Column 2 | Column 3 |
|----------|:--------:|---------:|
| Left     | Center   | Right    |
| a        | b        | c        |
```
- `:---` left-aligns, `:---:` centers, `---:` right-aligns.

| Column 1 | Column 2 | Column 3 |
|----------|:--------:|---------:|
| Left     | Center   | Right    |
| a        | b        | c        |

### Line Breaks
- End a line with two spaces, or a backslash `\`, to force a line break without starting a new paragraph.

### Escaping Characters
```
\* Not a bullet point
\# Not a heading
```

### Footnotes
```
Here is a statement with a footnote.[^1]

[^1]: This is the footnote text.
```

### HTML in Markdown
Most renderers allow raw HTML for things Markdown can't do natively:
```html
<details>
<summary>Click to expand</summary>

Hidden content here.

</details>
```


