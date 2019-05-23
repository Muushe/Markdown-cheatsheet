# Markdown Cheatsheet

**Markdown** is a lightweight markup language, which allows you to write using plaintext format, easy to write and read, and then convert it to a structurally valid XHTML or HTML. The language has many similarities with the conventions that already exist when you format plain text in emails.

1. [Headers](#headers)
2. [Paragraphs](#paragraphs)
3. [Line-break](#line-break)
4. [Emphasis](#emphasis)
5. [Horizontal-line](#horizontal-line)
6. [Lists](#lists)
    1. [Ordereds lists](#ordereds)
    2. [Unordereds lists](#unordereds)
    3. [Sub-lists](#sub-lists)
7. [Blockquotes](#blockquotes)
8. [Tables](#tables)
9. [Code](#code)
    1. [Pure code](#pure-code)
    2. [No Markdown](#no-markdown)
10. [Links](#links)
11. [Images](#images)
12. [Videos](#videos)
    1. [YouTube Videos](#youtube-videos)

------

## Headers

The symbol # is used to create headers. Each # used increases the header level from 1 to 6. See the code below:  
  
```
# Level 1
## Level 2
### Level 3
#### Level 4
##### Level 5
###### Level 6
```

This is what you get when you use this code:

# This is the level 1
## This is the level 2
### This is the level 3
#### This is the level 4
##### This is the level 5
###### This is the level 6

Otherwise, for the level 1 and 2 you can type the following code:  

```
Level 1
===
Level 2
---
```

See the code below:  

This is the level 1
===
This is the level 2
---

------

## Paragraphs

To create a new paragraph in Markdown, the only thing required is to insert a blank line. Follow the next syntax:

```
Paragraph 1

Paragraph 2
```

This is the result:

Paragraph 1

Paragraph 2

-----

## Line break

To jump to another line without creating a new paragraph you must insert two blank spaces at the end of the upper line. Follow the next syntax:


```
This is the first line (put here two blank spaces)  
and this is the second line
```

This is the result:

This is the first line  
and this is the second line

-----

## Emphasis

Markdown uses asterisks, *, and uderscores, _, to emphasis. To use you must use the symbol/s at the start and at the end of the word, phrase, paragraph or text.

| Markdown | Result |
| :---: | :---: |
| `*Italics*` | *Italics* |
| `_Italics_` | _Italics_ |
| `**Bold**` | **Bold** |
| `__Bold__` | __Bold__ |
| `***Italics and bold***` | ***Italics and bold*** |
| `___Italics and bold___` | ___Italics and bold___ |

---

You can scrath text, paragraphs, phrases or words using the symbol ~ at the start and end where you decide.

| Markdown | Result |
| :---: | :---: |
| `~~Strikethrough~~` | ~~Strikethrough~~ |

------

## Horizontal line

The horizontals lines are used to separate each section in a visual way. To generate, you must start a blank line with, at least, ***, ---, or ___.

```
Line 1
*****
Line 2
____
Line 3
***
```

This is the result:

Line 1
*****
Line 2
____
Line 3
***

-----

 ## Lists

1. [Ordereds lists](#Ordereds)
2. [Unordereds lists](#Unordereds)
3. [Sub-lists](#sub-lists)

There are two types of lists: ordereds and unordereds:

### Ordereds

For ordereds lists you must follow the next syntax: 'number' followed by a dot (1., 2., 3., ..., n.):

```
Ordered lists:  
1. First item
2. Second item
3. Third item
```

And this is the result:

Ordered lists:
1. First item
2. Second item
3. Third item

You can start an ordered list by the number of your choose:

9. Some item
10. Another item

### Unordereds

For unordered lists you can use the nexts symbols at the start of the items of the list: asterisks, *, plus, +, or minus, -.

```
Unordered lists
+ First item
+ Second item

- Third item
- Fourth item

* Fifth item
* Sixth item
```

And this is the result:  

Unordered lists
+ First item
+ Second item

- Third item
- Fourth item

* Fifth item
* Sixth item

### Sub-lists

To generate sub-lists, in ordered or unordered lists, the only thing is needed, is to add four spaces at the start of the sub-list or a space tab. You can create a sub-list from a sub-list using the same syntax.

```
Ordered lists
1. First item
    1. A item
    2. B item
        1. B.1 item
        2. B.2 item
2. Second item
```

This is the result:

1. First item
    1. A item
    2. B item
        1. B.1 item
        2. B.2 item
2. Second item

```
Unordered lists
+ First item
    + A item
    + B item
        + B.1 item
        + B.2 item
+ Second item
```

This is the result:

+ First item
    + A item
    + B item
        + B.1 item
        + B.2 item
+ Second item

-----

## Blockquotes

For blockquotes the only requirement is to start the text with the symbol >. Follow the next syntax:

```
>A statesman cannot create anything himself. He must wait and listen until he hears the steps of God sounding through events; then leap up and grasp the hem of His garment.
```

This is the result:

>A statesman cannot create anything himself. He must wait and listen until he hears the steps of God sounding through events; then leap up and grasp the hem of His garment.

If you need to create a blockquote text made with more than a paragraph, you must start each paragraph with the symbol >.

```
>A statesman cannot create anything himself. He must wait and listen until he hears the steps of God sounding through events; then leap up and grasp the hem of His garment.

>Not by speeches and votes of the majority, are the great questions of the time decided.
```

This is the result:

>A statesman cannot create anything himself. He must wait and listen until he hears the steps of God sounding through events; then leap up and grasp the hem of His garment.

>Not by speeches and votes of the majority, are the great questions of the time decided.

You can create a sub-blockquote from another quote introducing a new symbol > at the start of the sub-blockquote. Follow the next syntax:

```
>A statesman cannot create anything himself. He must wait and listen until he hears the steps of God sounding through events; then leap up and grasp the hem of His garment.  
>>--Otto von Bismarck

>Not by speeches and votes of the majority, are the great questions of the time decided.  
>>--Otto von Bismarck
```

This is the result:

>A statesman cannot create anything himself. He must wait and listen until he hears the steps of God sounding through events; then leap up and grasp the hem of His garment.  
>>--Otto von Bismarck

>Not by speeches and votes of the majority, are the great questions of the time decided.  
>>--Otto von Bismarck

-----

## Tables

To insert a table using Markdown, you must follow the next syntax creating a visual table:

```
| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Item 1   | Item 2   | Item 3   |
| Item 4   | Item 5   | Item 6   |
```

This is the result:

| Header 1 | Header 2 | Header 3 |
| -------- | -------- | -------- |
| Item 1   | Item 2   | Item 3   |
| Item 4   | Item 5   | Item 6   |

There must be at least 3 dashes, ---, separating each header cell. The outer pipes, |, are optional.
Colons, ., can be used in to align columns.

```
| Header 1     | Header 2 | Header 3      |
| :----------- | :------: | ------------: |
| Left-aligned | Centered | Right-aligned |
| Item 1       | Item 2   | Item 3        |
```

This is the result:

| Header 1     | Header 2 | Header 3      |
| :----------- | :------: | ------------: |
| Left-aligned | Centered | Right-aligned |
| Item 1       | Item 2   | Item 3        |

-----

## Code

If you want to generate a text without be interpreted by Markdown, you must start an upper blank line with ``` or ~~~ and end the text with also the same symbols.

~~~
```
This is a code without be interpreted by ***Markdown***
```
~~~

And this is the result:

~~~
This is a code without be interpreted by ***Markdown***
~~~

### Pure Code

In techinical documents, we will need to add sections where we show other languages codes, keyboards shortcuts, or other content that should not be trated as such.

The simplest way to write code in Markdown is to wrap the text between two single quotes, \`. See the next syntax:

```
`This is a code line`
```

This is the result:

`This is a code line`  

### No Markdown

If you need to scape specials characters in Markdown, like asterisks, \*, underscores, \_, etc. You need to start each of this symbols using the backlash, \\. This is the symbols you need to scape in case you need to write them in Markdown documents:

+ \_
+ \*
+ \`
+ \\
+ \( \)
+ \[ \]
+ \{ \} 
+ \#
+ \+
+ \-
+ \!

-----

## Links

To generate an inline link you must close the word or phrase with [ ] followed by the link between parenthesis, ( ).

| Markdown | Result |
| :---: | :---: |
| `[Sample text](www.google.com)` | [Sample text](www.google.com) |

We also can create reference links to create a more clean text instead of writing all the link to a web page.  

The reference link will not be showed and can be included in any part of the document, so you can organize better and in a cleaner way, collecting all our references in one place.See the next syntax:

```
[name of the link][name of the reference]

[name of the reference]: http://www.ourlink.com
```

This is the result:

[name of the link][name of the reference]

[name of the reference]: http://www.ourlink.com  

-----

## Images 

To insert an image with Markdown you must follow the same syntax for insert links. In this case, you must add the symbol !, exclamation mark, at the beginning and the link will be the image link.

```
![Alternative text](link to the image.jpg)
```

This is the result:

![Markdown](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png)

You can add an alternative title to be showed on mouse over the image. Put this alternative title at the end of the link quoted.

The alternative text will be showed if the image is not available or the link doesn't work.

```
![Alternative text](link to the image.jpg "alternative title")
```

This is the result (put your mouse over the image):

![Markdown](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png "alternative title")

Like reference links, you can fetch images from a reference link stablished in theany part of the document only calling it by the same way. You can stablish an alternative text in the reference link. See the following syntax:

```
![name of the image][img1]

[img1]: https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png "alternative text"
```

This is the result:

![name of the image][img1]

[img1]: https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png "alternative text"

-----

## Videos

Videos work like links, so you can follow the next syntax:

```
[name of the video link](http://www.our link.com)
```

This is the result:

[name of the video link](http://www.ourlink.com)

You can also establish them in any part of the document using the reference link method:

```
[name of the video link][linkvideo1]

[linkvideo1]: http://www.ourlink.com
```

This is the result:

[name of the video link][linkvideo1]

[linkvideo1]: http://www.ourlink.com

### YouTube Videos

You can link YouTube videos in Markdown using a miniature image of the video using the next syntax (the alternative text will be showed on mouse over the image):

```
[![alternative text if video does not work](http://img.youtube.com/vi/ID_VIDEO_HERE/0.jpg)](http://www.youtube.com/watch?v=ID_VIDEO_HERE "alternative text")
```

This is the result:

[![Markdown video](http://img.youtube.com/vi/hpAJMSS8pvs/0.jpg)](http://www.youtube.com/watch?v=hpAJMSS8pvs "markdown")