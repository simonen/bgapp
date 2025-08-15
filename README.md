MyBGApp Project

```docker network create --driver bridge app-network```

```docker run -d --net app-network --name db -e MYSQL_ROOT_PASSWORD=Pass img-db```

```docker run -d --net app-network --name web -p 8080:80 -v $(pwd)/web:/var/www/html img-web```
