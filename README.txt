-----------SIMPLE WEB SERVER SETUP & CONFIGURATION GUIDE-----------

Welcome to the Simple Web Server Setup and Configuration Guide! This README will walk you through the process of setting up and configuring a basic web server. 

###Table of Contents
1.Introduction
2.Prerequisites
3.Project Setup
    -Step 1: Installing the Web Server Software
    -Step 2: Configuring Web Server
4.Accessing Your Website
5.Troubleshooting
    -Common Issues and Solutions
6.Important Lessons Learned
7.Conclusion

###Introduction
In this project, we'll be setting up a basic web server to host a static website. A web server is essential for delivering web content to users' browsers over the internet. We'll be using a popular web server software, and this guide will help you through the installation, configuration, and troubleshooting processes.

###Prerequisites
Before you begin, make sure you have:
- A server or virtual machine running a supported operating system (e.g., Linux Ubuntu 20.04).
- Basic command-line knowledge.
- Access to the terminal with administrative privileges.
- Your website's HTML/CSS content ready.

###PROJECT SETUP
##Step 1: Installing the Web Server Software
1.Open a terminal window.
2.Update your package list: "sudo apt update -y".
3.Install the web server software (we'll use Apache here): "sudo apt install apache2 -y".
4.Start the Apache service: "sudo systemctl start apache2"
5.Enable it to start on boot: "sudo systemctl enable apache2".

##Step 2: Configuring Web Server
1.Navigate to the web server's configuration directory: "cd /etc/apache2/JOHN DOE".
2.Create a configuration file for your website (e.g., "JOHN DOE").
3.Edit the configuration file to specify your website's settings:
4. Create the directory to store your website files: `sudo mkdir -p /var/www/html/mywebsite`.
5. Copy your website files into the directory: `sudo cp -r /path/to/your/website/* /var/www/html/mywebsite/`.
6. Set the correct permissions: `sudo chown -R www-data:www-data /var/www/html/mywebsite`.
7. Enable your site configuration: `sudo a2ensite mywebsite.conf`.
8. Reload Apache for changes to take effect: "sudo systemctl reload apache2".

###Accessing Your Website
Open a web browser and enter your server's IP address or domain name. You should see your website's content displayed.

###Troubleshooting
If you encounter issues:

###Common Issues and Solutions
1.Web server not starting: Check for syntax errors in your configuration files using `sudo apache2ctl configtes".
2.Permission issues: Ensure proper permissions on website files: "sudo chown -R www-data:www-data /var/www/html/mywebsite".

###Important Lessons Learned
Through this project, you've learned:
-Installing and configuring a basic web server.
-Managing virtual hosts to host multiple websites.
-Troubleshooting common web server issues.
-The importance of file permissions and ownership.

###Conclusion
Congratulations! You've successfully set up a basic web server to host your static website. This knowledge forms a solid foundation as you explore more advanced web server configurations and technologies.



