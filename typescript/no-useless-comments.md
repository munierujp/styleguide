# no-unused-imports

コードを読めば分かるような、不要なコメントを書かないでください。

:thumbsdown: このルールの誤ったコードの例：

```ts
// メールアドレスが空文字ではない場合
if (email !== '') {
  console.log(email)
}
```

```ts
// ユーザーを取得
const user = await fetchUser(userName)
```

:thumbsup: このルールの正しいコードの例：

```ts
if (email !== '') {
  console.log(email)
}
```

```ts
const user = await fetchUser(userName)
```
