# CSS ID Selectors

The last and most specific type of selectors is an ID selector. Unlike the other types of selectors, the ID selector is usually only applied to a single element. 


### How does this translate to code?

We add an `id` attribute to the HTML element as follows:

```html
<img src="http://bit.ly/2cGjisn" id="logo-main" />
```

In the code above, we have created an image tag for a logo image and added the `id` attribute.

Now, in our CSS, we can do the following to select ONLY that element and specify our styles:

```css
#logo-main{
    height: 200px; /* px means pixels */
}
```

The final result would be as follows (the `result` tab may take a second to load):

{% codeeditor src='../assets/sources/004_css_id_selector.html', readOnly='false' %} {% endcodeeditor %}


----

## Resources & Links


### [CSS Selectors - W3Schools](http://www.w3schools.com/css/css_syntax.asp)

