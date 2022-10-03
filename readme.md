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

## How does it work?
1. The ubuntu image is referenced as the base image with the FROM command
2. Dependencies are updated so apache can be installed
3. Apache2 web server is installed
4. The working directory is changed to the html folder for when the user enters the container
5. index.html is copied and named to index2.html
6. index2.html is edited