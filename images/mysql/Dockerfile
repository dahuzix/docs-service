# 一个Dockerfile

# mysql镜像源
FROM mysql:5.7.29

# 运行用户
USER root

# 将my.cnf复制到mysql配置
COPY "./my.cnf" /etc/mysql/conf.d

# RUN 安装vim
# RUN apt-get update \
# && apt-get install vim