# Network-boot

ネットワークブートサーバ

ネットワークブートクライアントはこちら → `https://github.com/murata0531/Network-boot-client`

# コンテナ作成

```
$ docker-compose build
```

# コンテナ起動

```
$ docker-compose up -d
```

# コンテナのシェルに入りブートサーバの実行ファイルを作成

```
$ docker-compose exec app /bin/bash

$ cd src

$ go build .
```
` Network-boot ` という実行ファイルが作成されているはずなので、それを実行すると `DHCPサーバ` 、 `TFTPサーバ` が起動する