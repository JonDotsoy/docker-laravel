# Docker file to Laravel Docker
FROM  php:5.6-apache
MAINTAINER Jon Dotsoy <hi@jon.soy> (http://jon.soy/)

# Get Composer
RUN echo "Install Composer" && cd /bin && php -r "readfile('https://getcomposer.org/installer');" | php -- --install-dir=/bin --filename=composer

# RUN cd /bin && ls -la | grep composer

# Install Git
RUN echo "Update (apt-get)" && apt-get update
RUN echo "Install Git" && apt-get install git -y

# Install Laravel Installer
# RUN echo "Install Laravel" && composer global require "laravel/installer=~1.1"

# Zip dependences
RUN echo "Zip Archive" && apt-get install -y zlib1g-dev && docker-php-ext-install zip
RUN echo "mbstring bcmath" && docker-php-ext-install bcmath mbstring
RUN echo "Libmcrypt-dev" && apt-get install -y libmcrypt-dev
RUN echo "mcrypt" && docker-php-ext-install mcrypt

# Add Bin Composer in PATH
ENV PATH ${PATH}:~/.composer/vendor/bin

# RUN laravel DemoProject
# ~/.composer/vendor/bin/laravel new html -n
RUN echo "New Demo project" && cd /var/www && rm -r /var/www/html && composer create-project laravel/laravel /var/www/html "4.2.11" --prefer-dist

WORKDIR /var/www/html/public

RUN chmod -R 777 /var/www/html/app/storage

# Change public folder
# /etc/apache2/sites-available/000-default.conf
RUN sed -i -e 's/DocumentRoot\ \/var\/www\/html/DocumentRoot\ \/var\/www\/html\/public/g' /etc/apache2/apache2.conf
# RUN sed -i -e 's/DocumentRoot\ \/var\/www\/html/DocumentRoot\ \/var\/www\/html\/public/g' /etc/apache2/sites-available/000-default.conf
# cat /etc/apache2/sites-available/000-default.conf /var/www/html/public
# /var/www/html/public
# apache2.conf

EXPOSE 80
