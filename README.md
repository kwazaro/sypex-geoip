GeoIP PHP library for Sypex GeoIP database
========================================
This library uses Sypex GeoCity database by default.

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist kwazaro/sypex-geoip "@dev"
```

or add

```
"kwazaro/sypex-geoip": "@dev"
```

to the require section of your `composer.json` file.


Usage
-----

Once the library is installed, simply use it in your code by  :

```php
<?php
use kwazaro\sypexgeoip\Geoip;

$geo = new Geoip();

$data = $geo->get('xxx.xxx.xxx.xxx');

$country = $geo->getCountry('xxx.xxx.xxx.xxx');

$vity = $geo->getCity('xxx.xxx.xxx.xxx');

$fullInfo = $geo->getCityFull('xxx.xxx.xxx.xxx');