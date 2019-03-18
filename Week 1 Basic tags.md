# Table of Content

- Anatomy of HTML Tags
- `<div></div>` Division
- `<a></a>` Anchor (Link)
- `<p></p>` Paragraph
- `<h1></h1>` Heading
- `<br>` Line Break
- `<hr>` Horizontal Line
- Summary Sheet

# Welcome

Hello, there!

Welcome to the HTML Basic Course :)

This repository is dedicated for helping friend to learn the basic of HTML that we need to know for newly creating a simple site.

Today, we are going to go thru 5 basic tags we mostly use on HTML those are listed in the table of content!


# Anatomy of HTML Tags

We will use this concept for all along the course. 

Don't be worried if you feel confused about the syntax because we'll try the best on the practical workshop.

You will not even realize that it's already stick in your head, lmao.


## Get Started

like other programming language, HTML also has its own syntax and web browser will properly interpret HTML code to our beautiful website.

Before going deep into HTML code, we have to understand the anatomy of HTML first!

HTML are basically compose of 2 things: element name and attribute(s)

```
<element-name attribute="value"></element-name>
```

* __element-name__: name of HTML component, ex. `div`, `a`, `button` and so on
* __attribute__: most of attributes for HTML are optional but basically if we want to have fancy options for our html then we need to specify the attribute with value.

for example

```
<div id="myDiv">this is my div</div>
```

`div` is an element name

`id="myDiv"` is an attribute `id` that has value `myDiv`

`this is my div` is the content inside the scoped of `div` block


## Tag Closing?


> __once we open the tags (like this `<div>`), we will usually close the tag (like this `</div>`)__

most of HTML tags requires to the closing tag like `<div></div>`, `<a></a>`, `<section></section>`

but some of the tags __are not__ requires the closing tag because it's already completed in itself. We can call it __Self-Closing__ tag.

for example, `<input />` << this is a Self-Closing tag because it does not require the content inside the tag

and there are some tags those can be isolated on itself and no need `/` to close the tag

for example, <br> and <hr>


## Before you move on

Say again - Don't be worried if you can't remember how many kind of the tag closing has nor the anatomy/syntax of HTML

the best way for learning is to do it practically!

so open your text editor and web browser. let's try as much as you can!


# Division

need a divided block for adjusting the elements? - let's use `<div></div>`

1. open your text editor and try

```
<div>my first div</div>
```

2. save it as `whatevername.html` and open it in web browser
3. Congratulations! you have your first `div` tags with the content as `my first div` inside showing in the screen!

`div` has been using anywhere where you would like to make a block of elements and adjust the layout

> if you are thinking about "Layout", think about `div`

(Creating a beautiful layout will be covered later in the course)

# Link

now we're talking about __Linking__

to jump from this website to another website, we can call it a __Link__

Link in HTML con be introduced with `<a></a>`

try this on your text editor 

```
<a href="https://www.google.com/">Go to Google<a>
```

it will show an underline blue text.

And if you click on the text, it will go to Google site!

## Jumping with Link

`href` is the attribute of `a` tag where we can specify a destination of where we want to go - _even in our own page!_

for example, if there is a `div` element in the bottom of the page and we want to click on a link and it will jump to that div

try this

```
<div style="width: 150%;">
    <a href="#footer">Go to bottom</a>
</div>
<div id="footer">
   this is bottom
</div>
```

save and open it in web browser, you will see "Go to bottom" on the top and when you click on it, it will jump to the bottom of the page

why?

because when `href` value is using `#`, it means "please jump to the element that has this `#id`

`#` is the represent of id. If that id is not present anywhere in the HTML code, it _also_ won't jump to anywhere.






