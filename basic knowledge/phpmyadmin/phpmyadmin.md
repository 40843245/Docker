# phpmyadmin
# intro
phpmyadmin is a system to manage mysql database using apache2 server.

NOTE that 

<p style='color:red;'><b>phpmyadmin is NOT a server!!!</b></p>

<b>phpmyadmin is NOT a server!!!</b>

<b>phpmyadmin is NOT a server!!!</b>

## Default path
### Default path for file

It is defined in the configuration file. 

      /etc/apache2/apach2.conf
      
https://askubuntu.com/questions/193465/setting-path-for-apache

The default path defined in apach2.conf is 

    /var/www/html
    
### Default path for url
Suppose that you use <b>apache2 server</b> in <b>Docker</b>.

If you want to visit the webpage, 

then you should enter the following url in the url search box.

     http://<host>[::<port>][/<path>[#<fragment>]]

