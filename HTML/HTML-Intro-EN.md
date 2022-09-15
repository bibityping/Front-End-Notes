# HTML Intro

[中文版本](HTML-Intro.md)

HTML is an abbreviation for Hypertext Markup Language. It is not a programming language, but a markup language used to structure the content of web pages.

HTML is like building a house with only a structure.

<img src="https://cdn.pixabay.com/photo/2018/05/03/10/18/housebuilding-3370969_1280.jpg" alt="House framing">

## HTML Elements

📎 HTML documents are made up of many elements.

📎 The content of the HTML element is written in the Opening tag and the Closing tag.

Take the `<p>`element as an example,the opening tag `<p>`is the Opening tag，the last tag `</p>`is the Closing tag,the content of the element "I am a Front-end Engineer"is written between these two tags.

```html
<p>I am a Front-end Engineer</p>
```

Attributes can be added within the opening tag of an element, and the attributes provide additional information to the HTML that is not displayed in the page.

Take the anchor tag `<a>`as an example，add the`href`attribute to the opening tag，which will jump to the specified page when the user clicks on it.

```html
<a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a"
  >The Anchor element</a
>
```

## HTML Empty element

Not all HTML elements have closing tags.

##### For example：

`<br>`
`<hr>`
`<input>`
`<img>`
`<meta>`
`<link>`

## HTML Structure

HTML documents have a standard writing specification.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Frontend Tutorial</title>
  </head>
  <body>
    <h1>HTML</h1>
  </body>
</html>
```

#### Explanation of code：

- `<!DOCTYPE html>`Define that the document is written in the HTML5 syntax
- `<html>`is the root element that wraps all the content of the page, where the `lang` attribute specifies the language of the element's content
- `<head>`Contains metadata for the HTML page that will not be displayed on the page
- `<meta charset="UTF-8">` Set the UTF-8 character set
- `<title>`is the title of the page, which appears on the browser tab
- ` <body>` All the content displayed on the HTML page is inside this tag
- `<h1>`is a title tag

## Reference

```

https://developer.mozilla.org/en-US/docs/Web/HTML


```
