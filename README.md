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
MYSQL_USER=sistema
MYSQL_PASSWORD=$sistem#@
MYSQL_ROOT_PASSWORD=root

### MYSQL 5.7 #################################################
MYSQLDATA_PATH_HOST_5_7=**where you will save the data**
MYSQL_VERSION_5_7=5.7
MYSQL_CONTAINER_NAME_5_7=mysql5_7
MYSQL_DATABASE_5_7=mysql5_7
MYSQL_PORT_5_7=3207
MYSQL_ROOT_PASSWORD=root
MYSQL_ENTRYPOINT_INITDB_5_7=./docker/mysql_5_7/docker-entrypoint-initdb.d////


### MYSQL 5.6 #################################################
MYSQLDATA_PATH_HOST_5_6=**where you will save the data**
MYSQL_VERSION_5_6=5.6
MYSQL_CONTAINER_NAME_5_6=mysql5_6
MYSQL_DATABASE_5_6=mysql5_6
MYSQL_PORT_5_6=3306
MYSQL_ENTRYPOINT_INITDB_5_6=./docker/mysql_5_6/docker-entrypoint-initdb.d////

### MONGO #################################################
MONGODB_CONTAINER_NAME=mongodb_server_docker
MONGODB_PATH_HOST=**where you will save the data**
MONGODB_PATH_DUMPS_HOST=**where you will make the dumps**
MONGODB_PORT=27017


```

```
docker-compose up -d
```