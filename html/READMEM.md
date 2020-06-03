`sudo docker run --name nginx-html -v /media/code/docker_test/html:/usr/share/nginx/html -v /media/code/docker_test/html/html.conf:/etc/nginx/conf.d/default.conf -d -p 8888:8888 nginx`


```
sudo docker build -t aldora/nginx-html .
 sudo docker run -p 8888:8888 --name nginx-html -d aldora/nginx-html
```