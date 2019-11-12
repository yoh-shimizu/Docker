参考記事リンク

- https://knowledge.sakura.ad.jp/15253/



Dockerfileあるディレクトリまで行く

```
cd gopython/
```

「gopython」という名前のimageを作製する

```
docker build -t gopython .
```

「test」という名前のコンテナを作る

```
docker run -d --name test gopython tail -f /dev/null
```

「test」コンテナに入るコマンド

```
docker exec -it test bash
```

コンテナ消すコマンド

```
docker rm -vf determined_villani
```


動いていないDockerイメージ全部消しちゃうやつ

```
docker image prune
```

