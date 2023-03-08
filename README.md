# サーバ起動

```sh
docker run --rm -it -v $(pwd):/work --workdir /work -p 3000:3000 node server.js
```

# サーバを落とす

Ctrl+Cで落ちないの何故なのだ

```sh
docker kill $(docker ps -q)
```

# WSLでのハマりどころ
## site.exampleの設定方法
Windows側のhostsに下記を追加

```
127.0.0.1 site.example
::1 site.example
```

**参考**
- https://github.com/microsoft/WSL/issues/6426
- https://qiita.com/tiibun/items/5719869552ee5b713d83
  - hostsを管理者権限でシュッと開く方法
