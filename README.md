# Shipping
This is a docker image that contains a basic LAMP stack.

The images used are:
  - php:7-apache
  - mysql:5.7
  - phpmyadmin/phpmyadmin

It is recommended to also install a monitoring service like Portainer to monitor the containers.
  
  Portainer can be installed with the following command:
    $ docker volume create portainer_data
  
  Portainer can be started with the following command:
    $ docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer
