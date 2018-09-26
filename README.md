# FullStack Nanodegree Project 6 - Linux Server Configuration

## SSH access:
  - IP : 35.178.140.208
  - ssh port : 2200
  - download the key file (udacityGrader) from this repository
  - connect with : ssh grader@35.178.140.208 -p 2200 -i udacityGrader
  - (use the following passphrase: grader123 )
  
  
## The web application URL
~~http://35.178.140.208/~~


## Additional software installed:
  - Apache2
  - PostgreSQL
  - Python 2
  - Python packages: 
    - WSGI adapter module for Apache (libapache2-mod-wsgi)
    - Flask
    - SQLAlchemy
    - requests
    - httplib2
    - oauth2client


## Configuration changes made:
  - updated and upgraded all packages
  - added user grader and provided sudo access in sudoers.d
  - Disabled remote root login in sshd_config
  - Disabled password-based login
  - RSA key auth enabled
  - Changed the SSH port to 2200 in sshd_config
  - Configured UFW firewall to allow ports 
    - 123 (NTP)
    - 2200 (SSH - custom)
    - 80 (HTTP)
  - Setup WSGI application including: 
    - PostgreSQL database server (database in use by app: bookcatalog)
    - Flask application
    - Apache2 server
  
  
## List of any third-party resources made use of to complete this project:
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-16-04
https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
https://www.digitalocean.com/community/tutorials/how-to-install-linux-apache-mysql-php-lamp-stack-on-ubuntu-14-04
https://www.postgresql.org/docs/


