# Devops challenge

The objective of this challenge is to create a container that uses ubuntu as a base image, installs an HTTPD (apache2) server and edits the index.html file. 

## Build the image
```
docker build . -f dockerfile
```

## Run the container
```
docker run --name test -it ubuntu
```