# prefer-object-arguments

関数の引数が複数ある場合、オブジェクトとして受け取ることを検討してください。

## :thumbsdown: 悪い例

```ts
const func = (foo: boolean, bar: boolean): void => {
  // do something
}

func(true, false)
```

## :thumbsup: 良い例

```ts
const func = ({
  foo,
  bar
}: {
  foo: boolean,
  bar: boolean
}): void => {
  // do something
}

func({ foo: true, bar: false })
```

## 関連リンク

- [キーワード引数とOptions Objectパターン | TypeScript入門『サバイバルTypeScript』](https://typescriptbook.jp/reference/functions/keyword-arguments-and-options-object-pattern)
