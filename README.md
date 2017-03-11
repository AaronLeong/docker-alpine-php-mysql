## Package Included
- nginx (1.8.0)
- php-fpm (5.6.15)
- mysql (mariadb 10.1.8)

## RUN

```
docker run -d \
  --name nginx-php-mysql \
  -p 80:80 \
  -v $PWD/data:/var/lib/mysql \
  -v $PWD/logs:/data/logs \
  -v $PWD:/data/htdocs \
  cutec/docker-alpine-php-mysql
```
