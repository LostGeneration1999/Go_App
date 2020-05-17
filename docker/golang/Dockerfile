# 使用するGolangのイメージを指定する
FROM golang:1.13

# 必要なパッケージなどなどをインストールする
RUN apt-get update -qq && \
    apt-get install -y mysql-client vim

# ワーキングディレクトリを指定する
WORKDIR /go/src/docker_compose_golang

# sample_docker_compose直下のディレクトリをコンテナ上に載せる
ADD . .

# プロジェクトをビルド
RUN go build