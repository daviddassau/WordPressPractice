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
Author: David T. Dassau
Template:  twentyseventeen
*/
```
- Go back to WP, refresh, and activate your new child theme
- From there, you can start to add your own styles to the style sheet, and when you refresh your site, you can see the changes. 
- It also helps to have some sort of dummy data, so you can actually see changes made to your site.
  - HINT: You can Google "Wordpress theme unit test data", and you'll find a link to download some test content to your site.

### Set up multiple sites with custom domains
You can give your local sites custom domain names, instead of having them be `localhost/****`. Here are the steps:
1. Create a folder anywhere. EX: Create a folder called `MyWebProjects` in your Documents folder. Inside that folder, create a new folder, and name it whatever your project is going to be.
2. as;dkfj

### Create Boostrap Integrated WP Themes
