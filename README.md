# docker-cartodb-nginx
nginx container configured with [cartodb.nginx.proxy.conf](https://github.com/spawnthink/docker-cartodb-nginx/blob/master/cartodb.nginx.proxy.conf) which is based on config file from [sverhoeven/docker-cartodb](https://github.com/sverhoeven/docker-cartodb/blob/master/config/cartodb.nginx.proxy.conf) with few modifications.

Note: You have to link your cartodb container as cartodb.localhost

```console
git clone https://github.com/vpac-innovations/docker-cartodb-nginx.git
cd docker-cartodb-nginx
git clone https://github.com/vpac-innovations/docker-cartodb.git
git clone https://github.com/vpac-innovations/docker-mapproxy.git
git clone https://github.com/vpac-innovations/docker-postgis.git
```

### cartodb source code is need to change fixit 
```bash
cd docker-cartodb
git clone https://github.com/vpac-innovations/cartodb.git
cd ..
cd docker-postgis
git clone https://github.com/vpac-innovations/cartodb.git
```

## change config files on ~/docker-cartodb-nginx/docker-cartodb/config/
### app_config.yml
 - setting mapproxy service
 - database settings
 - cartodb SQL api service settings

## database.yml
 - config database location


### execute docker compose
```
docker-compose build
docker-compose up -d
```