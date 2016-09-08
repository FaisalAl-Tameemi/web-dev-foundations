# Tag Variations

## Normal Tags

The tags we discussed in the previous section (`<p>` and `<h1>`) are both examples of normal tags. There are however other types of tags available which we will discuss next.

## Tags with Attributes

If we wanted to show a link on our webpage, we can use the `<a>` tag (stands for _anchor_). For example, let's say we want to link to the google homepage from our page. 

We know that the google page URL is __http://google.com__. Our HTML will then be as follows:

```html
<a href="http://google.com">
    Go To Google
</a>
```

Which would result in this:

{% codeeditor src='../assets/sources/001_html_links.html' %} {% endcodeeditor %}


In the code above, we've used the __href__ attribute to tell our browser the place it should go to once the user clicks the link.

Another attribute we can add to our link tag is a __target__. Clicking the link above will actually change our current tab on the browser to the specified URL (aka link). Using the __target__ attribute and giving it the value of _"_blank"_ would tell the browser to open the URL in a new tab on the browser.

```html
<a href="http://google.com" target="_blank">
    Go To Google In New Tag
</a>
```

which would show: <a href="http://google.com" target="_blank">Go To Google In New Tag</a>

We could also add an `id` tag to our link if we wanted to refer to it later

```html
<a href="http://google.com" target="_blank" id="google-link">
 Go To Google In New Tag
</a>
```

There is no limit to the number of attributes an element has.


### With Opening Tags

Some tags don't require that you close them, this is because there is no content that goes between the opening tag and close tag in their case. An example of this kind of tags is an `<img>` tag. 

The main attribute we need to be able to show an image is `src` (stands of source) which indicates the location of the image on the web:

```
<img src="http://bit.ly/1OMiOIV" />
```

which would result in:

<img src="http://bit.ly/1OMiOIV" />


If you visit the link, you'll notice that the only thing on that page is the image itself, that's the kind of URL we need to provide in the tag.

We can also add attributes like `height` and `weight` to change the size of the image (checkout the resources below).


### Nested Tags

In the example below, we can see that HTML allows us to place tags within other tags. This is HTML's way of allowing us to express more complicated structures.

For example, we will us the `<body>` tag to define the main content of the page but within that we will use many other tags and keep nesting them.

```html
<article>
    <header>
        <h2> Our Article </h2>
        <h3> Written by… </h3>
    </header>
</article>
```

Remember that humans are the only ones that care about indentation. HTML actually ignore anything more than one whitespace and considers it as a single whitespace.

This means we could rewrite the code above as:

```html
<article><header><h2> Our Article </h2><h3> Written by… </h3></header></article>
```

and that would result in the same thing but much harder to read.


### HTML Page Skeleton

HTML pages are general composed of the following structure:

```html
<!doctype html>
<html>
    <head>
        ... (other tags here)
    </head>
    <body>
        ... (other tags here)
    </body>
</html>
```

Every webpage starts with the `<!doctype html>` to tell the browser about the kind of the document we have written and what to the expect.

The `<html>` tags wraps up the entire page. While the `<head>` tag within in contains other files that we may need as well as some metadata about the page. We will work within the `<head>` tag in upcoming sections as we start to work with CSS and Javascript.

The `<body>` tag is where we will place the content that we want to display within our page. This means all the `<p>` tags and the `<a>` tags go into the `<body>` tag.


The goal of HTML tags is to be as descriptive as possible of the content they contain. This is what we refer to as __Semantic Tags__. An example of those include `<footer>` which clearly describes the content of the footer of the page. Another one is `<hav>` which describes a navigation menu or bar.


### Default Styling

Some tags such as `<h1>` through to `<h6>` contain some minimal default styling but it can all be changed with CSS as we will see in the next chapter.


----

## Resources & Links

### [W3Schools Tags List](http://www.w3schools.com/tags/default.asp)

### [Mozzile Element Reference](https://developer.mozilla.org/en/docs/Web/HTML/Element)

### [Read more about image tags](http://www.w3schools.com/tags/tag_img.asp)