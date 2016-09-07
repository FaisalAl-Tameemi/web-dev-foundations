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

Which would result in this: <a href="http://google.com">Go To Google</a>

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

----

## Resources & Links

### [W3Schools Tags List](http://www.w3schools.com/tags/default.asp)

### [Mozzile Element Reference](https://developer.mozilla.org/en/docs/Web/HTML/Element)
