---
title: "Useful Markdown Syntax"
date: 2020-06-08T08:06:25+06:00
description: Useful Markdown Syntax
menu:
  sidebar:
    name: Useful Markdown Syntax
    identifier: useful markdown syntax
    weight: 80
    hero: background-2.jpg
math: true
---

Markdown is a lightweight markup language used to make webpages easier on the eye and simpler to read. Markdown is built into many applications such as documentation systems, note-taking applications and content management systems. 

The below examples showcase some of the basic Markdown syntax elements, however, there are more features and extensions available depending on the Markdown implementation or specific application you're using. Markdown's popularity comes from its simplicity and ease of use, making it a preferred choice for creating content that can be easily shared and displayed on the web. For further information on markdown and a more robust syntax list please review https://www.markdownguide.org/

# Markdown Syntax Rendering

## Headings

Headings and subheadings may be used to provide an outline of how the page in structured by breaking up web pages into sections and introducing the reader to a new topic. With H1 being the largest and H6 the smallest headings available:

```
# H1
## H2
### H3
#### H4
##### H5
###### H6
```  

All headings in this article are between H1 and H3 size and the topics these are used for may be observed in the Table of Contents on the right hand side.

## Emphasis

Emphasis is important to assist readers to garner important points in text. Basic Markdown allows for the use of italic, bold, italic and bold, or strikethrough.

### Italic 

Italics are usually used for titles and names in writing such as books, movies, vehicles or if the word may be in an alternate language or a new word or concept. For use of *italics* in markdown:

```
*Italic text*
```

### Bold 

For strong emphasis on keywords you may use **bold** on your words:
```
**Bold text**
```
<br/>

On occasion you may require the use of both ***italic and bold***:

```
***Italic and bold***
```


### Strikethrough

The use of strikethrough can be a fun way to emphasize a change of idea or opinion. Such as; ~~You don't need to backup your storage.~~ Everyone needs to backup their storage:

```
~~You don't need to backup your storage.~~ Everyone needs to backup their storage.
```  

## Paragraph

Markdown renders paragraphs and line breaks as you would normally write them, there is no need for any special characters. However, traditional html paragraph code and line breaks may be used if required, however, not all applications will render these the same way. 

## Blockquotes

A blockquote represents content that is quoted from another source. Markdown has systax for blockquotes with and without citation. When using citation for your sources these will be contained within the footer (see bottom of page).

#### Blockquote without Citation

> It always seems impossible until it's done.
> **Note:** *Markdown syntax* may be used within a blockquote for example to achieve *italic* or **bold** emphasis.

```
> It always seems impossible until it's done.
> **Note:** *Markdown syntax* may be used within a blockquote for example to achieve *italic* or **bold** emphasis.
```

#### Blockquote with Citation

> It always seems impossible until it's done.</p>
> — <cite>Nelson Mandela[^1]</cite>


```
> It always seems impossible until it's done.</p>
> — <cite>Nelson Mandela[^1]</cite>
```

## Footnotes

A footnote contains additional information printed at the bottom of the page for reference.

**Example:** Here's a small footnote,[^1] and here's a lengthier one containing a full paragraph with some code.[^bignote]

[^1]: Footnote one 

[^bignote]: A footnote with paragraphs and code.

    Indent your paragraphs to have them included in the footnote.

    `{ add some code }`

    See bottom of the page for the full output of footnotes
```
Here's a small footnote,[^1] and here's a lengthier one containing a full paragraph with some code.[^bignote]

[^1]: Footnote one 

[^bignote]: A footnote with paragraphs and code.

    Indent your paragraphs to have them included in the footnote.

    `{ add some code }`

    See bottom of the page for the full output of footnotes
```

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Markdown doesn't support tables as part of its core capability, however, many applications support them.

   | Name  | Age |
   | ----- | --- |
   | Rosa  | 25  |
   | Ben   | 32  |  

<br/>

```
   | Name  | Age |
   | ----- | --- |
   | Rosa  | 25  |
   | Ben   | 32  |  
```

## List Types

Lists provide the reader with a neat and ordered overview or set of instructions. Markdown supports multiple ways to create lists.

#### Ordered List

1. Milk
2. Bread
3. Flour

```
1. Milk
2. Bread
3. Flour
```

#### Unordered List

* Ordered Lists 
* Unordered Lists 
* Nested Lists 
* Task Lists

```
* Ordered Lists 
* Unordered Lists 
* Nested Lists 
* Task Lists 
```

#### Nested List

* Pantry
  * Pasta
  * Tomato Sauce
  * Cereal
* Fish
  * Cod
  * Hake
  
```
* Pantry
  * Pasta
  * Tomato Sauce
  * Cereal
* Fish
  * Cod
  * Hake
```

### Task Lists

- [x] Sunblock
- [ ] Towel
- [ ] Beachwear

```
- [x] Sunblock
- [ ] Towel
- [ ] Beachwear
```

## Code Words

To denote a word or a phrase as code, enclose the word(s) in backticks. **Example:** At the command prompt, enter `vi newtextfile.txt`.

```
At the command prompt, enter `vi newtextfile.txt`.
```

## Code Blocks

Code blocks can be extremely useful when writing instructions especially in relation to computing and software. There are multiple ways to introduce code blocks with markdown.

#### Code Block using Backticks

The easiest way to use a code block is to use three backticks (`) at the beginning of the code and three backticks at the end of the code.

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Paragraph</p>
</body>
</html>
```

#### Code Block using Four Indented Spaces

You may also use four indented spaces for a block of code.

```
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Paragraph</p>
    </body>
    </html>
```    

#### Code Block Inside of a List

1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>This is the Title</title>
          </head>

3. Update the title to match the name of your website.

```
1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>This is the Title</title>
          </head>

3. Update the title to match the name of your website.
```

## Other Elements

### Subscript

H<sub>2</sub>O

```
H<sub>2</sub>O
```

### Superscript 

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

```
X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>
```

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.


## Images

![Alt text](background-2.jpg)

```
![Alt text](background-2.jpg)
```

### Image inside of a list

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.

```
1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.
```

## Links

[Link text](https://www.example.com)

```
[Link text](https://www.example.com)
```

## URLs and Email Addresses

To quickly turn a URL or email address into a link, enclose it in angle brackets.

<https://www.markdownguide.org>  
<fake@example.com>

```
<https://www.markdownguide.org>
<fake@example.com>
```

## Horizontal rule

---

```
---
```

---

## Math Rendering

{{< math.inline >}}
<p>
Inline math: \(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\)
</p>
{{</ math.inline >}}

Block math:
$$
 \varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } } 
$$

