# WordPressPractice

### Set up multiple sites with custom domains
You can give your local sites custom domain names, instead of having them be `localhost/****`. Here are the steps:
1. Create a folder anywhere. EX: Create a folder called `MyWebProjects` in your Documents folder. Inside that folder, create a new folder, and name it whatever your project is going to be.
2. Then, you want to navigate back to wherever you installed WP, copy all of the files, then head back to your new project folder, and paste those bad boys in.
3. What you need to do next is start creating your custom domain. First, inside the finder window in the "url" box with the folder path, click in there and copy the path. Then you want to go to your browser > localhost > Add Virtual Host. Once you're there, paste in the pathway in the last box with the green boxes.

### Create Boostrap Integrated WP Themes
1. The first thing you want to do is, on the themes folder in your code editor, right-click and create a new folder called "parent_theme_name-child".
2. A child theme folder needs to have at least two files: the `style.css` and `functions.php` files. You can navigate to https://codex.wordpress.org/Child_Themes to get more info.
3. From that site, you can use the chunk of code to paste at the top of your new `style.css` file that's inside the `-child` folder. Don't forget to change everything to match what you need it to be in the commented out code!
4. Also from that site, you can use the chunk of code for the `functions.php`. There are two blocks to choose from, it's best to use the second block, so that you can change the CSS. Don't forget to change the name of the parent theme in the commented out code!
5. Head over to the WP dashboard, and under Appearance, switch to your brand new child theme, and activate it.
6. You'll also want a `header.php` and `footer.php` in your child theme folder. You can copy these two files from the parent theme, and paste them into your child theme.
7. Then you'll want to head over to getbootstrap.com, and grab the CDNs for the CSS, JavaScript, and jQuery. You'll want to paste the CSS CDN into the `header.php` right before the closing header tag. Then paste in the JS and jQuery CDNs into the `footer.php` at the bottom before the closing body tag.

### Adding Custom Stylings
There are several different ways to make changes to the appearance of your site using your new child theme. You could use your `style.css` in your child theme folder, but in this case we're going to make changes to the footer of the TwentySeventeen theme.
1. First, go into the `footer.php` file in the parent theme folder. Select all of the code and copy.
2. Back in your child theme folder, create a new file called `footer.php`. **IMPORTANT**: The new file you are creating must match exactly the name exactly of which file you are making changes to. Once you've created `footer.php`, paste in the code you copied.
3. Above the `<footer...>` tag, create an opening/closing `div` with a class of `advertisement`. Inside the two tags, type something like `ads will be placed here` in opening/closing `p` tags.
