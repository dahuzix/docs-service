# docs-service

a confluence service based on docker

## 说明

本项目仅用于个人兴趣爱好学习，如有商用，请支持正版

## 编译镜像

```js
docker-compose build

```

## 启动镜像

```js
docker-compose up -d
```

## 破解

```js
docker exec confluence-7.3.4  
    java -jar /opt/atlassian/confluence/atlassian-agent.jar
    -p conf
    -m data@data.com
    -o http://127.0.0.1
    -s BJTS-QYFC-PCVL-5L09
```
