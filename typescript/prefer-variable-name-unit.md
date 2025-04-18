# prefer-variable-name-unit.md

時間や距離など単位のある数値を表す変数の名前には単位を含めてください。

## :thumbsdown: 悪い例

```ts
const TIMEOUT = 1
```

## :thumbsup: 良い例

```ts
const TIMEOUT_SECONDS = 1
const TIMEOUT_SEC = 1
```

## 関連リンク

- [【プログラミング全般】関数名や変数名等には単位を付けよう | ReMIXのブログ](https://remix-yh.net/301/)
