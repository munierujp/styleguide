# no-variable-name-type

変数名に型名を含めないでください。

## :thumbsdown: 悪い例

```ts
const numberArray = [1, 2]
```

## :thumbsup: 良い例

```ts
const numbers = [1, 2]
```

## :warning: 例外

既存の変数と役割が同じで型のみが異なる変数に対して、変数名の重複を避けるために型名をつけて区別するのはかまいません。

```ts
const requestBody = {
  message: 'Hello World'
}
const requestBodyString = JSON.stringify(requestBody)
```
