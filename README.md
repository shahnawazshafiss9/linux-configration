# system setup first time
 

1. Go to the this path  etc/apach2/apache2.conf and replace the below codes 

<Directory /var/www/> 

Options Indexes FollowSymLinks 

AllowOverride All 

Require all granted 

</Directory> 

2. Go to the this path  etc/apach2/sites-available/000-default.conf and replace the below codes 

<Directory /var/www/html> 

        		Options Indexes FollowSymLinks 

        		AllowOverride All 

        		Require all granted 

        	</Directory> 

3. It’s mandatory to run this command which is given below 

sudo a2enmod rewrite 

sudo systemctl restart apache2 

4. It’s also mandatory to access the path /var/www/html/ and give to the permission read/write below mentioned command. 

sudo chmod –R 777 foldername/ 

 

 

 
