# @hiroxto/prettier-config

Prettier の設定

## 使い方

prettier をインストール。

```shell
$ yarn add -D prettier
```

`package.json`に`prettier`フィールドを作成し，`@hiroxto/prettier-config`を指定する。

```json
{
  "name": "my-project",
  "devDependencies": {
    "prettier": "latest"
  },
  "prettier": "@hiroxto/prettier-config"
}
```

設定を上書きしたい時は`package.json`では指定せずに，`.prettierrc.js`で指定して上書きする。

```javascript
module.exports = {
  ...require('@hiroxto/prettier-config'),
  semi: false,
};
```

## LICENSE

MIT
