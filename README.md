## NGINX quick conf test ##

### Start container ###
```docker-compose up -d```

### Stop container ###
```docker-compose down```

### Restart container ###
```docker-compose restart```

### Know how: ###
1. Do modification to default.conf
2. Test changes - run ```docker container exec nginx nginx -t```
3. Apply changes - run ```docker container exec nginx nginx  -s reload```
4. Or just restart container

### html/.htapswd for basic auth test ###
user/user

### self-assigned certificate for 443
* html/nginx-selfsigned.crt
* html/nginx-selfsigned.key

### Just for fun: ###
```docker container exec {container name} nginx -t```

[Docker exec manual](https://docs.docker.com/engine/reference/commandline/exec/)

### Ports 80 and 443 available ###
Listen on 80 and 443