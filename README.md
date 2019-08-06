# DOCKER DATABASES


## Prerequisites

- Docker https://docs.docker.com/install/



## Installing
1. Go to the dir where you cloned the project
2. Create the .env file with your settings
3. Run the command docker-compose up -d

##### .env sample
```
### Timezone ###############################################
TZ=America/Bahia

### MYSQL #################################################
MYSQLDATA_PATH_HOST= **where you will save the data**
MYSQL_VERSION=5.7
MYSQL_CONTAINER_NAME=mysql5_7
MYSQL_DATABASE=mysql5_7
MYSQL_USER=sistema
MYSQL_PASSWORD=$sistem#@
MYSQL_PORT=3207
MYSQL_ROOT_PASSWORD=root
MYSQL_ENTRYPOINT_INITDB=./docker/mysql/docker-entrypoint-initdb.d////

### MONGO #################################################
MONGODB_CONTAINER_NAME=mongodb_server_docker
MONGODB_PATH_HOST= _where you will save the data_
MONGODB_PATH_DUMPS_HOST= **where you will make the dumps**
MONGODB_PORT=27017
```

```
docker-compose up -d
```