## Instructions for migrating your local WordPress site to your host/server

### Step 1
1. Download the plugin [**Duplicator**](https://wordpress.org/plugins/duplicator/)
2. Once installed, navigate to the Duplicator main page.
3. Click on **Create New** to create a new package.
4. Give your package a name, and feel free to add notes if you need/want to. When you're done, click **Next**.
5. Duplicator will run a system scan to help determine any potential issues. Once it's done, hit **Build** to create your package.
6. Now the plugin will begin backing up your site. Duplicator will produce two files for you: an archive of your site, as a `.ZIP` file; and an installer file, as a `.PHP` file.

### Step 2
1. You will need Filezilla for this step. Open up Filezilla, login to your site via FTP, navigate to your `public_html` folder and copy the archive and installer files from your computer to the folder.

### Step 3
1. Now we need to install the archived site on the live server. We do this by accessing the installer file we just copied into the live site. In your browser, go to yourdomain.com/installer.php.
2. If you did this correctly, you should see the installer interface, prompting you to add your MySQL details. Click **Create New**.

### Resources
https://premium.wpmudev.org/blog/guide-to-migrating-localhost-wordpress-to-live-site/
