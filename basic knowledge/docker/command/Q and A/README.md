# Q and A about Docker 
## How to export all images to local machine through command?
### A
One solution as follows.

![image](https://github.com/40843245/Docker/assets/75050655/e5f88bf5-e324-4b16-a7b0-0c3a2efe7276)

### Ref
https://stackoverflow.com/questions/35575674/how-to-save-all-docker-images-and-copy-to-another-machine

## How to export a container to local machine through command?
### A
Use 
      
      docker container export 
or its alias

      docker export

Such as:
      
      docker container export "bfdf06879f4c" > "mariadb.tar"

### Ref
From Docker docs,

https://docs.docker.com/reference/cli/docker/container/export/
