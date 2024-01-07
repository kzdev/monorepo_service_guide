# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.187.0/containers/typescript-node/.devcontainer/base.Dockerfile

# [Choice] Node.js version: 16, 18, 20
ARG VARIANT="20-buster"
FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:0-${VARIANT}

# タイムゾーンを設定
ENV TZ=Asia/Tokyo

# 日本語のロケールをインストール
RUN apt-get update && apt-get install -y locales && \
    locale-gen ja_JP.UTF-8

# 環境変数を設定
ENV LANG=ja_JP.UTF-8 \
    LANGUAGE=ja_JP:ja \
    LC_ALL=ja_JP.UTF-8

# Turborepo/pnpm のインストール
RUN npm install -g turbo pnpm
