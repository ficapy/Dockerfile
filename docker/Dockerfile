FROM docker:17.09-rc

RUN echo "https://mirrors.tuna.tsinghua.edu.cn/alpine/v3.6/main/" > /etc/apk/repositories \
    &&  apk update && apk upgrade \
    && apk add --no-cache git tzdata  && cp -r -f /usr/share/zoneinfo/Asia/Shanghai /etc/localtime