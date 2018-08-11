# docker_training
Docker練習用 Repository

## first
### 概要
Docker & Docker-composeの使い方を理解するために，node.jsでHello worldを出力する環境を構築．
### 使い方

```bash
$ cd first
$ docker-compose build
$ docker-compose up
```

## apache_simple
### 概要
DockerでApacheの環境構築および，自作したWebコンテンツをdockerコンテナにコピーすることを理解する．


## ssl_apache
### 概要
ssl通信をするために，自己証明を行うApacheサーバ  
コンテナ立ち上げ時に，鍵を生成し，HTTPS通信の設定を自動で行う．
