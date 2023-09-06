# Dockerfile
FROM php:fpm-alpine
# Utilise une petite image

RUN apk update; \
    apk upgrade;
# Mets a jour le serveur

#install mysqli
RUN docker-php-ext-install mysqli
