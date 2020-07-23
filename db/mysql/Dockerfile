FROM  mysql:5.7

LABEL version="1.0" description="mysql" authtor="wangjiayu" email="15270673102@163.com"

COPY mysqld.cnf /etc/mysql/mysql.conf.d/

RUN ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
RUN echo 'Asia/Shanghai' >/etc/timezone
