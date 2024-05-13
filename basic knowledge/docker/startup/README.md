# Docker
## installation 
For the installation, see the Official Docs, or my attachments in this repo at Github.

## start your first project on Docker
### upload file to Docker container
For fully understand, I will take my first project as an example.

Suppose I have a Docker container where
container's id:0e1066ed12fc

Now, I want to upload a folder name "nfu" to the Docker container. 

First, I have to change directory by CD command.
Then, I have to type these command on DOS cmd prompt (NOT on Docker's cmd prompt).

docker cp "nfu" "0e1066ed12fc:/var/www/html"

NOTICE that 
1. The destionation path (i.e. the path of file or file in Docker container) must start with Docker container's id. Can NOT start with Docker container's name.
2. The ':' symbol must be followed by the Docker container's id. It's syntax.
3. After ':' symbol, 'var/www/html/' must be followed.
4. There are two different syntax. For more, see official Docs or my notes "docker/cp.md" at Github.

Conclude 1th to 4th points, there are two different syntax.

    docker cp "<src_path>" "<dest_path>"

or

    docker cp "<dest_path>" "<src_path>"

Here

    <src_path> :=
        The source path that contains the file that will be uploaded, or the file that will be upload.
        It can be either a folder or a file.
    
    <dest_path> := <container_id>:/var/www/html/<rest_dest_path>

    <container_id> := 
          The id of Docker container that you want to upload to.

    <rest_dest_path> :=
          Any directory that you want to upload to. It can NOT be a file name. It only can be a folder.
          
### url that links to file on Docker container
Let's continue the example.

After uploading the folder, 

suppose there is a file named 'test1.php' in the path '/var/www/html/nfu/course/5th/DBMS/final_project/php' in Docker,

and the hostname of Docker container is 'localhost', while the port of that is '8763'.

To look at result of 'test1.php', one has to open internet browser (I recommend NOT to open the browser that is obsolete such as IE.) 

Then type the url in the url bar.

    http://localhost:8763/nfu/course/5th/DBMS/final_project/php/test1.php

If you can see the result of your code instead of the error message (such as 404 NOT found.) looks as following figure, then you're done.

![image](https://github.com/40843245/Docker/assets/75050655/cd663761-d9de-4389-8841-1401c0fb946b)



