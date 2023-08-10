## 开发环境(目前)
- JDK8
- Maven3
- 本地具有Redis服务器
- 本地具有Neo4j数据库
- 本地具有elasticsearch8.6引擎
- 剩余磁盘空间大于20M

## 配置文件需要修改的地方
1. application.yml
- 本地Redis服务器URL和端口 `spring.redis.host/port`
- 后端端口 `server.port`
- 临时Neo4j数据库(本地)信息 `temporary-neo4j.uri/username/password`
- 本地文件存储位置 `files-path`
- 本地elasticsearch配置 `elasticsearch.host/port`
- Swagger2开启 `swagger.enable` 上线后置为false

2. db.yml
- 如果使用本地Oracle数据库，则修改该文件中的相关信息

3. logback.xml
- LOG_HOME 日志文件存储文件夹 绝对路径

## Swagger Api
开启swagger后，访问`host:port/swagger-ui.html`查看接口信息
