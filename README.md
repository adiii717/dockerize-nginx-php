# dockerize-nginx-php
Run Nginx and PHP docker container with docker-compose as separate container

## One process per container !
Base on `one process per container` this repo deal with one of the common issue by running two process `Nginx+PHP` in the same Docker container, it will start two containers

- PHP
- Nginx

Both container will share same volume `app/`, and Nginx will use docker compose network to connect and interparate with PHP.

## To run the container
```
git clone https://github.com/Adiii717/dockerize-nginx-php.git
cd dockerize-nginx-php;
docker-compose up
```

Now open the browser

http://localhost/helloworld.php

Or 

http://localhost/

To viw your PHP Info or Helloworld file.
