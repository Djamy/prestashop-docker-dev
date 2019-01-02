#Docker run syntax
Need to build image then,
`docker run prestadev --add-host=docker.host:192.168.0.2`

#Compose syntax
```yml
php:
    build: ./1.6
    volumes:
        - ./www:/var/www/html:cached
    links:
        - some-db
    extra_hosts:
        - "docker.host:192.168.0.2"
```
