FROM php:8.0-apache

# Install necessary PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql

# Enable Apache mod_rewrite
RUN a2enmod rewrite

# Set the document root
ENV APACHE_DOCUMENT_ROOT /var/www/html/src

# Copy the PHP source code into the container
COPY ../src /var/www/html/src

# Set permissions
RUN chown -R www-data:www-data /var/www/html/src

EXPOSE 80