# no-unused-imports

コードを読めば分かるような、不要なコメントを書かないでください。

:thumbsdown: このルールの誤ったコードの例：

```ts
// メールアドレスが空文字ではない場合
if (email !== '') {
  console.log(email)
}
```

:thumbsup: このルールの正しいコードの例：

```ts
if (email !== '') {
  console.log(email)
}
```
