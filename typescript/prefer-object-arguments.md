# prefer-object-arguments

関数の引数が複数ある場合、オブジェクトとして受け取ることを検討してください。

## :thumbsdown: このルールの誤ったコードの例

```ts
const func = (foo: string, bar: string): void => {
  // do something
}

func('foo', 'bar')
```

## :thumbsup: このルールの正しいコードの例

```ts
const func = ({
  foo,
  bar
}: {
  foo: string,
  bar: string
}): void => {
  // do something
}

func({ foo: 'foo', bar: 'bar' })
```

## 参考

- [キーワード引数とOptions Objectパターン | TypeScript入門『サバイバルTypeScript』](https://typescriptbook.jp/reference/functions/keyword-arguments-and-options-object-pattern)
