# WordPressPractice

### Up and Running
- First, you need to install WAMP, if you're running Windows. MAMP if you're running on a Mac.
- Once you have WAMP or MAMP installed, you need to download a copy of the latest version of WordPress from Wordpress.org.
  - To get setup with Wordpress locally, navigate to where you installed WordPress on your computer.
  - Click on the zip folder > Wordpress > and select all files and copy.
  - Click on the WAMP icon, and go to www directory. From there, you can create a new folder, name it whatever your site/project is. Inside that folder, you'll paste in all of the copied WP files.
  - Then, in your browser, you can type in localhost/whateverYouNamedYourFolder, and this will bring you to the first WP page, where you select your language.
  - You then want to again click on the WAMP icon, click on phpMyAdmin, and log in. Once you're in, you want to create a new database, and call it the same thing that you called this project.
  - Once you've done that, you can go back to the window in your browser with WP. Run through the steps.
- Once you have that, you need to chose a parent theme for your Wordpress site. This can be any theme you want. It's easiest to start out with the official WP themes, such as `twentyseventeen` or `twentysixteen`. You can do this by inside the WP dashboard, clicking on Appearance > Themes > and choose which theme you want.
- After you have your parent theme activated, you need to open up your source files in a text editor. Navigate to the mysite > wp-content > themes folder. Right-click on the themes folder, and create a new folder. You want to make sure it's apparent that this new folder is a child theme, so name it something like `childoftwentyseventeen`. Inside that folder, create a `style.css`. In the style.css, you want to type out something like this:
```CSS
/*
Theme Name: Child of Twenty Seventeen
Theme URI: (this will be wherever your site is hosted)
Description: A child theme of Twenty Seventeen
Author: David T. Dassau
Author URI: (Your personal develper website)
Template:  twentyseventeen
Version:
*/
```
- Go back to WP, refresh, and activate your new child theme
- From there, you can start to add your own styles to the style sheet, and when you refresh your site, you can see the changes. 
- It also helps to have some sort of dummy data, so you can actually see changes made to your site.
  - HINT: You can Google "Wordpress theme unit test data", and you'll find a link to download some test content to your site.

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
