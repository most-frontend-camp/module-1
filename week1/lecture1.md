# Lecture notes

# Lecture 1

## HTML

### What is the HTML?

HTML (Hypertext Markup Language)
- Describes the content and structure of a web page; not
  a programming language.
- Made up of building blocks called elements.

```javascript
<p>
 HTML is <em>awesome!!!</em>
 <img src="puppy.png" />
</p>
```


### name.html
Hit the shortcut doc4 or doc in name.html file and receive that one

```html
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">
      <title>Document</title>
  </head>
  <body>
    // content of the body
  </body>
</html>
```

head - Metadata that doesn't appear in the viewport of  the browser
title - shows up as the name of the tab
body - Contents that render in the viewport of the browser

### HTML Elements

An element usually has start and ending tags (<p> and </p>), content: stuff in between start and end tags

```javascript
<p>
 HTML is <em>awesome!!!</em>
 <img src="puppy.png" />
</p>
```
Also, 
1. An element can be self-closing (img)
2. An element can have attributes (src="puppy.jpg")
3. Elements can contain other elements (p contains em and img)

Another html tags:

1. [ ] Top-level heading h1, h2, ... h6  - <h1>Moby Dick</h1>
2. [ ] Paragraph - <p>Call me Ishmael.</p>
3. [ ] Line break - since feeling is first<br/> who pays any attention
4. [ ] Image - <img src="cover.png" />
5. [ ] Link - <a href="google.com">click here!</a>
6. [ ] Strong (bold) - <strong>Be BOLD</strong>
7. [ ] Emphasis (italic) - He's my <em>brother</em> and all

### HTML Types

Each HTML element is categorized by the HTML spec into one of
three-ish categories:
1. block: large blocks of content, has height and width <p>, <h1>, <blockquote>, <ol>, <ul>, <table>
2. inline: small amount of content, no height or width <a>, <em>, <strong>,<br> also,
 - inline block: inline content with height and width <img>
3. metadata: information about the page, usually not visible <title>, <meta>

### 1. Block elements:
Some info: 
- Take up the full width of the page (flows top to bottom)
- Have a height and width
- Can have block or inline elements as children
Examples are <p>, <h1>, <blockquote>, <ol>, <ul>, <table>.

Code snippet for block elements
```javascript
<h1>About vrk</h1>
<p>
 She likes <em>puppies</em>
</p>
```

### 2. Inline elements:
Some info: 
- Take up only as much width as needed (flows left to right)
- Cannot have height and width
- Cannot have a block element child
- Cannot be positioned (i.e. CSS properties like float and position do not apply to inline elements)
  - Must position its containing block element instead

  - Examples are <a>, <em>, <strong>, <br>

Code snippet for inline elements

```javascript
<strong>Web programming resources:</strong>
<a href="https://google.com://google.com">CS 193X</a>
<a href="https://developer.mozilla.org/en-US/">MDN</a>
<a href="https://google.com">Google</a>
```

#### Inline block
Examples: <img>, any element with display: inline-block;
- Take up only as much width as needed (flows left to right)
- Can have height and width
- Can have a block element as a child
- Can be positioned (i.e. CSS properties like float and position apply)


#### Meta Data
Metadata is — in its very simplest definition — data that describes data. 
For example, an HTML document is data, but HTML can also contain metadata in its <head> element that describes the document — for example who wrote it, and its summary.
Examples: <head>,  <title>.

Let's consider example below:
<meta charset="utf-8" />

This element specifies the document's character encoding — the character set that the document is permitted to use. utf-8 is a universal character set that includes pretty much any character from any human language.
If you set your character encoding to ISO-8859-1, for example (the character set for the Latin alphabet), your page rendering may appear all messed up:


### Practice 1
Go to folder practice1
Write down from scratch the sample.html


# Lecture 2

### HTML in forms


### Practice 2
Go to folder practice2
Write down from scratch the sample.html