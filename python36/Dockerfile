FROM python:3.6.5-slim-stretch

RUN apt update && apt install -y apt-transport-https \
    && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian stretch main" > /etc/apt/sources.list \
    && echo "deb-src https://mirrors.tuna.tsinghua.edu.cn/debian stretch main" >> /etc/apt/sources.list \
    && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian stretch-updates main" >> /etc/apt/sources.list \
    && echo "deb-src https://mirrors.tuna.tsinghua.edu.cn/debian stretch-updates main" >> /etc/apt/sources.list \
    && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian-security stretch/updates main" >> /etc/apt/sources.list \
    && echo "deb-src https://mirrors.tuna.tsinghua.edu.cn/debian-security stretch/updates main" >> /etc/apt/sources.list \
    && apt update \
    && apt install -y htop vim curl tzdata && ln -snf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime