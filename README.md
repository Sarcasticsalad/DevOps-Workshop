# php-hello-world
A simple hello-world for composer

Installation using Dockerfile
------------
Build Docker Image
``` 
docker build -t workshop .
```
Run Docker Image
``` bash
docker run -dp 0.0.0.0:8080:80 workshop
```

Installation using docker-compose.yml
------------

Build and run Docker Image
``` bash
docker-compose up -d
```

Install with composer
``` bash
composer require silarhi/hello-world
```

Run composer update
``` bash
composer update silarhi/hello-world
```

Usage
-----

``` php
require_once __DIR__ . '/vendor/autoload.php';

use Silarhi\Hello;

$hello = new Hello();
echo $hello->display() . "\n";
```
