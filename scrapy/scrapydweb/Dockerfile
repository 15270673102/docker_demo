FROM ryanvin/scrapydweb
MAINTAINER wangjiayu

RUN cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo 'Asia/Shanghai'>/etc/timezone

#RUN rm -rf /app
#RUN mkdir -p /app

#RUN mkdir -p /root/logs

#RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple --upgrade pip
#RUN pip3 install -i https://pypi.tuna.tsinghua.edu.cn/simple logparser

COPY scrapydweb_settings_v8.py /app/

#ENTRYPOINT ["logparser"]
