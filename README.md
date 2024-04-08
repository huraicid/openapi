# openapi
#後で書く

---

# 前準備
## npmのインストール
npmがインストールされていない場合はあらかじめインストールしておく。

### Windowsの場合
以下を参照。

https://qiita.com/gahoh/items/8444da99a1f93b6493b4

### Macの場合
Homebrewでインストールすると楽。

```bash
$ brew install node
```

## Docker Desktopの起動
あらかじめDocker Desktopを起動しておく。

---

# 実行手順
### このリポジトリをcloneする

```bash
git clone https://github.com/huraicid/openapi.git
```


### モックサーバを起動する
```bash
cd openapi
npm run mockapi
```

※Windowsの場合、そのまま実行するとエラーになるので、`openapi/package.json`の中身を以下のように置換する必要あり。

- `${PWD}` → `%cd%`


### APIにアクセスする

下記のURLにアクセスする

```
http://localhost:3001/api/v1/hello
```

レスポンスが帰ってきているのが確認できるはず。


---

# 参考
- [OpenAPI (Swagger) まとめ](https://qiita.com/KNR109/items/7e094dba6bcf37ed73cf)
