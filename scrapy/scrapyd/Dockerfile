FROM python:3
MAINTAINER wangjiayu

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai'>/etc/timezone

RUN mkdir -p /etc/scrapyd
COPY ./scrapyd.conf /etc/scrapyd/

RUN mkdir -p /home/wangjiayu/scrapyd
COPY ./requirements.txt /home/wangjiayu/scrapyd/
WORKDIR /home/wangjiayu/scrapyd/

RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple --upgrade pip
RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple -r requirements.txt

EXPOSE 6800
ENTRYPOINT ["scrapyd"]