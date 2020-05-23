# Install Apache to check from web browser using 0.0.0.0 or localhost, check version, start,stop & restart Apache into Ubuntu
```
sudo apt update
sudo apt upgrade
sudo apt install apache2
apache2 -v
sudo service apache2 start
sudo systemctl enable apache2
sudo service apache2 stop
sudo service apache2 start
sudo service apache2 restart 
```
Visit:  http://localhost/


# Install MySQL & check version, start,stop & restart Apache
```
sudo apt install mysql-server
sudo mysql_secure_installation
mysql --version
sudo service mysql start
sudo service mysql enable
sudo service mysql start
sudo service mysql restart
```

# Create MySQL DB, User
```
sudo mysql -u root -p
CREATE DATABASE school DEFAULT CHARACTER SET utf8 COLLATE utf8_unicode_ci;
GRANT ALL ON school.* TO 'trainee'@'localhost' IDENTIFIED BY 'Da@y=001';
FLUSH PRIVILEGES;
EXIT;
```

# Install PHP & check version 
```
sudo apt install php-pear php-fpm php-dev php-zip php-curl php-xmlrpc php-gd php-mysql php-mbstring php-xml libapache2-mod-php
php --version
```

# Install PHPmyAdmin
```
sudo apt update 
sudo apt install phpmyadmin php-mbstring php-gettext
# sudo nano /etc/apache2/apache2.conf
# Then add the following line to the end of the file:
# Include /etc/phpmyadmin/apache.conf
# Then restart apache:
sudo service apache2 restart 
```
visit: http://localhost/phpmyadmin/
