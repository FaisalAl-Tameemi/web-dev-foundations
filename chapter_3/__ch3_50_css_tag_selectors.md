# CSS Tag Selectors

If we recall the CSS syntax from 2 sections ago, we would know that to have a correctly written CSS style we would need the following:

- A __selector__, for example "p", to tell the page which elements we want to style
- A set of __property__ and __value__ pairs.

However, we have only ever seen one type of selectors and there are 3 main ones.

1. __Tag Selectors__ (ex: "p" or "img") and __Nested Tags__
2. __Class Selectors__ (ex: ".my-paragraph" or ".contacts-list")
3. __ID Selectors__ (ex: "#paragraph-1" or "#main-navbar")

In this section, we will discuss and practice the first (and least specific) type of CSS selectors.

### Tag Selectors

Tag selectors work by specifying the type of HTML tag that we would like to style. A __gotcha__ with this type of selectors is that the style specified will be applied to ALL html elements with that tag.

For example, if we had 3 paragraphs on an HTML page:

```html
<p>
    Paragraph 1
</p>
<p>
    Paragraph 2
</p>
<p>
    Paragraph 3
</p>
```

and then loaded a CSS file which contained the following code:

```css
p{
    font-size: 36px;
    letter-spacing: 2;
}
```

then all the paragraphs on the page would be styled the same. Large characters and spaced out. As you can imagine, we may need more specifity as we build more complex UIs (user interfaces).

### Nested Tag Selectors

Another way to write CSS tag selectors is to nest them. 

That means we can specify the styles of certain tags which are inside of other tags.

Consider the following HTML code:

```html
<div>
    <p>
        My paragraph text...
    </p>
</div>
<p>
    A paragraph outside the div...
</p>
```

Now if we wanted to style only the paragraph that are inside of `div`s, then our CSS code would be the following:

```css
div p {
    color: blue;
}
```

which specifies that only paragraphs that are inside of `div` tags should change their text color to blue.

The final result of the code above would be as follows:

{% codeeditor src='../assets/sources/002_css_tag_selector.html', readOnly='false' %} {% endcodeeditor %}

In the upcoming sections, we will look into more specific ways of applying CSS styling. Ways that could allows us to apply styles to specific elements on the page.


----

## Resources & Links

### [CSS Selectors - W3Schools](http://www.w3schools.com/css/css_syntax.asp)
