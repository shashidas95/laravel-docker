# Use an official PHP runtime as a base image
FROM php:8.2-fpm

# Install dependencies
RUN apt-get update && apt-get install -y \
    libzip-dev \
    unzip \
    git \
    && docker-php-ext-install zip pdo pdo_mysql

# # Install Composer
 #RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# # Copy composer.json and composer.lock
 # COPY composer.json composer.lock ./

# # Install application dependencies
 #RUN composer install --no-scripts --no-autoloader

# # Copy the rest of the application code
 #COPY . .

# # Generate autoloader
 #RUN composer dump-autoload --optimize

# # Set permissions
# RUN chown -R www-data:www-data /var/www/html/storage /var/www/html/bootstrap/cache

# # Expose port 9000 and start php-fpm server
 #EXPOSE 9000
 #CMD ["php-fpm"]

