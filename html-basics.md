# HTML Basics

## What is HTML?

- HTML stands for Hyper-Text Markup Language
- **HyperText** refers to any text/document referring i.e. linking to other documents
- **Markup** means to annotate content. We wrap our content inside **semantic tags to annotate** that it is a particular type of content. **XML** is also a markup language
- `HTML` provides **Structure** ; `CSS` provides **Style** ; `JS` provides **Behaviour**

---

## Resources

1. [**W3C**](https://www.w3.org/) makes the HTML standards. W3C also has an [HTML validator](https://validator.w3.org/)
1. [**WHATWG**](https://whatwg.org/) consists of browser vendor groups that keep trying out new features
1. Refer [CanIUse](https://caniuse.com/) for checking support of a web feature across browsers

---

## Anatomy of HTML tag

```html
<p id="ap01r" class="filler intro" onClick="alert('hi')">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum
  ullamcorper rutrum orci at posuere.
</p>
```

- `p` is known as the paragraph **Element**
- `<p>` and `</p>` are the opening & closing **Tags** of a paragraph
- `id`, `class`, `onClick` are the **attributes** and their **attribute values** are specified in quotes
- The Lorem ipsum text inside the tag is called the **Content**

> **Note:**

- Most tags come in opening & closing tag pairs (`<h2>...</h2>`). However, there are some special tags that don't have a closing tag. These are called **Void element** tags i.e. they cannot contain any children inside them. Examples are `<br>`, `<hr>`, `<img>`, `<input>`, `<meta>`, `<link>` . Refer [MDN docs](https://developer.mozilla.org/en-US/docs/Glossary/Void_element)
- HTML does NOT have self-closing tags. For example `<img.../>` is not valid HTML
- The element name can be written in any case (upper/lower/mixed)
- No spaces between `<` and `p` or `/p` of the tags
- At least one space required before and between attributes
- Specify attributes ONLY in the opening tag

---

## Basic HTML Document Structure

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Homepage</title>
  </head>
  <body>
    <h1>This is the homepage</h1>
  </body>
</html>
```

- The `<!doctype html>` standalone tag is used to indicate that the document is an HTML document to be rendered in **standard mode**. Without this tag, the browser assumes the document to be of some other format or legacy standards and it will be rendered in **quirks mode**. Refer [MDN page for Quirks & Standard modes](https://developer.mozilla.org/en-US/docs/Web/HTML/Quirks_Mode_and_Standards_Mode).
- The `<html>...</html>` tags are HTML document
- The `<head>...</head>` tags contain description about the content inside the page. This includes metadata, external resources to import, and the required `<title>...</title>` tags
- The `<body>...</body>` tag is the **root** of all content that is visible to the user. It is also called as the **viewport**
- The HTML document is rendered from top to bottom
