[Click Here: PHP- Docker Official File](https://hub.docker.com/_/php)

### Run from command
`sudo docker run --name php -v "$PWD":/usr/src/myapp -w /usr/src/myapp php:7.4-cli php docker.php`

### Run from Dockerfile
```
 sudo docker build -t aldora/php .
 sudo docker run --name php aldora/php
```