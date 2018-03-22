# Adding Custom Stylings

There are several different ways to make changes to the appearance of your site using your new child theme. You could use your `style.css` in your child theme folder, but in this case we're going to make changes to the footer of the TwentySeventeen theme.
1. First, go into the `footer.php` file in the parent theme folder. Select all of the code and copy.
2. Back in your child theme folder, create a new file called `footer.php`. **IMPORTANT**: The new file you are creating must match exactly the name exactly of which file you are making changes to. Once you've created `footer.php`, paste in the code you copied.
3. Above the `<footer...>` tag, create an opening/closing `div` with a class of `advertisement`. Inside the two tags, type something like `ads will be placed here` in opening/closing `p` tags.
