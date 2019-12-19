# FSND_03
Udacity FullStack Nano Degree - Project 3 , Linux Server Configuration
i. The IP address and SSH port so your server can be accessed by the reviewer:
  3.214.76.20:2200
ii. The complete URL to your hosted web application.
  http://3.214.76.20.xip.io
iii. A summary of software you installed and configuration changes made.
  Updated all outdates initial packages provided by the default ubuntu distro provided over aws lightsail.
  sudo ufw allow 2200/tcp          # Allow incoming tcp packets on port 2200.
  sudo ufw allow www               # Allow HTTP traffic in.
  sudo ufw allow 123/udp           # Allow incoming udp packets on port 123.
  sudo ufw deny 22                 # Deny tcp and udp packets on port 53.
  Installed fail2ban to ban attackers, setup bantime, notification email and allowed port
  setup unattended-upgrades to automatically install upgraded packages
  
  created grader user with root access , grader password = graderpass
  installed apache with  mod_wsgi application
  installed and configured PostgreSQL
  installed git and pulled down catalog project from git
  installed dependecies in virtual host environment
  disabled the default apache site
  updated google oauth for new site/config
  
 
iv. A list of any third-party resources you made use of to complete this project.
  git
  flask
  sqlalchemy
  google oauth
  postgresql
  psycopg2
  apache
