# Lecture notes

# Lecture 1

## HTML

### What is the HTML?

HTML (Hypertext Markup Language)
- Describes the content and structure of a web page
- not a programming language
- Made up of building blocks called elements

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

An element usually has 
- start tags (`<p>`)
- ending tags (`</p>`)
- content: stuff in between start and end tags

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

1. [ ] Top-level heading `h1, h2, ... h6  - <h1>Moby Dick</h1>`
2. [ ] Paragraph - `<p>Call me Ishmael.</p>`
3. [ ] Line break - since feeling is first `<br/>` who pays any attention
4. [ ] Image - `<img src="cover.png" />`
5. [ ] Link - `<a href="google.com">click here!</a>`
6. [ ] Strong (bold) - `<strong>Be BOLD</strong>`
7. [ ] Emphasis (italic) - `He's my <em>brother</em>` and all

### HTML Types

Each HTML element is categorized by the HTML spec into one of
three-ish categories:
1. block: large blocks of content, has height and width` <p>, <h1>, <blockquote>, <ol>, <ul>, <table>`
2. inline: small amount of content, no height or width `<a>, <em>, <strong>,<br>` also, inline block: inline content with height and width `<img>`
3. metadata: information about the page, usually not visible` <title>, <meta>`

### 1. Block elements:
Some info: 
- Take up the full width of the page (flows top to bottom)
- Have a height and width
- Can have block or inline elements as children
Examples are` <p>, <h1>, <blockquote>, <ol>, <ul>, <table>`.

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
  - Examples are` <a>, <em>, <strong>, <br>
`
Code snippet for inline elements

```
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
For example, an HTML document is data, but HTML can also contain metadata in its `<head>` element that describes the document — for example who wrote it, and its summary.
Examples:` <head>,  <title>`.

Let's consider example below:
`<meta charset="utf-8" />`

This element specifies the document's character encoding — the character set that the document is permitted to use. utf-8 is a universal character set that includes pretty much any character from any human language.
If you set your character encoding to ISO-8859-1, for example (the character set for the Latin alphabet), your page rendering may appear all messed up:

#### Meta viewport tag

Unless directed otherwise via HTML or CSS cues, mobile browsers render web pages at a desktop screen width (~1000px), then "zooms out" until the entire page fits on screen.
```
<meta name="viewport" content="width=device-width, initial-scale=1">
```

### Practice 1
Go to folder practice1
Write down from scratch the sample.html

# Lecture 2

### HTML Structure

HTML - язык разметки, Язык декларативный, Семантика

Говоря же о семантике в HTML — обычно имеют ввиду использование именно смысловых тегов, вместо обычных div.

Пример страницы с div - `indexdiv.html`

При написании содержимого в HTML, такого как абзацы, списки или ссылки, вы наделяете смыслом свой текст. Но вы, возможно, захотите сгруппировать некоторые из этих элементов вместе.

### HTML Core Tags
Например, веб-страницу блога можно разделить на четыре части:

1. «шапка», которая похожа на каждой странице и является главной навигацией по сайту;
2. основное содержание, что меняется для каждой страницы: список статей, одна статья с комментариями, страница «о нас» и др.;
3. боковая панель, которая содержит ссылки на ежемесячные архивы и категории;
4. «подвал» для дополнительных ссылок на менее важные страницы.

### Div, Aside, Section, Article
— Тег div — это универсальный элемент для группировки элементов.
— Элемент main необходим для разметки части страницы, в которой
находится ее основной контент.
— Элемент aside определяет область страницы, которая дополняет ее основной контент.
— Элемент section служит для создания раздела страницы, смысл которого определяется заголовком.
— Элемент article разделяет страницу на независимые области, которые можно вынести из своего логического окружения, и они не потеряют свой смысл.

### div, article or section?

Чтобы определиться, какой из элементов выбрать, можно использовать алгоритм:
— Будет ли содержимое иметь осмысленное значение само по себе, например, при публикации в ленте новостей? Если да, то выбираем
article
— Если части содержимого объединены общим смыслом, то выбираем section
— Наконец, если нет никакого семантического значения, то выбираем div



# Lecture 3
### HTML forms
HTML forms are used to get information from users. 

They are widely used in webpages or apps for surveys or registration processes.

HTML form basics include the common HTML elements, tags, attributes, concepts, or best practices required for you to create good HTML forms.

### Sample form
Тег <form> используется для создания HTML-формы. 

В нём находится всё содержимое формы: поля для ввода, подписи к этим полям и кнопка отправки.

```
  <html>
  <head>
      <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">
      <title>Document</title>
  </head>
  <body>
      <form action ='/login' method='post'>
          <label for='username'>Имя персонажа:
          </label>
          <input type='text' id="username" name="username"><br>
          <label for='password'>Пароль персонажа:
          </label>
          <input type='text' id="password" name="password"><br>
          <input type='submit' value="Войти">
      </form>
  </body>
  </html>
```

### Practice 2
Go to folder practice2
Write down from scratch the sample.html