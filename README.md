# Guides
Guides for yclas.com
# Getting Started with Yclas Self-Hosted

Welcome! 👋

**Yclas Self-Hosted** is a classifieds script that helps you run a fully functional classifieds website needing from little to no knowledge in web-design or web-development. This free open source software is ready for any modification from developers or advanced users.

The software can be used for a variety of purposes, from automobiles and real estate classifieds to wedding planning services and fish accessories.




# What do you get with Yclas Self-Hosted?

You get access to open source and you can use **hostpapa hosting services.** 
After purchasing, you’ll receive a license for hostpapa.com as well as **one domain name for free**. 

Moreover, you’ll get all of Yclas’s features and themes and **1 month of Pro Support for free.**

You can use your own server or your current web hosting if you have one. Yclas only **requires PHP 7 Apache and MySQL to run.**

You have complete control over your server data and the installation of Yclas. You are also responsible for the software to work correctly.

Yclas Self-Hosted Lite is a Free Open Source Software (FOSS) available in [GitHub](https://github.com/yclas/yclas), and Self-Hosted Pro is an Open Source.

# Install

**How do you instal the Self-Hosted version?**

Yclas Self-Hosted installation takes *a few minutes.*

You only need a compatible hosting and you will be one step away from installing the software onto your website.

If your hosting provider supports [Softaculous](https://www.softaculous.com/softwares/admanager/Yclas)  (Installer tools that you can access through your Cpanel), the installation process will take just a moment.

If your hosting provider doesn’t support Softaculous don’t worry! Scroll down

  

Start by accessing Softaculous in your Panel and then choose the Yclas Self-Hosted in Ads management. Click on the Installation button.

[Video guide](https://www.youtube.com/watch?v=EjNjkUEJS08) 

## **1 file installation**

Another way to install this version is 1 file installation. Follow the steps one by one:

-   Download  [install-yclas.php](https://raw.githubusercontent.com/yclas/yclas/master/install-yclas.php)
    
-   Upload it to the root of your domain or wherever you want to install Yclas
    
-   Press Download
    
-   Follow the steps that will appear on your screen
    
-   Log in to your Admin Panel, create some Categories and Locations
    
-   You are all ready to start!
    

 [Video Guide](www.youtube.com/watch?v=L2-b8r8DAfU%5D%29) 

**

## Traditional installation

**

The traditional installation is suitable for anyone who wants to use it.

-   [Download](https://yclas.com/self-hosted.html)
    
-   Unpack
    
-   Run the installation in http://yourdomain.com/
    
-   Follow the steps
    
-   Login in Admin Panel, create some Categories and Locations
    
-   You are all ready to start!
    

Note: To install it, you will need a Database and a Username created in your hosting. Follow [this link](https://docs.yclas.com/create-mysql-database) to learn how to create a MySQL Database.

[Video Guide](https://www.youtube.com/watch?v=PLW0qfeWudE) 

**

## Theme Installation

**For 2.x versions**

-   Go to Panel > Appearance > Themes
    
-   Input your license number
    
-   You are ready
    


**Traditional installation**

-   Download the compressed file, either from the link in your e-mail or from your account at our [market](https://selfhosted.yclas.com/oc-panel/profile)
    
-   Uncompress the folder /themes/
    
-   Go to the Admin Panel, area Appearance > Themes and select the theme
    

[Video Guide](https://www.youtube.com/watch?v=u8KbTWoy4jM)


## How to install Yclas Self-Hosted on Digital Ocean, VULTR or Linode

Let’s start by  creating the image / installing server

 

***Introduction***


In this guide we will teach you how to install Yclas Self Hosted in a VPS. We will be covering, [Digital Ocean](https://www.digitalocean.com/?refcode=ebff5f6941b0), [VULTR](https://www.vultr.com/?ref=6814237) and [Linode](https://www.linode.com/). Here are some requirements that you have to cover before proceeding:

***Requirements***

 - Apache 2+



-   PHP 5.6+

-   Short Tags

-   GD support

-   mod_rewrite

-   mcrypt

-   Gettext

-   Curl

-   MySQL 5+

    *We provide guides for you in every step of the way!*

# Guides

For [Digital Ocean](https://www.digitalocean.com/?refcode=ebff5f6941b0)

-   Ubuntu 14.04 Droplet
    
-   Create a non-root user with sudo privileges. You can follow steps 1-4 in the [Initial Server Setup with Ubuntu 14.04](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-14-04/) guide
    

For [VULTR](https://www.vultr.com/?ref=6814237)

Follow  [this guide](https://www.vultr.com/docs/how-to-install-apache-mysql-and-php-on-ubuntu) to install LAMP.

[Linode](https://www.linode.com/)

Follow [this guide](https://www.linode.com/docs/websites/lamp/lamp-server-on-ubuntu-12-04-precise-pangolin) to install LAMP.

[RoseHosting.com](https://www.rosehosting.com/)

Follow  [this guide](https://www.rosehosting.com/blog/how-to-install-open-classifieds-on-a-debian-8-vps/) to install it on Debian or contact their support team and they will install it for free.

# Creating your user Database

In order to install Yclas Self-Hosted, you will need a Database and a Username.

Log in to MySQL with the root account. That’s how it will look:

> mysql -u root -p

The system will prompt you for a password. You can use your MySQL root as a password.

Now, create a database that you’ll use with Yclas. We will call it yclas in the following example.

> CREATE DATABASE yclas;

Next, create a database user and assign a password. You can replace the username ycuser and the password with your own password.

> CREATE USER ycuser@localhost IDENTIFIED BY '_password_';

Next, grant permission to access the database.

> GRANT ALL PRIVILEGES ON yclas.* TO ycuser@localhost;

Now set the new user and then reload the privileges.

> FLUSH PRIVILEGES;

Exit MySQL

> exit

That’s all!
