FROM mcr.microsoft.com/devcontainers/base:ubuntu

# タイムゾーンを設定
ENV TZ=Asia/Tokyo

# 必要なパッケージのインストール
RUN apt-get update && apt-get install -y locales sudo

# 環境変数を設定
RUN locale-gen ja_JP.UTF-8
ENV LANG=ja_JP.UTF-8 \
    LANGUAGE=ja_JP:ja \
    LC_ALL=ja_JP.UTF-8