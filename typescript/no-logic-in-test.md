# no-logic-in-test

テストコードにロジックを書かないでください。

## :thumbsdown: 悪い例

```ts
const actual = add(1, 2)
assert.strictEqual(actual, 1 + 2)
```

## :thumbsup: 良い例

```ts
const actual = add(1, 2)
assert.strictEqual(actual, 3)
```

## 関連リンク

- [テストコードの期待値はDRYを捨ててベタ書きする ～テストコードの重要な役割とは？～ #Ruby - Qiita](https://qiita.com/jnchito/items/eb3cfa9f7db752dcb796)
- [フロントエンドのテストコードを書くときに大切にしていること - Cybozu Inside Out | サイボウズエンジニアのブログ](https://blog.cybozu.io/entry/2022/11/14/120000)
- [テストコード内では条件分岐を書かないようにする](https://azukiazusa.dev/blog/avoid-writing-conditional-branches-in-the%E2%80%93test-code/)
