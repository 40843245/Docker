# phpmyadmin
# intro
phpmyadmin is a system to manage mysql database using apache2 server.

NOTE that 

<p style='color:red;'><b>phpmyadmin is NOT a server!!!</b></p>

<b>phpmyadmin is NOT a server!!!</b>

<b>phpmyadmin is NOT a server!!!</b>

## Default path
### Default root directory for file

It is defined in the configuration file. 

      /etc/apache2/apach2.conf
      
https://askubuntu.com/questions/193465/setting-path-for-apache

The default root directory defined in apach2.conf is 

    /var/www/html
    
### Default path for url
Suppose that you use <b>apache2 server</b> in <b>Docker</b>.

If you want to visit the webpage, 

then you should enter the following url in the url search box.

     http://<host>[::<port>]?[/<path>[#<fragment>]?]?
     
where 

      the syntax applies to the regular expression. 
     
      <host> refers your host name of the server.
      
      <port> determines the port the server used.
      
      <path> refers the path of the file
      
      <path> determines what file to be redirected.
      
      <path> <part_path>[/<part_path>]*
      
      <part_path> [A-Za-z]([A-za-z0-9_])*
      
      <fragment> refers the part of the url to be redirected.
      
 For example.
 
      Suppose the root directory is /var/www/html, the host of server name is 'localhost' , and the port is 80.
      
      If you want to visit the webpage which its url is 
            
       /var/www/html/Docker/docker_1.html
       
       Then you should enter the following url in the search box.
       
       http://localhost::80/Docker/docker_1.html
       
       
## Recall 
### Recall for regular expression
            
            1. []
                  The group of lots of elem, it can also be used with - .
            2. ()
                  The group of lots of elem, it can NOT be used with - .
            
            3. * 
                  0, 1 or, many times.
            
            4. ? 
                  0 or 1 times.
             
            
    
      
      

