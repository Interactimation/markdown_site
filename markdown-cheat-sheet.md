# Markdown Cheat Sheet

Thanks for visiting [The Markdown Guide](https://www.markdownguide.org)!

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. It can’t cover every edge case, so if you need more information about any of these elements, refer to the reference guides for [basic syntax](https://www.markdownguide.org/basic-syntax/) and [extended syntax](https://www.markdownguide.org/extended-syntax/).

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

### Heading
```
# H1
## H2
### H3
#### H4
##### H5
```

# H1
## H2
### H3
#### H4
##### H5

### Linkable Custom Heading
(See link to this custom heading, bottom of page)

```
##### My Great Heading {#custom-id}
```

##### My Great Heading {#custom-id}


### Bold

```
**bold text**
```

**bold text**

### Italic

```
_italicized text_
```

_italicized text_

### Blockquote

```
> blockquote
```

> blockquote

### Ordered List

```
1. First item
2. Second item
3. Third item
```

1. First item
2. Second item
3. Third item

### Unordered List

```
* First item
* Second item
* Third item
    * Inset 1
        * Inset 2
```

* First item
* Second item
* Third item
    * Inset 1
        * Inset 2

### Code

Uses backticks like this
```
`code`
```

`code`

### Horizontal Rule

```
---
```

---

### Link

```
[Markdown Guide](https://www.markdownguide.org)
```

[Markdown Guide](https://www.markdownguide.org)

### Image

```
![alt text](https://www.markdownguide.org/assets/images/tux.png)
```

![alt text](https://www.markdownguide.org/assets/images/tux.png)

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |


### Fenced Code Block
Uses 3 backticks, new lines, 3 backticks (hard to draw here)

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote
(See footnote, bottom of page)

```
Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.
```

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

### Definition List

```
term
: definition
```

term
: definition

### Strikethrough

```
~~The world is flat.~~
```

~~The world is flat.~~

### Task List

```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

### Emoji

```
That is so funny! :joy:
```

That is so funny! :joy:

(See also [Copying and Pasting Emoji](https://www.markdownguide.org/extended-syntax/#copying-and-pasting-emoji))

### Highlight

```
I need to highlight these ==very important words==.
```

I need to highlight these ==very important words==.

### Subscript

```
H~2~O
```

H~2~O

### Superscript

```
X^2^
```

X^2^

### Heading ID

```
### My Great Heading {#custom-id}

[Return home](index.html)
```

[Link to "My Great Heading" Above](#custom-id)

