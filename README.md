# IIEC_Docker_Dynamic_Web
# Develope a Dynamic Website or blog Using Mysql and Wordpress
  This  Project is based on creating a dynamic website and blog using Mysql and Wordpress.
In this project there we adopt the docker compose infrastucture technology.
Integrating all the configuration,creation and management usind docker-compose infrastructure.

# What is Docker ?
Docker is a set of platform as a service products that uses OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels

# Configuration of Docker
  -For getting a docker on your linux system, you have to create a one repo file in following way
  
    - change a directory  cd /etc/yum.repos.d/
    - create a one file   vim docker.repo
    - in that file put the following text.
      - [docker]
        baseurl=https://download.docker.com/linux/centos/7/x86_64/stable/
        gpgcheck=0
    - after putting the above content in that file ,save that file 
    -and run following command
    - yum install docker-ce
    -systemctl enable docker

- For requirement of developer docker creates an appropriate environment using image file.Image file is look like an iso file that has limited bundle of resources that necessary for developer.You can download the image file with the following syntax

  -docker pull imageFileName
  
 For this project i have got two image one is mysql and another one is wordpress that are get with following command
  For MySql Image File
   -docker pull mysql:5.7
  
  For Wordpress Image file
  - docker pull wordpress:5.1.1-php7.3-apache"

-You can test the database procedure y should have the client side mysql,that can be pull like:
    yum install mysql

# what is Docker-Compose 
-Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application's services. Then, with a single command, you create and start all the services from your configuration. ... Run docker-compose up and Compose starts and runs your entire app

- Using docker compose we run the both wordpress and mysql container.
- it saves a lot of time, human work for making a whole infrastucture.


# References

  -https://www.youtube.com/watch?v=-lpDRE3Fcj0
  -http://www.linuxworldindia.org/
  -https://docs.docker.com/compose/
  -https://en.wikipedia.org/wiki/Docker_(software)
