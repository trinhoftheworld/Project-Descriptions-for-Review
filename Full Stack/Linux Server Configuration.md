![Project Roadmap](http://i.imgur.com/S1VH83A.jpg)

##Project Overview
You will take a baseline installation of a Linux distribution on a virtual machine and prepare it to host your web applications, to include installing updates, securing it from a number of attack vectors and installing/configuring web and database servers.

##Why this project?
A deep understanding of exactly what your web applications are doing, how they are hosted, and the interactions between multiple systems are what define you as a Full Stack Web Developer. In this project, you’ll be responsible for turning a brand-new, bare bones, Linux server into the secure and efficient web application host your applications need.

##What will I learn?
You will learn how to access, secure and perform the initial configuration of a bare-bones Linux server. You will then learn how to install and configure a web and database server and actually host a web application.

##How does this help my career?
* Deploying your web applications to a publicly accessible server is the first step in getting users
* Properly securing your application ensures your application remains stable and that your user’s data is safe

##How will I complete this project?

1. Launch your Virtual Machine with your [Udacity account](https://www.udacity.com/account#!/development_environment)
2. Follow the instructions provided to SSH into your server
3. Create a new user named `grader`
4. Give the `grader` the permission to sudo
5. Update all currently installed packages
6. Change the SSH port from 22 to 2200
7. Configure the Universal Firewall to only allow incoming connections for SSH (port 2200), HTTP (port 80), and NTP (port 123)
8. Configure the local time zone to UTC
9. Install and configure Apache to serve a Python mod_wsgi application
10. Install and configure PostgreSQL:
* Do not allow remote connections
* Create a new user named `catalog` that has limited permissions to your catalog application database
11. Install git, clone and setup your Catalog App project (from your GitHub repository from earlier in the Nanodegree program) so that it functions correctly when visiting your server’s IP address in a browser. Remember to set this up appropriately so that your .git directory is not publicly accessible via a browser!

##Evaluation
Your project will be evaluated by a Udacity Code Reviewer according to the rubric below. Be sure to review it thoroughly before you submit. All criteria must "meet specifications" in order to pass.

![Project Rubric](http://i.imgur.com/DCax9jH.png)
