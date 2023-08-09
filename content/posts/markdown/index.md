---
title: "Using Markdown"
date: 2023-05-05T10:56:25+06:00
description: Using Markdown
menu:
  sidebar:
    name: Using Markdown
    identifier: using markdown
    weight: 80
# hero: background-2.jpg
# math: true
---

Markdown is a lightweight markup language used to make webpages easier on on the eye when displayed and simplier to read in plain text format. Markdown is widely popular due to its ease of use and its acceptance by many applications such as documentation systems, note-taking applications and messaging systems.

The below examples showcase some of the basic Markdown syntax elements, however, there are more features and Markdown flavours available depending on the Markdown implementation or specific application you're using. For further information on markdown and a more robust syntax list please review https://www.markdownguide.org/

# Markdown Syntax Rendering

## Headings

Headings and subheadings may be used to provide an outline of how the page is structured by breaking up web pages into sections and introducing the reader to a new topic. H1 is the largest heading available while H6 is the smallest:

```
# H1
## H2
### H3
#### H4
##### H5
###### H6
```  
</br>

All headings in this article are between H1 and H4 in size and the topics these are used for may be observed in the Table of Contents on the right hand side of this page.

## Emphasis

Emphasis is an important asset to assist readers in identifing important points in text. Basic Markdown allows for the use of italic, bold, italic and bold, or strikethrough.

### Italic 

Italics are generally used for titles and names in writing such as books, movies and vessels or for a new word or concept. For use of *italics* in markdown see below:

```
*Italic text*
```

### Bold 

To strongly emphasize keywords the use of **bold** can be very effective:

```
**Bold text**
```
</br>

To use both ***italic and bold***, begin and end the word(s) with three asterisks:

```
***Italic and bold***
```

### Strikethrough

The use of strikethrough can be a fun way to emphasize a change of idea or opinion. Such as; ~~You don't need to backup your storage.~~ Everyone needs to backup their storage:

```
~~You don't need to backup your storage.~~ Everyone needs to backup their storage.
```  

## Paragraph

Markdown renders paragraphs and line breaks as you would normally write them, there is no need for any special characters. However, traditional html paragraph code and line breaks may be used if required although caution should be taken when used as not all applications will render this code in the the same manner.

## Blockquotes

A blockquote represents content that is quoted from another source. Markdown has systax for blockquotes with and without citation. When using citation for your sources these will be contained within the footer.

#### Blockquote without Citation

A blockquote without citation may be achieved by beginning the line with the greater than symbol:

> It always seems impossible until it's done.
> **Note:** *Markdown syntax* may be used within a blockquote for example to achieve *italic* or **bold** emphasis.

```
> It always seems impossible until it's done.
> **Note:** *Markdown syntax* may be used within a blockquote for example to achieve *italic* or **bold** emphasis.
```

#### Blockquote with Citation

Creating a blockquote with citation is similar to the above with some added code: 

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

[^1]: The above quote is a small footnote

## Tables

Markdown does not support tables as part of its core capabilities, however, many applications support a basic table such as:

   | Name  | Age |
   | ----- | --- |
   | Rosa  | 22  |
   | Ben   | 34  |  

<br/>

Creating a table can be as simple as the below formating: 

```
   | Name  | Age |
   | ----- | --- |
   | Rosa  | 22  |
   | Ben   | 34  |  
```

## List Types

Lists provide the reader with a precise and ordered overview and thankfully Markdown supports multiple ways to create lists.

#### Ordered List

Example ordered list:

1. Open the command line
2. Navigate to the root directory 
3. Make a new directory 

```
1. Open the command line
2. Navigate to the root directory 
3. Make a new directory 
```

#### Unordered List

Example undordered list:

* Flour
* Milk 
* Bread 
* Olive Oil

```
* Flour
* Milk 
* Bread 
* Olive Oil
```

#### Nested List

Example nested list:

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

#### Task Lists

Example task list:

- [x] Sunblock
- [ ] Towel
- [ ] Beachwear

```
- [x] Sunblock
- [ ] Towel
- [ ] Beachwear
```

#### Image inside of a list

When providing instructions it may be helpful to place an image inside of a list, for example: 

1. To open the command prompt on windows press "Windows + R". 
2. In the run program window type "cmd" and press "Enter" to launch the command prompt

    ![Windows Command Line](cmd.png)

3. Enjoy exploring the command line!

Syntax:

```
1. To open the command prompt on windows press "Windows + R". 
2. In the run program window type "cmd" and press "Enter" to launch the command prompt

    ![Windows Command Line](cmd.png)

3. Enjoy exploring the command line!
```

## Code Words

To denote a word or a phrase as code, enclose the word(s) in backticks. **For example:** At the command prompt, enter `vi newtextfile.txt`.

```
At the command prompt, enter `vi newtextfile.txt`.
```

## Code Blocks

Code blocks can be extremely useful when writing instructions, especially in relation to computing and software. Thankfully, there are multiple ways to use code blocks with Markdown as seen below.

#### Code Block using Backticks

The easiest way to announce a code block is to use three backticks (`) at the beginning of the code and three backticks at the end of the code:

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

You may also use four indented spaces to indicate a block of code:

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

When conveying complex instructions it may be beneficial to have a code block in the middle of a list. For example:

1. Open the command line
2. Run the following command on your Linux Ubuntu machine to install Go

        sudo apt-get install golang 

3. Enter your administrator password

Syntax:
```
1. Open the command line
2. Run the following command on your Linux Ubuntu machine to install Go

        sudo apt-get install golang 

3. Enter your administrator password
```

## Images

Using images can draw the reader into your article by providing visual appeal, illistrating examples and conveying important messages. 

Syntax: 
```
![Text](commandline.jpg)
```

## Links

Providing links is an important way to direct the reader to sources or further reading materials. With Markdown you can turn text into a [link from text](https://www.markdownguide.org) via:

```
[link from text](https://www.markdownguide.org)
```

## URLs and Email Addresses

To use a URL or an email address as a link you may enclose either in angle brackets. **Example:** Email me at <email@example.com> or visit <https://www.markdownguide.org> for further information:

```
<https://www.markdownguide.org>
<email@example.com>
```

## Horizontal rule
---
The horizontal rule creates a line across the page which can be helpful to break up content. For example, the horizontal rule is in use and may be observed at both the start and end of this section. The horizontal rule may be acieved by using three or more asterisks, dashes or underscores on their own. Please note mixing and matching these symbols will not achieve the horizontal rule.

```
***
---
___
```
---
## Footnote Example