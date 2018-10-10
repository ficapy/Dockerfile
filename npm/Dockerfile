FROM node:10.11

RUN apt update && apt install -y apt-transport-https && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian/ jessie main contrib non-free" > /etc/apt/sources.list \
    && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian/ jessie-updates main contrib non-free" >> /etc/apt/sources.list \
    && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian/ jessie-backports main contrib non-free" >> /etc/apt/sources.list \
    && echo "deb https://mirrors.tuna.tsinghua.edu.cn/debian-security jessie/updates main contrib non-free" >> /etc/apt/sources.list \
    && apt update \
    && apt install -y htop vim curl tzdata rsync && ln -snf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && npm set registry "https://registry.npm.taobao.org" \
    && npm set disturl "https://npm.taobao.org/dist"  \
    && npm set sass_binary_site "https://npm.taobao.org/mirrors/node-sass" \
    && npm set electron_mirror "https://npm.taobao.org/mirrors/electron/"   \
    && npm set puppeteer_download_host "https://npm.taobao.org/mirrors" \
    && npm set chromedriver_cdnurl "https://npm.taobao.org/mirrors/chromedriver" \
    && npm set operadriver_cdnurl "https://npm.taobao.org/mirrors/operadriver" \
    && npm set phantomjs_cdnurl "https://npm.taobao.org/mirrors/phantomjs" \
    && npm set selenium_cdnurl "https://npm.taobao.org/mirrors/selenium"  \
    && npm set node_inspector_cdnurl "https://npm.taobao.org/mirrors/node-inspector"  \
    && npm set selenium_cdnurl "http://npm.taobao.org/mirrors/selenium"   \
    && npm set node_inspector_cdnurl "https://npm.taobao.org/mirrors/node-inspector"

