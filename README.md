# docker-cartodb-nginx
nginx container configured with [cartodb.nginx.proxy.conf](https://github.com/spawnthink/docker-cartodb-nginx/blob/master/cartodb.nginx.proxy.conf) which is based on config file from [sverhoeven/docker-cartodb](https://github.com/sverhoeven/docker-cartodb/blob/master/config/cartodb.nginx.proxy.conf) with few modifications.

Note: You have to link your cartodb container as cartodb.localhost

## build 
docker-compose build

```console
git clone https://github.com/vpac-innovations/docker-cartodb-nginx.git
cd docker-cartodb-nginx
git clone https://github.com/vpac-innovations/docker-cartodb.git
git clone https://github.com/vpac-innovations/docker-mapproxy.git
git clone https://github.com/vpac-innovations/docker-postgis.git
```
