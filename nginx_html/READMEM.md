[Click Here: Nginx- Docker Official File](https://hub.docker.com/_/nginx)

### Run from command
`sudo docker run --name nginx-html -v /media/code/docker_test/nginx_html:/usr/share/nginx/html -v /media/code/docker_test/nginx_html/html.conf:/etc/nginx/conf.d/default.conf -d -p 8888:8888 nginx`

### Run from Dockerfile
```
sudo docker build -t aldora/nginx-html .
 sudo docker run -p 8888:8888 --name nginx-html -d aldora/nginx-html
```