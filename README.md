# @hiroxto/prettier-config

[![npm version](https://badge.fury.io/js/@hiroxto%2Fprettier-config.svg)](https://badge.fury.io/js/@hiroxto%2Fprettier-config)
![GitHub Actions test workflow](https://github.com/hiroxto/prettier-config/actions/workflows/test.yml/badge.svg)

Prettierの設定

## 使い方

prettierと@hiroxto/prettier-configをインストール。

```shell
$ yarn add -D prettier @hiroxto/prettier-config
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
