# tgitcrash

## Crash tgitcache on windows 7 x64

### Instructions

1) clone this repo and install php 7.1.3 or better
2) run the following command to install composer in this directory. From https://getcomposer.org/download/.

```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```

3) run ./composer.phar update
4) run ./composer.phar --prefer-lowest update
5) goto 2 and cycle through untill crash