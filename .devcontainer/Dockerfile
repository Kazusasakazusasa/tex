FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

# タイムゾーン設定
ENV TZ=Asia/Tokyo

# LaTeX および関連ツールをインストール
RUN apt-get update && apt-get install -y \
    texlive-full \
    ghostscript \
    git \
    git-lfs \
    && rm -rf /var/lib/apt/lists/*

# LaTeX ドキュメントのビルド設定
WORKDIR /workspace
