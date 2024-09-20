# Utiliser une image de base PHP
FROM php:7.3-apache

RUN apt-get update -y && \
apt-get install -y unzip wget mariadb-client && \
rm -rf /var/lib/apt/lists/*; 

# Installer mysqli
RUN docker-php-ext-install mysqli

# Copier les fichiers de PMB dans le conteneur
COPY ./pmb/ /var/www/html/

# Configurer les permissions
RUN chown -R www-data:www-data /var/www/html/

CMD ["apache2-foreground"]
