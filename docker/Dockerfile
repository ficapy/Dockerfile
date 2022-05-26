FROM docker:20.10.16

RUN apk update && apk upgrade \
    && apk add --no-cache git tzdata openssh netcat-openbsd bash rsync curl py-pip \
    && pip install awscli \
    && cp -r -f /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && wget https://dl.min.io/client/mc/release/linux-amd64/mc \
    && chmod +x mc \
    && mv mc /usr/local/bin/
