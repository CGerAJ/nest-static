docker volume create nest-static-mysql-vol

docker run --name nest-static-mysql \
 --restart=always \
 -v nest-static-mysql-vol:/var/lib/mysql \
 -p 3306:3306 \
 -e MYSQL_ROOT_PASSWORD=my_root_password \
 -e MYSQL_DATABASE=nest-static \
 -e MYSQL_USER=CGerAJ \
 -e MYSQL_PASSWORD=3dgrgeeDF3rerf3ww \
 -d mysql
