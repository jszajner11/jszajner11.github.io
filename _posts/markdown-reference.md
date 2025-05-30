---
layout: default
title: Markdown Reference Guide
description: A comprehensive reference for all Markdown syntax and GitHub Flavored Markdown features
date: 2025-05-30
permalink: /markdown-reference/
---
# Markdown Reference Guide 🚀

A comprehensive reference for all Markdown syntax and GitHub Flavored Markdown features.

---

## Table of Contents

- [Headers](#headers)
- [Text Formatting](#text-formatting)  
- [Lists](#lists)
- [Links](#links)
- [Images](#images)
- [Code](#code)
- [Tables](#tables)
- [Blockquotes](#blockquotes)
- [Horizontal Rules](#horizontal-rules)
- [Task Lists](#task-lists)
- [Strikethrough](#strikethrough)
- [Emoji](#emoji)
- [Line Breaks](#line-breaks)
- [Escaping Characters](#escaping-characters)
- [HTML in Markdown](#html-in-markdown)
- [GitHub Specific Features](#github-specific-features)

---

## Headers

```markdown
# H1 Header
## H2 Header  
### H3 Header
#### H4 Header
##### H5 Header
###### H6 Header
```

**Result:**

# H1 Header
## H2 Header  
### H3 Header
#### H4 Header
##### H5 Header
###### H6 Header

### Alternative Header Syntax

```markdown
Header 1
========

Header 2
--------
```

**Result:**

Header 1
========

Header 2
--------

---

## Text Formatting

### Basic Formatting

```markdown
**Bold text**
__Bold text alternative__

*Italic text*
_Italic text alternative_

***Bold and italic***
___Bold and italic alternative___

~~Strikethrough~~

==Highlighted text== (GitHub Pages specific)
```

**Result:**

**Bold text**  
__Bold text alternative__

*Italic text*  
_Italic text alternative_

***Bold and italic***  
___Bold and italic alternative___

~~Strikethrough~~

### Subscript and Superscript

```markdown
H~2~O (subscript)
X^2^ (superscript)
```

**Result:**

H~2~O (subscript)  
X^2^ (superscript)

---

## Lists

### Unordered Lists

```markdown
- Item 1
- Item 2
  - Nested item 2.1
  - Nested item 2.2
    - Deep nested item
- Item 3

* Alternative bullet
+ Another alternative
```

**Result:**

- Item 1
- Item 2
  - Nested item 2.1
  - Nested item 2.2
    - Deep nested item
- Item 3

* Alternative bullet
+ Another alternative

### Ordered Lists

```markdown
1. First item
2. Second item
   1. Nested numbered item
   2. Another nested item
3. Third item

1. You can use 1. for all items
1. Markdown will auto-number
1. Like this
```

**Result:**

1. First item
2. Second item
   1. Nested numbered item
   2. Another nested item
3. Third item

1. You can use 1. for all items
1. Markdown will auto-number
1. Like this

---

## Links

### Basic Links

```markdown
[Link text](https://example.com)
[Link with title](https://example.com "Title text")

<https://example.com>
<email@example.com>
```

**Result:**

[Link text](https://example.com)  
[Link with title](https://example.com "Title text")

<https://example.com>  
<email@example.com>

### Reference Links

```markdown
[Reference link][1]
[Another reference][link-ref]

[1]: https://example.com
[link-ref]: https://example.com "Optional title"
```

**Result:**

[Reference link][1]  
[Another reference][link-ref]

[1]: https://example.com
[link-ref]: https://example.com "Optional title"

### Internal Links

```markdown
[Link to header](#headers)
[Link to text formatting](#text-formatting)
```

**Result:**

[Link to header](#headers)  
[Link to text formatting](#text-formatting)

---

## Images

### Basic Images

```markdown
![Alt text](https://via.placeholder.com/150x100.png)
![Alt text with title](https://via.placeholder.com/150x100.png "Image title")
```

**Result:**

![Alt text](https://via.placeholder.com/150x100.png)  
![Alt text with title](https://via.placeholder.com/150x100.png "Image title")

### Reference Images

```markdown
![Reference image][img-ref]

[img-ref]: https://via.placeholder.com/150x100.png "Reference image"
```

**Result:**

![Reference image][img-ref]

[img-ref]: https://via.placeholder.com/150x100.png "Reference image"

### Linked Images

```markdown
[![Image link](https://via.placeholder.com/100x100.png)](https://example.com)
```

**Result:**

[![Image link](https://via.placeholder.com/100x100.png)](https://example.com)

---

## Code

### Inline Code

```markdown
Use `inline code` for short snippets.
```

**Result:**

Use `inline code` for short snippets.

### Code Blocks

#### Fenced Code Blocks

```markdown
```
Basic code block
```

```javascript
// JavaScript with syntax highlighting
function hello() {
    console.log("Hello, World!");
}
```

```python
# Python example
def greet(name):
    return f"Hello, {name}!"
```

```css
/* CSS example */
.container {
    max-width: 1200px;
    margin: 0 auto;
}
```
```

**Result:**

```
Basic code block
```

```javascript
// JavaScript with syntax highlighting
function hello() {
    console.log("Hello, World!");
}
```

```python
# Python example
def greet(name):
    return f"Hello, {name}!"
```

```css
/* CSS example */
.container {
    max-width: 1200px;
    margin: 0 auto;
}
```

#### Indented Code Blocks

```markdown
    // Indented with 4 spaces
    function example() {
        return true;
    }
```

**Result:**

    // Indented with 4 spaces
    function example() {
        return true;
    }

---

## Tables

### Basic Table

```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data     | More     |
| Row 2    | Data     | Data     |
```

**Result:**

| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Row 1    | Data     | More     |
| Row 2    | Data     | Data     |

### Aligned Tables

```markdown
| Left Aligned | Center Aligned | Right Aligned |
|:-------------|:--------------:|--------------:|
| Left         | Center         | Right         |
| Text         | Text           | Text          |
```

**Result:**

| Left Aligned | Center Aligned | Right Aligned |
|:-------------|:--------------:|--------------:|
| Left         | Center         | Right         |
| Text         | Text           | Text          |

### Complex Table

```markdown
| Feature | Supported | Notes |
|---------|:---------:|-------|
| **Bold** | ✅ | Works in tables |
| *Italic* | ✅ | Also works |
| `Code` | ✅ | Inline code too |
| [Links](https://example.com) | ✅ | External links |
```

**Result:**

| Feature | Supported | Notes |
|---------|:---------:|-------|
| **Bold** | ✅ | Works in tables |
| *Italic* | ✅ | Also works |
| `Code` | ✅ | Inline code too |
| [Links](https://example.com) | ✅ | External links |

---

## Blockquotes

### Basic Blockquotes

```markdown
> This is a blockquote.
> It can span multiple lines.

> You can also
> break it like this.
```

**Result:**

> This is a blockquote.
> It can span multiple lines.

> You can also
> break it like this.

### Nested Blockquotes

```markdown
> Outer quote
>> Nested quote
>>> Deeply nested quote

> Back to outer level
```

**Result:**

> Outer quote
>> Nested quote
>>> Deeply nested quote

> Back to outer level

### Blockquotes with Other Elements

```markdown
> ## Header in blockquote
> 
> - List item 1
> - List item 2
> 
> **Bold text** and *italic text* work here.
> 
> ```javascript
> // Even code blocks!
> console.log("Hello from blockquote");
> ```
```

**Result:**

> ## Header in blockquote
> 
> - List item 1
> - List item 2
> 
> **Bold text** and *italic text* work here.
> 
> ```javascript
> // Even code blocks!
> console.log("Hello from blockquote");
> ```

---

## Horizontal Rules

```markdown
---

***

___

- - -

* * *
```

**Result:**

---

***

___

- - -

* * *

---

## Task Lists

```markdown
- [x] Completed task
- [x] Another completed task
- [ ] Incomplete task
- [ ] Another incomplete task
  - [x] Nested completed task
  - [ ] Nested incomplete task
```

**Result:**

- [x] Completed task
- [x] Another completed task
- [ ] Incomplete task
- [ ] Another incomplete task
  - [x] Nested completed task
  - [ ] Nested incomplete task

---

## Strikethrough

```markdown
~~This text is struck through~~
~~You can strike through~~ normal text ~~multiple times~~.
```

**Result:**

~~This text is struck through~~  
~~You can strike through~~ normal text ~~multiple times~~.

---

## Emoji

### GitHub Emoji Shortcodes

```markdown
:smile: :heart: :thumbsup: :rocket: :octocat:
:+1: :-1: :100: :fire: :sparkles:
```

**Result:**

:smile: :heart: :thumbsup: :rocket: :octocat:  
:+1: :-1: :100: :fire: :sparkles:

### Unicode Emoji

```markdown
😀 😍 👍 🚀 🔥 ✨ 🎉 💯
```

**Result:**

😀 😍 👍 🚀 🔥 ✨ 🎉 💯

---

## Line Breaks

### Two Spaces Method

```markdown
Line one  
Line two (note the two spaces after "one")
```

**Result:**

Line one  
Line two (note the two spaces after "one")

### Backslash Method

```markdown
Line one\
Line two (using backslash)
```

**Result:**

Line one\
Line two (using backslash)

### HTML Break

```markdown
Line one<br>
Line two (using HTML)
```

**Result:**

Line one<br>
Line two (using HTML)

---

## Escaping Characters

```markdown
\*This is not italic\*
\**This is not bold\**
\# This is not a header
\[This is not a link\]
\`This is not code\`
```

**Result:**

\*This is not italic\*  
\**This is not bold\**  
\# This is not a header  
\[This is not a link\]  
\`This is not code\`

### Characters that can be escaped:

```
\ ` * _ { } [ ] ( ) # + - . !
```

---

## HTML in Markdown

You can use HTML tags directly in Markdown:

```html
<details>
<summary>Click to expand</summary>

This content is hidden by default.

You can put **Markdown** inside HTML tags.

</details>

<kbd>Ctrl</kbd> + <kbd>C</kbd>

<mark>Highlighted text</mark>

<sub>Subscript</sub> and <sup>Superscript</sup>
```

**Result:**

<details>
<summary>Click to expand</summary>

This content is hidden by default.

You can put **Markdown** inside HTML tags.

</details>

<kbd>Ctrl</kbd> + <kbd>C</kbd>

<mark>Highlighted text</mark>

<sub>Subscript</sub> and <sup>Superscript</sup>

---

## GitHub Specific Features

### Mentioning Users and Teams

```markdown
@username
@organization/team-name
```

### Referencing Issues and Pull Requests

```markdown
#123
organization/repository#123
GH-123
```

### SHA References

```markdown
commit 16c999e8c71134401a78d4d46435517b2271d6ac
```

### Automatic Linking

GitHub automatically converts URLs to links:
```
https://github.com
```

### Math Expressions (GitHub)

```markdown
$\sqrt{3x-1}+(1+x)^2$

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$
```

### Diagrams with Mermaid

````markdown
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

### Footnotes

```markdown
Here's a sentence with a footnote[^1].

[^1]: This is the footnote.
```

**Result:**

Here's a sentence with a footnote[^1].

[^1]: This is the footnote.

---

## Tips and Best Practices

### 1. Consistent Spacing
- Always add blank lines before and after headers
- Add blank lines before and after code blocks
- Use consistent indentation for nested lists

### 2. Link Organization
- Use reference links for repeated URLs
- Keep reference definitions at the bottom of the document

### 3. Table Formatting
- Align table headers for better readability in source
- Use shorter column names when possible

### 4. Code Blocks
- Always specify language for syntax highlighting
- Use descriptive variable names in examples

### 5. Documentation Structure
- Use a logical hierarchy of headers
- Include a table of contents for long documents
- Add horizontal rules to separate major sections

---

## Quick Reference Cheat Sheet

| Element | Syntax |
|---------|--------|
| Header | `# H1` `## H2` `### H3` |
| Bold | `**text**` or `__text__` |
| Italic | `*text*` or `_text_` |
| Code | `` `code` `` |
| Link | `[text](url)` |
| Image | `![alt](url)` |
| List | `- item` or `1. item` |
| Quote | `> quote` |
| Rule | `---` |
| Table | `\| cell \| cell \|` |
| Strikethrough | `~~text~~` |
| Task List | `- [x] done` `- [ ] todo` |

---

*Last updated: May 2025*

**Happy Markdown writing! 🚀**
