# Prettier
Prettierについての設定やメモ

## Install

### npm
#### local
```shell
npm i -D prettier
```

## VSCodeの設定

VSCodeでファイル保存時にフォーマットが実行されるようにする。

### 拡張機能をインストール

- [Prettier - Code formatter - Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

### settings.json

インストールした拡張機能をVSCodeの既定のフォーマッターとし、
指定された拡張子のみファイル保存時のフォーマットを有効にする。
下記を追記する。

```json
"editor.formatOnSave": false,
"editor.defaultFormatter": "esbenp.prettier-vscode",
"[(lang)]": {
    "editor.formatOnSave": true
}
```
- (lang)には`html`や`javascript`といった言語名が入る。

## フォーマット形式の設定

ルートディレクトリに`.prettierrc`ファイルを作成し、それに設定を書き込む。
