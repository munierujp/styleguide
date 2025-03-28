# no-default-export

デフォルトエクスポートを使わないでください。かわりに名前付きエクスポートの使用を検討してください。

## :thumbsdown: 悪い例

```ts
export default class Foo {}
```

## :thumbsup: 良い例

```ts
export class Foo {}
```

## 関連リンク

- [export - JavaScript | MDN](https://developer.mozilla.org/ja/docs/Web/JavaScript/Reference/Statements/export)
- [エクスポートとインポート](https://ja.javascript.info/import-export)
- [Avoid Export Default | TypeScript Deep Dive 日本語版](https://typescript-jp.gitbook.io/deep-dive/main-1/defaultisbad)
- [import、export、require | TypeScript入門『サバイバルTypeScript』](https://typescriptbook.jp/reference/import-export-require)
- [なぜ default export を使うべきではないのか？](https://engineering.linecorp.com/ja/blog/you-dont-need-default-export)
- [アンサー: named exportは有害なのか - uhyo/blog](https://blog.uhy.ooo/entry/2021-09-09/answer-named-export/)
