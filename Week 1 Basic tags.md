# Table of Content

- [Anatomy of HTML Tags](#anatomy-of-html-tags)
- [`<div></div>` Division](#division)
- [`<a></a>` Anchor (Link)](#link)
- [`<p></p>` Paragraph](#paragraph)
- [`<br>` Line Break](#line-break)
- [`<h1></h1>` Heading](#heading)
- [`<hr>` Horizontal Line](#horizontal-line)
- [Summary Sheet](#summary-sheet)

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


# Paragraph

for looooong text which normally contains sentence(s), we usually put it in proper `<p></p>`

go to some page that has long content and put it in `<p></p>` that's it...

Tips: for mocking a long paragraph, we usually use __Lorem Ipsum__ text. Go to [Google](www.google.com) and seach for "Lorem Ipsum Generator"

## Styling the text

I wish I could add more content about this section so please let me introduce you too __Styling__

you see it thru this material, it's the attribute called `style`

try this on your text editor

```
<p style="color: #00FF00;">
    this is long paragraph
</p>
```

save and open it, you will see the text is changed to be green.

so let's try more

```
<p style="color: #00FF00; text-align: center;">
    this is long paragraph
</p>
```

save and open, now the green text are aligning centered! 

you can try more on your own for styling the text inside `p` tag. 

I give you some keywords then you can go to google more about what we can style the text

`text-decoration`

`text-indent`

`text-transform`

`font-size`

`font-weight`

Go google!

# Link Break

In long paragraph, you may need to break in into new line, simply apply `<br>` into your paragraph

example,

```
<p>This is a long parangraph<br>and this is a new line</p>
```

# Heading

Heading in HTML has level from 1 to 6 - see the HTML code below

```
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

the actual different is the default size of text. Level 1 is the biggest and level 6 is the smallest.

you can also apply the [__Styling__](#styling-the-text) in previous section with this tag to! 

if you are a UI designer, the header will be useful for specified the hierarchy of paragraph heading :) 

make it fancy!

# Horizontal Line

`<hr>` will be a standalone tag that create a long line from end to end of the page's width.

try this on your text editor

```
<div>
    this is first
    <hr>
    this is second
</div>
<hr>
<div>
    this is third
</div>
```

save and open, you will see 2 lines on the page.

`hr` can be styling in many way, you can try

```
<hr style="height: 10px; background: pink;">
```

your line will be bigger and has pink color

if you dont like an ugly weird black border, try `border: 0;`

or if you'd like to change border color, try `border-color: green;`

there are more many way to style `<hr>` like making the dotted line, dashed line or else

Google with this words: hr style 



Example,

```
<hr style="border-top: 1px dotted red;">
```

create a read dotted line

# Summary Sheet

| Tags | what's for |
| ----- | ----------- |
| `<div></div>` | create a block of elements |
| `<a></a>` | make a link |
| `<h1></h1>` | biggest header (has level 1 to level 6) |
| `<p></p>` | make a paragraph |
| `<br>` | break into new line |
| `<hr>` | long line from end to end width of page |

# First Homework

create a new page that has your name on the top and your information

you may have some link to your own social network and introduce yourself a bit in short sentences (or Lorem ipsum is fine)

then try to styling it as you would like to, makes it fancy and most beautiful as much as possible
