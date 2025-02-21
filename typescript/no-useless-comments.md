# no-useless-comments

コードを読めば分かるようなコメントを書かないでください。

## :thumbsdown: 悪い例

```ts
// IDが空文字ではない場合
if (id !== '') {
  console.log(id)
}
```

```ts
// ユーザーを取得
const user = await fetchUser(id)
```

## :thumbsup: 良い例

```ts
if (id !== '') {
  console.log(id)
}
```

```ts
const user = await fetchUser(id)
```
