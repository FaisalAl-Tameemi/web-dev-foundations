# CSS Tag Selectors

If we recall the CSS syntax from 2 sections ago, we would know that to have a correctly written CSS style we would need the following:

- A __selector__, for example "p", to tell the page which elements we want to style
- A set of __property__ and __value__ pairs.

However, we have only ever seen one type of selectors and there are 3 main ones.

1. __Tag Selectors__ (ex: "p" or "img")
2. __Class Selectors__ (ex: ".my-paragraph" or ".contacts-list")
3. __ID Selectors__ (ex: "#paragraph-1" or "#main-navbar")

In this section, we will discuss and practice the first (and least specific) type of CSS selectors.

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


_Note:_ "px" stands for pixels.


