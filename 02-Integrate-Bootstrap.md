# Integrate Bootstrap Into Your Child Theme

1. The first thing you want to do is, on the themes folder in your code editor, right-click and create a new folder called "parent_theme_name-child".
2. A child theme folder needs to have at least two files: the `style.css` and `functions.php` files. You can navigate to https://codex.wordpress.org/Child_Themes to get more info.
3. From that site, you can use the chunk of code to paste at the top of your new `style.css` file that's inside the `-child` folder. Don't forget to change everything to match what you need it to be in the commented out code!
4. Also from that site, you can use the chunk of code for the `functions.php`. There are two blocks to choose from, it's best to use the second block, so that you can change the CSS. Don't forget to change the name of the parent theme in the commented out code!
5. Head over to the WP dashboard, and under Appearance, switch to your brand new child theme, and activate it.
6. You'll also want a `header.php` and `footer.php` in your child theme folder. You can copy these two files from the parent theme, and paste them into your child theme.
7. Then you'll want to head over to getbootstrap.com, and grab the CDNs for the CSS, JavaScript, and jQuery. You'll want to paste the CSS CDN into the `header.php` right before the closing header tag. Then paste in the JS and jQuery CDNs into the `footer.php` at the bottom before the closing body tag.
