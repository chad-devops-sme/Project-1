
I just created my Frist Linux Server in AWS!!

![apt update](Images/AWS-Linux-Server.jpg)



# WEB STACK IMPLEMENTATION (LAMP) ON AWS
A technology stack is a set of frameworks and tools used to develop a software product. This set of frameworks and tools are very specifically chosen to work together in creating a well-functioning software. some examples are…

1. **LAMP** (Linux, Apache, MySQL, PHP, Python, or Perl)
2. **LEMP** (Linux, Nginx, MySQL, PHP or Python, or Perl)
3. **MERN** (MongoDB, ExpressJS, ReactJS, NodeJS)
4. **MEAN** (MongoDB, ExpressJS, AngularJS, NodeJS

## STEP 1 - Installing Apache and Updating the Firewall

sudo apt update

![apt update](Images/sudo-apt-update.jpg)

sudo apt install apache2

![apt install](Images/sudo-apt-install-apache2.jpg)


sudo systemctl status apache2** 

![apache2 status](Images/sudo-systemctl-status-apache2.jpg)


Open Tcp Port 80 

![tcp port 80](Images/open-tcp-port80.jpg)


Now the Apache webserver is install and can access via port 80


![apache2 default page](Images/Apache2-Ubuntu-Default-Page.jpg)









## STEP 2 - Installing MySQL 

Now that you have a web server up and running, you need to install a Database Management System (DBMS) to be able to store and manage data for your site in a relational database. MySQL is a popular relational database management system used within PHP environments.


sudo apt install mysql-server

![mysql install](Images/sudo-apt-install-mysql-server.jpg)

sudo mysql

![mysql](Images/sudo-mysql.jpg)


sudo mysql_secure_installation

![mysql](Images/sudo-mysql_secure_installation.jpg)


sudo mysql -p

![mysql](Images/sudo-mysql-p.jpg)


## Step 3 — Installing PHP 

sudo apt install php libapache2-mod-php php-mysql


![Install php](Images/sudo-apt-install-php.jpg)


php-v  Checking the version of php


![checking version](Images/php-v.jpg)


## Step 4 — Create a Vitural Host

sudo mkdir

![checking version](Images/sudo-mkdir.jpg)

sudo chown

![checking version](Images/sudo-chown.jpg)

sudo vi 

![checking version](Images/sudo-vi.jpg)

sudo ls /etc/apache2/sites-available

![checking version](Images/sudo-ls.jpg)

sudo a2ensite projectlamp

![checking version](Images/sudo-a2ensite.jpg)







Step 5 — Enable PHP 

sudo vim
![checking version](Images/sudo-vim.jpg)


sudo systemctl reload apache2


PHP site

![checking version](Images/php-site.jpg)