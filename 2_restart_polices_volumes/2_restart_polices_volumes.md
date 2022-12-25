## 2. Restart Polices, Volumes, ENV

### Restart Polices 
* no (default)
* on-failure
* unless-stopped
* always

### volumes

`docker container run -dt --name mynginx -v /root/index:/usr/share/nginx/html nginx`

`docker container run -dt --name mynginx -v MyVolume:/usr/share/nginx/html nginx`

`docker container run -dt --name mynginx --mount type=bind,source=/root/index,target=/usr/share/nginx/html nginx`

`docker volume create --name demo-earthly`
## Docker simple commands
* --restart no ...
* docker system df
* docker system df -v
* docker run --env var1=value
* docker save myapp > myapp.tar
* docker load < myapp.tar
* docker history image_name


## DockerFile simple commands
* ENV var 1.3
* VOLUME /usr/share/nginx/html
