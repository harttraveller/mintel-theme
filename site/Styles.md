![[page.styles.jpg]]

This page is the documentation for the CSS styling choices. I've included comments on the CSS where the purpose might not be clear. The publish theme file is available in [this](https://github.com/harttraveller/mintel-theme/blob/main/publish.css) GitHub repository.

<p style="color: red;"><i>Work in progress...</i></p>
%%
# Note

There is likely a lot of redundant/malformed stuff here (I'm primarily a python developer focused on AI research in systems engineering, and not a web dev). If you ping me on GitHub if you spot something I could improve, I'd be grateful!

# Text Customization

## Font

I'm using the [inter](https://fonts.google.com/specimen/Inter?query=inter) font for this theme. It's imported with the line below.
```CSS
@import url('https://fonts.googleapis.com/css?family=Inter');
```
## Paragraphs

The `text-align` parameter assignment [justifies](https://www.shutterstock.com/blog/wp-content/uploads/sites/5/2018/07/shutterstock-align-typography-example-copy2.jpg) paragraph text.
```CSS
p {
    text-align: justify;
    font-family: 'Inter';
}
```
## Divs
```CSS
div {
    font-family: 'Inter';
}
```
## Headings

I don't normally go four levels deep, so I haven't yet added styling beyond H4. You can submit a feature request if you would use this.

Note that for headings 3 and 4, increasing `line-height` prevents expansion glitch when hovering over heading and copy header link button appears.
```CSS
h1 {
    color: #ffffff;
    font-size: 28px !important;
    font-family: 'Inter';
    font-weight: normal !important;
}

h2 {
    color: #cad1e2;
    font-size: 24px !important;
    font-family: 'Inter';
    font-weight: normal !important;
}

h3 {
    color: #9aa9c8;
    font-size: 20px !important;
    font-family: 'Inter';
    font-weight: normal !important;
    line-height: 1.4 !important;
}

h4 {
    color: #7689b0;
    font-size: 20px !important;
    font-family: 'Inter';
    font-weight: normal !important;
    font-style: italic !important;
    line-height: 1.4 !important;
}
```
## Links

Setting `text-decoration` to none removes the underline from the line. For the external link, setting `background-image` to none removes the external link icon - I think it looks better to differentiate with color than an icon. We also need to adjust the padding on the external link to normal, as the icon is no longer used.

```CSS
a,
.external-link {
    text-decoration: none !important;
    color: #7C8DFF;
    background-image: none;
    padding-right: 0px;
    font-family: 'Inter';
}

a,
.internal-link {
    text-decoration: none !important;
    color: #FF8D8D;
    font-family: 'Inter';
}
```

## Tags

Below we're setting the tag parameters before and after the mouse cursor hovers over it. `border-radius` makes the tags a little less round. `border` removes the border around the edge of the tag. The `transition` parameter adds a slight delay to the 
```CSS
.tag {
    font-family: 'Inter';
    border-radius: 4px !important;
    border: 0px !important;
    background-color: rgb(34, 59, 84) !important;
    transition: 0.3s;
}

.tag:hover {
    background-color: rgb(26, 105, 160) !important;
    transition: 0.3s;
}
```
%%