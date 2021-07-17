# CHANGE PHP VERSION
#### Follow the steps described below

### 1: add the PPA maintained by Ondrej Surý
```
sudo add-apt-repository ppa:ondrej/php
```
### 2: update the system
```
sudo apt update
```
###3: install PHP versions 7.2
```
sudo apt install php7.2
```
### 4: Select the standard version of PHP
```
sudo update-alternatives --set php /usr/bin/php7.2
```
### 5: Disable version 7.4 or the one you are using
```
sudo a2dismod php7.4
```
### 6: enable version 7.2
```
sudo a2enmod php7.2
```
### 7: Restart the apache server
```
sudo systemctl restart apache2
```
##### That's it!
