# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!-- Code goes here -->
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>

</body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
Explain here.
An img tag is specifically used for pulling images into your html structure, when a div tag is used for many different things. Basicly for structure.
---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Explain here
```
Inline CSS is when you write your css properties directly in your html which will give them the highest specificity.

Internal style sheet is when you designate a css area in your one page document along with your html using the style tag. also giving a high specificity, but one lower than inline css.

External style sheet is the best method for adding css to your html, so that you can use one css page for multiple html pages. It also gives you control over the specificity. Then all you have to do is add a link tag in your html head to use your css page.


2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* comment like this */
/* this selector will apply border-radius to all div elements. border-radius will round the corners of your element. */
div {
  border-radius: 50%;
}

/* this is a class selector using "." which will give the font-size property to all elements with class header. font-size will adjust you text size. */
.header p {
  font-size: 18px;
}

/* this class selector operates on all elements with class footer. position: absolute will tell your elements exactly where to be place on the page. bottom is used for adjusting the margin at the bottom of your element selected. */
.footer {
  position: absolute;
  bottom: 0;
}

/* this will apply to all elements with class splash-image. background image provides a background from your designated url and applys it to your element. background-size: cover makes it so your image covers your entire element, and width 100% is telling all elements selected to use all 100% of the parent element in there display.
.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/* when you add a css property to your element name like hover here, you are declaring what css properties will happen when hover is activated. so here we are saying all elements that are hovered over will have the display of none and the color black which will change our text to black. */
.ninja:hover {
  display: none;
  color: black;
}
```

