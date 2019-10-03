## NGINX quick conf test ##

## Start container ##
```docker-compose up -d```

## Stop container ##
```docker-compose down```

## Restart container ##
```docker-compose restart```

1. Do modification to default.conf
2. Test changes - run ```docker container exec nginx nginx -t```
3. Apply changes - rn ```docker container exec nginx nginx  -s reload```
4. Or just restart container



Just for fun:
```docker container exec {container name} nginx -t```

[Docker exec manual](https://docs.docker.com/engine/reference/commandline/exec/)