# PHPでPrettierを使用する

## npmパッケージのインストール

```
npm i -D prettier @prettier/plugin-php
```

- `prettier`: Prettier本体
- `@prettier/plugin-php`: php用のPrettierプラグイン

## プロジェクトルートに　`.prettierrc`を作成して設置

```
{
  "singleQuote": true,
  "trailingComma": "all",
  "phpVersion": "8.0"
}
```

## VSCode settings.json

- Prettier拡張機能は入れてある前提
- 参考サイト[1]で触れられている拡張機能`Run On Save`は特に必要ない。

PHPをPrettierでフォーマットする記述を追加する。

```json
"[php]": {
    "editor.formatOnSave": true
},
```

## 参考
- [PHPでもコード整形ツール「Prettier」を使いたい時 - Qiita](https://qiita.com/AkiraTameto/items/4cefe2608b03f396c7cd) [1]
- [@prettier/plugin-php  -  npm](https://www.npmjs.com/package/@prettier/plugin-php)
