![[page.styles.jpg]]

This page is the documentation for the CSS styling choices. I've included comments on the CSS where the purpose might not be clear. The publish theme file is available in [this](https://github.com/harttraveller/mintel-theme/blob/main/publish.css) GitHub repository.

# Text Customization

## Font Import

I'm using the [inter](https://fonts.google.com/specimen/Inter?query=inter) font for this theme. It's imported with the line below.
```CSS
@import url('https://fonts.googleapis.com/css?family=Inter');
```
## Paragraph Alignment & Font

The `text-align` parameter assignment [justifies](https://www.shutterstock.com/blog/wp-content/uploads/sites/5/2018/07/shutterstock-align-typography-example-copy2.jpg) paragraph text.
```CSS
p {
    text-align: justify;
    font-family: 'Inter';
}
```

## Div Font
```CSS
div {
    font-family: 'Inter';
}
```

