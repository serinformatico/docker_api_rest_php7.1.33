FROM php:7.1-fpm

# Instalación de apps
RUN apt-get update && apt-get install -y \
	bash vim sed

# Instalación de composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Instalación de xdebug
RUN pecl install xdebug-2.9.8 && docker-php-ext-enable xdebug

# Configuración de PHP (agrega el archivo al directorio de PHP)
ADD ./php/php.ini /usr/local/etc/php/