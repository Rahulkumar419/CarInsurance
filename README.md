# CarInsurance
Project to learn how to build a html website application using docker.

# Points

Docker is way of packaging the application.
For any application to run, what all things you need
 -> Server
 -> OS
 -> Dependencies
 -> Framework
 -> Runtime
When we use docker it just uses :
  -> Dependencies
  -> Framework
  -> Runtime
Docker is use abstraction of OS kernel.
that means it use the file capability of OS, memory management capability of OS etc.

To use the readymade image of the Docker from Docker hub (webserver of apache)
Create the Dockerfile for your html application.
FROM httpd // Download the webserver from docker hun
COPY . /usr/local/apache2/htdocs/ // Copy from the current directory to /usr/local/apache2/htdocs/

Build the container image 

docker build -t carinsurence . // make sure you use the '.'

To see image created 
docker image ls

If you find any error use the below command
& 'c:\program files\Docker\Docker\DockerCli.exe' -switchdeamon

Run the contgainer 
docker run -itd -p 80:80 --name carinsurence carinsurence


  



