---
layout: default
title: Home
nav_order: 1
description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio."
permalink: /
---

# Markdown

This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.

<!--more-->

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1

## H2

### H3

#### H4

##### H5

###### H6

## Paragraph

Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris. Dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris. 

Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. 

## Images

### Basic inline image syntax:

![Alt text](https://github.com/seanmcquaide/seanmcquaide.github.io/blob/bcf3c903b1d9f97abf5ec0dbfdb1995b37cee2f6/puppy-unsplash.jpeg)

> `![Alt text](https://github.com/seanmcquaide/seanmcquaide.github.io/blob/bcf3c903b1d9f97abf5ec0dbfdb1995b37cee2f6/puppy-unsplash.jpeg)`

### Inline image syntax w/ title attribute:

![Alt text](https://github.com/seanmcquaide/seanmcquaide.github.io/blob/bcf3c903b1d9f97abf5ec0dbfdb1995b37cee2f6/puppy-unsplash.jpeg "image title attribute")

> `![Alt text](https://github.com/seanmcquaide/seanmcquaide.github.io/blob/bcf3c903b1d9f97abf5ec0dbfdb1995b37cee2f6/puppy-unsplash.jpeg "image title attribute")`

### Reference image link syntax:

<!-- create image references like this -->  
[id]: https://github.com/seanmcquaide/seanmcquaide.github.io/blob/bcf3c903b1d9f97abf5ec0dbfdb1995b37cee2f6/puppy-unsplash.jpeg "image title attribute"

> ```
> <!-- create image references like this -->  
> [id]: https://github.com/seanmcquaide/seanmcquaide.github.io/blob/bcf3c903b1d9f97abf5ec0dbfdb1995b37cee2f6/puppy-unsplash.jpeg "image title attribute"
> ```

<!--Using an image reference-->
![large indigo bounteous logo][id]  

> ```
> <!--Using an image reference-->
> ![large indigo bounteous logo][id]
> ```



## Blockquotes

### Standard Block Quote 

> Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris. Dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris.

```
> Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris. Dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris.
``` 

### Nested Block Quote

> Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris. 
> > Dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris.

```
> Lorem ipsum dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris. 
> > Dolor sit amet, consectetur adipiscing elit mauris eu malesuada odio. Cras rutrum urna vitae rutrum dapibus adipiscing elit mauris.
```

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

| Name  | Age | Location   |
| ----- | --- | ---------- |
| Bob   | 27  | Pittsburgh |
| Alice | 23  | Chicago    |
| Bob   | 27  | Pittsburgh |
| Alice | 23  | Chicago    |

### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------- | -------- | ------ |
| _italics_ | **bold** | `code` |

## Code Blocks

### Inline Code Block

`<h4>This is inline code.</h4>`

### HTML Code Block

This HTML is for a Fly-in modal.

```html
<!-- Start Fly-in HTML. Hidden until Live Demo link is clicked.  -->
<div id="popout" style="right: 0px;">
    <div id="hider"></div>
    <div style="float:left;width:400px;text-align:center;">
        <h2 style="margin:10px 0px;">How Lazy Are You?</h2>
        <p style="margin:10px 0px;">Copy our code. Get free Google Tag Manager<br>Recipes to track your website!</p>
        <a href="https://www.bounteous.com/insights/?category=resources/google-recipes&amp;secondary_category=All" id="button-381">Download Free GTM Recipes</a>
    </div>
</div>
<!-- End Fly-in HTML. Hidden until Live Demo link is clicked.  -->
```

### JS Code Block

This function show/hides the Fly-in. 

```js
// This function show/hides the Fly-in. 
function showPopOut() {
    jQuery("#popout").animate({
        right: "0"
    }, "fast", "linear", function () {
    });
}
jQuery("#hider").click(function () {
    jQuery("#popout").animate({
        right: "-440"
    }, "fast", "linear", function () { });
})
```

### CSS Code Block

This is the css controls the Fly-in styling.

```css
/* this is the css controls the Fly-in styling */
#popout {
    -moz-transition: all 0.5s ease;
    -webkit-transition: all 0.5s ease;
    -transition: all 0.5s ease;
    position: fixed;
    -webkit-transform: translateZ(0);
    width: 420px;
    max-width: 420px;
    height: 11rem !important;
    bottom: 200px;
    right: -440px;
    font-size:14px;
    z-index: 100;
    background-color:#f5f5f5;
    font-family: "Helvetica Neue", "Arial", sans-serif;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    -webkit-box-shadow: -4px 4px 8px rgba(0, 0, 0, 0.2);
    -moz-box-shadow: -4px 4px 8px rgba(0, 0, 0, 0.2);
    box-shadow: -4px 4px 8px rgba(0, 0, 0, 0.2);
    }
#hider {
    height:100%;
    width:17px;
    z-index:101;
    float:left;
    background-color:#ccc;
    background-image:url('https://optimize-training.web.app/training-code/close_small.png');
    background-position:top left;
    background-repeat:no-repeat;
}
#hider:hover {
    background-color:#fff;
    cursor:pointer;
}
#button-381 {
    display: inline-block;
    position: relative;
    width: 225px;
    height: 40px;
    color: #0229a5;
    background-color: #00fdff;
    border: 0;
    border-radius: 25px;
    font-family: "Nunito Sans",sans-serif;
    font-size: 1em;
    line-height: 2.5rem;
    font-weight: 800;
    text-align: center;
    text-decoration: none;
    cursor: pointer;
    overflow: hidden;
    padding: 0;
}
#button-381:hover {
    background: #196bff;
    text-decoration: none;
    color: #ffffff;
}
```

### Undefined Language Code Block

```
#button-381:hover {
    background: #196bff;
    text-decoration: none;
    color: #ffffff;
}
```

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

- List item
- Another item
- And another item

#### Nested list

- Fruit
    - Apple
    - Orange
    - Banana
- Dairy
    - Milk
    - Cheese

#### Checklist

- [ ] item type
    - [ ] item 1
    - [ ] item 2
    - [ ] item 3
- [ ] item type
    - [ ] item 1
    - [ ] item 2
    - [ ] item 3

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Backslash escapes

Certain characters can be escaped with a preceding backslash to preserve the literal display of a character instead of its special Markdown meaning. This applies to the following characters:

\\  backslash  
\`  backtick  
\*  asterisk  
\_  underscore  
\{} curly braces  
\[] square brackets  
\() parentheses  
\#  hash mark  
\>  greater than  
\+  plus sign  
\-  minus sign (hyphen)  
\.  dot  
\!  exclamation mark  
