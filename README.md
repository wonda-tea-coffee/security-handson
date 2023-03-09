# サーバ起動

```sh
node server.js
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
