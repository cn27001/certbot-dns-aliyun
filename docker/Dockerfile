FROM ubuntu:20.04
RUN  sed -i 's/[a-z]\+\.[a-z]\+\.[a-z]\+/mirrors.aliyun.com/' /etc/apt/sources.list && \
     apt-get update && \
     apt-get install -y certbot

COPY .  /path/to/dns/
RUN chmod +x /path/to/dns/*
ENV PATH = "$PATH:/path/to/dns"
CMD ["/bin/bash"]
