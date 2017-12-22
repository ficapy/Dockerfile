FROM python:3.5.3-alpine
RUN echo "https://mirrors.tuna.tsinghua.edu.cn/alpine/v3.4/main/" > /etc/apk/repositories \
    &&  apk update && apk upgrade \
    && apk add --no-cache postgresql-dev gcc python3-dev musl-dev openssh netcat-openbsd tzdata bash rsync && cp -r -f /usr/share/zoneinfo/Asia/Shanghai /etc/localtime
