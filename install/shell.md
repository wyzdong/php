>系统部分
```
sudo apt-get install \
build-essential \
gcc \
g++ \
autoconf \
libiconv-hook-dev \
libmcrypt-dev \
libxml2-dev \
libmysqlclient-dev \
libcurl4-openssl-dev \
libjpeg8-dev \
libpng12-dev \
libfreetype6-dev \
```
>PHP部分
```
cd php-5.6.22/
./configure --prefix=/usr/local/php \
--with-config-file-path=/etc/php \
--enable-fpm \
--enable-pcntl \
--enable-mysqlnd \
--enable-opcache \
--enable-sockets \
--enable-sysvmsg \
--enable-sysvsem \
--enable-sysvshm \
--enable-intl \
--enable-shmop \
--enable-zip \
--enable-soap \
--enable-xml \
--enable-mbstring \
--disable-rpath \
--disable-debug \
--disable-fileinfo \
--with-mysqli=mysqlnd \
--with-pdo-mysql=mysqlnd \
--with-pcre-regex \
--with-iconv \
--with-zlib \
--with-mcrypt \
--with-gd \
--with-openssl \
--with-mhash \
--with-xmlrpc \
--with-curl \
--with-imap-ssl
--enable-maintainer-zts

sudo make
sudo make install
sudo mkdir /etc/php
sudo cp php.ini-development /etc/php/php.ini
```
