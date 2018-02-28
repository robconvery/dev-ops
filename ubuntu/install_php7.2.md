# Installing & Setting up PHP
```
sudo apt-get update
sudo add-apt-repository -y ppa:ondrej/php
sudo apt-get update
sudo apt-get install php7.2-fpm php7.2-cli php7.2-mbstring ...and so on
```

## Installing composer
```
cd ~
curl -sS https://getcomposer.org/installer -o composer-setup.php
sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```
