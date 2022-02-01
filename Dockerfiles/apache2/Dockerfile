#Dockerfile to build Docker Image Of ApacheServer running on Ubuntu
#Made by Arystanbek Muzdakhanov 
FROM ubuntu:18.04 
RUN apt-get update 
RUN apt-get install -y apache2 
RUN echo  'GREETING FROM DOCKER!' > /var/www/index.html	
CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]
EXPOSE 80

