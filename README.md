# Docker on rails6

## 環境
* ruby 2.6.3
* rails 5.2.3
* Postgresql 12.0

## まずはじめに

* Dockerfile
* docker-compose.yml
* Gemfile
* Gemfile.lock
* entrypoint.sh

を作る

## railsアプリ作成

```$ docker-compose run web rails new . --force --no-deps --database=postgresql```

## イメージのビルド

```$ docker-compose build```


## config/database.ymlを書き換える

## dbの作成
```$ docker-compose run web rake db:create```

## コンテナ起動
```$ docker-compose up```