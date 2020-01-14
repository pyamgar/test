#Base Image
FROM ubuntu:16.04

#Maintainer
MAINTAINER Popat

#Apt-get Repo
RUN apt-get update

#Install Apache Packages
RUN apt-get install apache2 -y

#Copy the code inside container
COPY index.html /var/www/html/index

#EXPOSE
EXPOSE 80

#Start Apache service
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]
