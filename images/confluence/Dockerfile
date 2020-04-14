# 一个Dockerfile

# confluence镜像源
FROM atlassian/confluence-server

# 运行用户
USER root

# 将代理破解包加入容器
COPY "./atlassian-agent.jar" /opt/atlassian/confluence/

# copy mysql驱动
COPY "./mysql-connector-java-5.1.48-bin.jar"  /opt/atlassian/confluence/confluence/WEB-INF/lib

# 设置启动加载代理包
RUN echo 'export CATALINA_OPTS="-javaagent:/opt/atlassian/confluence/atlassian-agent.jar ${CATALINA_OPTS}"' >> /opt/atlassian/confluence/bin/setenv.sh
