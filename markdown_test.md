---
title: "Testing markdown file"
date: "2000-01-20"
tags: ["Markdown-Test", "Blogs"]
excerpt: "A canonical Markdown file that demonstrates most common Markdown features: headings, math (inline & display), multi-line math, code blocks (many languages & fence styles), tables, lists, HTML blocks, diagrams, footnotes, task lists, and more."
---

# Markdown Test

This file demonstrates a wide variety of Markdown features to help test renderers.

## Headings

# H1
## H2
### H3
#### H4

## Inline elements

- **Bold text**
- *Italic text*
- ***Bold + Italic***
- `inline code` (use backticks)
- A link: [OpenAI](https://openai.com)
- Autolink: <https://example.com>

## Math

Inline math: Euler's identity is $e^{i\pi} + 1 = 0$.

Display math:

$$
\int_0^1 x^2 \, dx = \frac{1}{3}.
$$

Multiline math (aligned):

$$
\begin{aligned}
a &= b + c \\
  &= d + e + f \\
  &= 42
\end{aligned}
$$

## Code blocks

### Fenced code block (triple backticks, Python)
```python
def greet(name: str) -> str:
    """Return a greeting."""
    return f"Hello, {name}!"

print(greet('World'))
```

### Fenced code block (triple tildes, JavaScript)
~~~javascript
function add(a, b) {
  return a + b;
}
console.log(add(2, 3));
~~~

### Indented code block (4 spaces)
    # This is an indented code block
    echo "Hello from bash"

### Code block containing backticks (use longer fence)
````markdown
```not-a-real-language
This code block contains triple backticks inside it.
They are treated as literal content.
```
````

## Tables

Simple table:

| Name     | Type    | Notes              |
|:--------:|:-------:|-------------------:|
| Alpha    | String  | Left aligned text  |
| Beta     | Number  | Right aligned value|
| Gamma    | Bool    | Centered           |

Table with code and inline math:

| Expression | Value |
|------------|------:|
| `1 + 1`    | 2     |
| $\sqrt{2}$ | 1.414 |

## Lists

### Unordered
- Item 1
  - Subitem 1.1
  - Subitem 1.2
- Item 2

### Ordered
1. First
2. Second
   1. Second.A
   2. Second.B
3. Third

### Task list (GitHub-style)
- [x] Write tests
- [ ] Fix bugs
- [ ] Update docs

## Blockquotes

> This is a blockquote.
>
> > Nested blockquote with a list:
> > - Nested item A
> > - Nested item B

## HTML blocks (allowed in many Markdown flavors)

<div style="border:1px solid #ddd; padding:8px;">
  <strong>HTML block:</strong>
  This paragraph is raw HTML inside the Markdown file.
</div>

## Images

Inline image (linked):
![Placeholder image](https://via.placeholder.com/300x100.png?text=Markdown+Test)

Reference-style image:
![Ref-img][ref-img]

[ref-img]: https://via.placeholder.com/150 "Reference image"

## Footnotes

This sentence has a footnote.[^1]

[^1]: This is the footnote text. Footnotes may contain multiple lines.

## Definition list (informal)

Term 1
:   Definition for term 1.

Term 2
:   Another definition.

## HTML comments and raw HTML ignored by renderer

<!-- This is an HTML comment and should not be displayed. -->

## Special characters and escaping

Backslash escape: \*not italicized\*.

## Horizontal rules

---

## Mixed content example

> Code inside blockquote:
>
> ```bash
> echo "quoted code block"
> ```

## YAML front matter

The file begins with YAML front matter (see top of this document); many blog engines use this.

## End notes

- This file is intentionally verbose but compact.
- Use it to verify rendering of math, code, diagrams, tables, lists, footnotes, HTML blocks, and more.

