FROM python:3
MAINTAINER wangjiayu

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai'>/etc/timezone

COPY scrapy.conf /etx/scrapyd/

RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple --upgrade pip
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple scrapy
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple scrapyd
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple scrapyd-client

CMD ["scrapyd"]

# docker build -t wjy/flask:1.0 .