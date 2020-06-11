`sudo docker run --name php-nginx -v "$PWD":/usr/share/nginx/html -v "$PWD"/http.conf:/etc/nginx/nginx.conf -v "$PWD"/nginx.conf:/etc/nginx/conf.d/default.conf -d -p 8888:8888 nginx`

`sudo docker exec -it php-fpm sh`
`sudo docker cp php-fpm:/usr/local/etc/php/php.ini-development ./php.ini-development`
`docker cp tmp-nginx-container:/etc/nginx/nginx.conf /host/path/nginx.conf`

`sudo docker run --name php-fpm -v "$PWD":/var/www/html -P -d php:7.2-fpm-alpine`