# Loading CSS Files

There are 3 major ways to add CSS code to your HTML webpages. 

1. Via inline styles
2. Via the `<head>` tag
3. Via external styling files


### Inline

```html
<p style="color: red; font-size: 24;">
   My paragraph text...
</p>
```

The `style="color: red; font-size: 24;"` part is what makes the color of the paragraph text red and changes the font size.

The way we've applied the CSS styles above is referred to as __inline__.


### In the `<style>` Tag

We can insert the following code into the `<head>` tag of our HTML page.

```html
<head>
    ...
    <style>
        p {
            color: red;
            font-size: 24;
        }
    </style>
    ...
</head>
<body>
    <p> My paragraph text ... </p>
</body>
```


### External CSS Files

If we had placed our CSS code into an external file, for example: `style.css` then we can load the external CSS file into our HTML page as follows:

```html
<head>
    ...
    <link href="style.css" rel="stylesheet">
    ...
</head>
<body>
    <p> My paragraph text ... </p>
</body>

```

And the contents of our external CSS file (`./style.css`) would be as follows:

```css
p{
    color: red;
    font-size: 24;
}
```

