---
layout: post
title: "Markdown & Jekyll Syntax Reference"
date: 2026-11-25
categories: [notes, reference]
tags: [markdown, jekyll, kramdown]
published: true
permalink: /etc/jekyll-syntax.md
---

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

---

## Text Formatting

Standard paragraph text. Leave an empty line between paragraphs.  
Add two spaces at the end of a line to force a line break.

- **Bold text** with double asterisks or __double underscores__
- *Italic text* with single asterisks or _single underscores_
- ***Bold and italic*** with triple asterisks
- ~~Strikethrough~~ with double tildes
- `Inline code` with single backticks
- Subscript and superscript: H<sub>2</sub>O and x<sup>2</sup>
- Keyboard shortcut: <kbd>Ctrl</kbd> + <kbd>S</kbd>

---

## Blockquotes

> First level quote.
>
> > Nested quote inside the first one.
> >
> > - List item inside a quote

---

## Lists

### Unordered List
- Item A
- Item B
  - Nested item B1
  - Nested item B2
- Item C

### Ordered List
1. Step one
2. Step two
   1. Sub-step one
   2. Sub-step two
3. Step three

### Task List
- [x] Done
- [ ] To do

### Definition List
Term 1
: Definition for term 1.

Term 2
: Definition for term 2.

---

## Links & Images

### Standard Links
- Inline link: vv
- Link with title: [Link label](https://example.com "Hover title")
- Auto-link: <https://example.com>
- Reference link: [Reference label][ref-id]

[ref-id]: https://example.com

### Internal Jekyll Links
- removed

### Images
- Image: ![Alt text](/assets/images/sample.png)
- Image with title: ![Alt text](/assets/images/sample.png "Hover title")
- Linked image: [![Alt text](/assets/images/thumb.png)](/assets/images/full.png)

---

## Code Blocks

### Standard Fenced Block
```python
def add(a, b):
    return a + b
```

### Liquid Highlight with Line Numbers
{% highlight bash linenos %}
echo "Line numbers enabled"
ls -la
{% endhighlight %}

### Escaping Liquid Syntax
{% raw %}
```liquid
{{ page.title }}
{% if page.published %}
  Visible
{% endif %}
```
{% endraw %}

---

## Tables

| Left | Center | Right |
| :--- | :---: | ---: |
| Cell 1 | Cell 2 | 10 |
| Cell 3 | Cell 4 | 200 |
| **Bold** | `Code` | *Italic* |

---

## Footnotes & Abbreviations

Sentence with a numbered footnote.[^1] Sentence with an inline footnote.^[Inline footnote text.]

[^1]: Bottom footnote text.

Hover over HTML or CSS to see their definitions.

*[HTML]: HyperText Markup Language
*[CSS]: Cascading Style Sheets

---

## Kramdown Attributes (IDs, Classes, Styles)

### Heading with Custom ID {#custom-id}
Link to the heading above: [Jump to section](#custom-id).

[Styled Link](https://example.com){: .btn target="_blank" rel="noopener"}

Paragraph with a custom class and inline style.
{: .notice style="border-left: 3px solid currentColor; padding-left: 12px;"}

![Resized Image](/assets/images/sample.png){: width="250px"}

---

## Auto Table of Contents

* TOC
{:toc}

---

## Liquid Variables & Conditions

- Title: {{ page.title }}
- Date: {{ page.date | date: "%Y-%m-%d" }}

{% if page.tags %}
Tags: {{ page.tags | join: ", " }}
{% endif %}

---

## Horizontal Rule & Raw HTML

---

<details>
  <summary>Collapsible section</summary>
  <p>Hidden content revealed on click.</p>
</details>
