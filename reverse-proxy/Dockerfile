FROM nginx:latest

# 作成した設定ファイル(.reverse_proxy.conf)を/etc/nginx/conf.d 配下にコピーする
COPY /reverse_proxy.conf /etc/nginx/conf.d/reverse_proxy.conf

# pingで通信確認をするために必要なパッケージのインストール
RUN apt-get update && apt-get install -y inetutils-ping