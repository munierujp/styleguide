# no-function-name-check

`boolean`型を返す関数に`check`という名前をつけないでください。

## :thumbsdown: 悪い例

```ts
const checkZero = (value: unknown): value is 0 => value === 0
```

## :thumbsup: 良い例

```ts
const isZero = (value: unknown): value is 0 => value === 0
```

## 関連リンク

- [boolean 値を返却するメソッド名、変数名の付け方 - KUSAMAKURA](https://kusamakura.hatenablog.com/entry/2016/03/03/boolean_%E5%80%A4%E3%82%92%E8%BF%94%E5%8D%B4%E3%81%99%E3%82%8B%E3%83%A1%E3%82%BD%E3%83%83%E3%83%89%E5%90%8D%E3%80%81%E5%A4%89%E6%95%B0%E5%90%8D%E3%81%AE%E4%BB%98%E3%81%91%E6%96%B9)
- [プログラミング ワンポイント – boolean型の変数の名前は命題にする](https://www.dcom-web.co.jp/blog/2016/0601)
- [真偽値を返す関数名のつけ方の例 - Qiita](https://qiita.com/munieru_jp/items/f66026060b7b5f0c3cbf)
