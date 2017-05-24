FROM ubuntu:16.04
RUN apt-get update &&  apt-get upgrade -y
RUN apt-get install -y apache2
RUN apt-get install -y php7.0-common php7.0-gd php7.0-mcrypt php7.0-curl php7.0-intl php7.0-xsl php7.0-mbstring php7.0-zip php7.0-iconv mysql-client php7.0-cli
RUN a2enmod rewrite
RUN apache2 -v
RUN apt-get install -y libapache2-mod-php
RUN a2enmod php7.0
RUN php -v
RUN apt-get install -y vim
RUN apt-get install -y php7.0-mysql
EXPOSE 80
#VOLUME /home/iedux/Documents/docker/magento/iedux-magento/pub:/var/www/html
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
