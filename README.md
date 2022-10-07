# 概要
RailsのDocker環境テンプレート

# 環境構築手順
```
$ git clone git@github.com:Takuty-a11y/Rails-Docker-Sample.git
$ cd Rails-Docker-Sample
$ docker-compose build
$ docker-compose run web rails new . --force --no-deps --database=postgresql
# database.yml変更
$ docker-compose run web rails db:create
$ docker-compose up -d
```

## 参考
以下の記事で扱っています
- [Docker初心者がRailsのローカル環境を構築してみる](https://zenn.dev/takuty/articles/6f7afabca322d1)