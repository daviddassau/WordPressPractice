# Editing the Twenty Seventeen Wordpress Theme

If you'd like to get rid of those pesky page titles on the side, you can do the following:

Add this to the `style.css` in your child theme folder...
```CSS
body.page-template-template-full-width #content #primary {
	max-width: 100%;
}

body.page-template-template-full-width #content #primary .entry-header,
body.page-template-template-full-width #content #primary .entry-content {
    float: none;
    width: 100%;
}

body.page-template-template-full-width #content #primary .entry-header {
    margin-bottom: 4em;
}
```
