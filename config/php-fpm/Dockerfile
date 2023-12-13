##FROM php:7.2-fpm
#FROM php:7.4-fpm
##FROM php:8.1-fpm
#
#RUN apt-get update \
#    && apt-get install -y nano curl libpq-dev libxml2-dev \
#    && pecl install redis mongodb \
#    && docker-php-ext-enable redis mongodb \
#    && docker-php-ext-install pdo_pgsql sockets
## Install dependencies
#RUN apt-get update && apt-get install -y \
#    unzip \
#    git \
#    curl
#
#RUN apt-get -y update \
#&& apt-get install -y libicu-dev \
#&& docker-php-ext-configure intl \
#&& docker-php-ext-install intl
#
#RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
#&& composer --version
#
#RUN docker-php-ext-install soap
#
#RUN apt-get install -y \
#        libzip-dev \
#        zip \
#  && docker-php-ext-install zip
#
#RUN docker-php-ext-install sockets
#
#
#
#RUN docker-php-ext-install bcmath
#RUN apt-get update && apt-get install -y \
#        libfreetype6-dev \
#        libjpeg62-turbo-dev \
#        libpng-dev \
#    && docker-php-ext-configure gd --with-freetype --with-jpeg \
#    && docker-php-ext-install -j$(nproc) gd \
#    && docker-php-ext-install mysqli pdo pdo_mysql
#EXPOSE 9000
#
#RUN apt-get install -y locales locales-all
#RUN sed -i '/tr_TR.UTF-8/s/^# //g' /etc/locale.gen && \
#    locale-gen
#ENV LANG tr_TR.UTF-8
#ENV LANGUAGE tr_TR:en
#ENV LC_ALL tr_TR.UTF-8
#
##FROM php:7.2-fpm
##
##RUN apt-get update \
##    && apt-get install -y nano curl libpq-dev libxml2-dev \
##    && pecl install redis mongodb \
##    && docker-php-ext-enable redis mongodb \
##    && docker-php-ext-install pdo_pgsql sockets
### Install dependencies
##RUN apt-get update && apt-get install -y \
##
##    unzip \
##    git \
##    curl
##
##RUN apt-get -y update \
##&& apt-get install -y libicu-dev \
##&& docker-php-ext-configure intl \
##&& docker-php-ext-install intl
##
##RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
##&& composer --version
##
##RUN docker-php-ext-install soap
##
##RUN apt-get install -y \
##        libzip-dev \
##        zip \
##  && docker-php-ext-install zip
##
##RUN docker-php-ext-install sockets
##
##
##
##RUN docker-php-ext-install bcmath
##RUN apt-get update && apt-get install -y \
##        libfreetype6-dev \
##        libjpeg62-turbo-dev \
##        libpng-dev \
##    && docker-php-ext-configure gd  \
##    && docker-php-ext-install -j$(nproc) gd \
##    && docker-php-ext-install mysqli pdo pdo_mysql
##EXPOSE 9000
##
##ENV NODE_VERSION=16.13.0
##RUN apt install -y curl
##RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
##ENV NVM_DIR=/root/.nvm
##RUN . "$NVM_DIR/nvm.sh" && nvm install ${NODE_VERSION}
##RUN . "$NVM_DIR/nvm.sh" && nvm use v${NODE_VERSION}
##RUN . "$NVM_DIR/nvm.sh" && nvm alias default v${NODE_VERSION}
##ENV PATH="/root/.nvm/versions/node/v${NODE_VERSION}/bin/:${PATH}"
##RUN node --version
##RUN npm --version
##
##RUN apt-get install -y locales locales-all
##RUN sed -i '/tr_TR.UTF-8/s/^# //g' /etc/locale.gen && \
##    locale-gen
##ENV LANG tr_TR.UTF-8
##ENV LANGUAGE tr_TR:en
##ENV LC_ALL tr_TR.UTF-8



#FROM php:8.1-fpm
FROM php:7.4-fpm

RUN apt-get update \
    && apt-get install -y nano curl libpq-dev libxml2-dev \
    && pecl install redis mongodb \
    && docker-php-ext-enable redis mongodb \
    && docker-php-ext-install pdo_pgsql sockets
# Install dependencies
RUN apt-get update && apt-get install -y \
    unzip \
    git \
    curl

RUN apt-get -y update \
&& apt-get install -y libicu-dev \
&& docker-php-ext-configure intl \
&& docker-php-ext-install intl

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer \
&& composer --version

RUN docker-php-ext-install soap

RUN apt-get install -y \
        libzip-dev \
        zip \
  && docker-php-ext-install zip

RUN docker-php-ext-install sockets



RUN docker-php-ext-install bcmath
RUN apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng-dev \
    && docker-php-ext-configure gd  \
    && docker-php-ext-install -j$(nproc) gd \
    && docker-php-ext-install mysqli pdo pdo_mysql
EXPOSE 9000

ENV NODE_VERSION=16.13.0
RUN apt install -y curl
RUN curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
ENV NVM_DIR=/root/.nvm
RUN . "$NVM_DIR/nvm.sh" && nvm install ${NODE_VERSION}
RUN . "$NVM_DIR/nvm.sh" && nvm use v${NODE_VERSION}
RUN . "$NVM_DIR/nvm.sh" && nvm alias default v${NODE_VERSION}
ENV PATH="/root/.nvm/versions/node/v${NODE_VERSION}/bin/:${PATH}"
RUN node --version
RUN npm --version

RUN apt-get install -y locales locales-all
RUN sed -i '/tr_TR.UTF-8/s/^# //g' /etc/locale.gen && \
    locale-gen
ENV LANG tr_TR.UTF-8
ENV LANGUAGE tr_TR:en
ENV LC_ALL tr_TR.UTF-8