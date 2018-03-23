# Using Github with your local Wordpress site

When using Github to manage your local Wordpress workflow and updates, there are a few important things to know.

One of the most important things is setting up your `.gitignore` file properly within your repo.
1. First, you need to visit https://ironcodestudio.com/bare-minimum-git/ and scroll down to where you see "Bare Minimum Git .gitignore files". Click on "WordPress .gitignore". Alternatively, you can just go directly to https://gist.github.com/salcode/9940509
2. Copy all of the raw data from that big block of code. Then, you can either paste it in to your current .gitignore file, replacing all of the current data. Or, if you don't have a .gitignore file yet, create one and paste in the code.
3. Then, you'll want to right-click in your repo folder on your computer (where all the WP files are) and git bash there. Then do a `git init`.
4. You'll then want to do a `git add .gitignore`, so we're staging that file first, before anything else.
5. Then do a `git commit -m "adding .gitignore"`
6. Finally, do a `git push origin master`
7. Now you should be able to go back to Github, refresh your repo page, and all the added files (which should just be the `.gitignore` and `README.md`) should now be visable.


### Resources
Putting Your WordPress Child Theme Under Git Version Control
https://www.youtube.com/watch?v=I9o6GelEo6Q
