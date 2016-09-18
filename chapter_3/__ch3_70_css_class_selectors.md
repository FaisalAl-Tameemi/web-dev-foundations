# CSS Class Selectors

The next type of selectors we can use is called a class selector. It is especially useful because we may want to apply styles to a select few of tags. 

As we have seen before, tag selectors (nested or otherwise) will apply the styles to all elements that match that tag on the page and this may not be behaviour that we want.

Below is how we can use a class CSS selector.

In the html:

```html
<p class="styled-paragraph">
    Style this paragraph please :)
</p>
<p>
    This is another paragraph.
</p>
```

We have included `class="styled-paragraph"` as an attribute with a value for the first paragraph element but not the second.

Now, in the CSS code:

```css
.styled-paragraph{
    color: blue;
    font-size: 36pt;
}
```


----

## Resources & Links

...