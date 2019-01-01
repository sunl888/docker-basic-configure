# docker-basic-configure
docker 基礎配置

## 安装
   1. 使用 `docker network create app_net` 创建一个内部网络
   2. 在对应的目录使用 `dokcer-compose up -d` 即可创建对应服务

## Minio
 访问`minio`: http://localhost:9000

## Mysql
 - 在`docker`内部直接使用 `Host: mysql` 就可以连接`mysql`服务了
 - 访问`phpMyAdmin`: http://localhost:8081
 
## Nginx 
 - 复制一个`nginx.conf`到`sites-available`目录
 - 编辑`docker-compose.yml`里面的`volumes` 模块，映射目录
 - 执行 `docker-compose up -d`

## Redis
 - 在`docker`内部直接使用 `Host: redis` 就可以连接`redis`服务
 - 访问 `redisManager`： http://localhost:8082