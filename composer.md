```composer install```

``` composer clear-cache ``` <br>
``` composer require rxmg/warehouse-resources:dev-master ``` <br>
``` composer require rxmg/warehouse-resources:dev-develop ``` <br>

* use composer install for first install
* use composer require to add a new package OR UPDATE A PACKAGE 
* use composer update for some reason?
* can view composer branches available in packagist or private packagist(right hand side)
* composer update package:branch appears to change all dependencies as well, so even if already installed, use composer install package:branch


### Troubleshooting
-----
* run composer install -vvv or composer update -vvv to get more info 
* user profile global composer files located at ~/.config/composer or ~/.composer
* can delete the ~/.composer/cache/files to reset the composer cache
* delete vendor, composer.lock files/directories
* composer config --global --list to see all of the global composer keys
* composer clear-cache/composer dumpautoload
* composer install --prefer-dist
```
Oh, I see, you are installing dev-master so it defaults to cloning the repository which happens from GitHub only. If you want it to download a zip file from Packagist for a branch, you need to specify the option --prefer-dist on the composer command
```



### Private Packagist
-----
* deploy key in composer global
* COMPOSER_AUTH variable
* composer addition to composer.json file

