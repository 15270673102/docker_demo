FROM python:3
MAINTAINER wangjiayu

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai'>/etc/timezone

RUN mkdir -p /etc/scrapyd
COPY ./scrapyd.conf /etc/scrapyd/
WORKDIR /etc/scrapyd/

RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple --upgrade pip
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple scrapy
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple scrapyd
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple scrapyd-client

EXPOSE 6800
ENTRYPOINT ["scrapyd"]