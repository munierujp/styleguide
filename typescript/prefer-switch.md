# prefer-switch

単純な等価比較をする場合、if文よりもswitch文を使用してください。

## :thumbsdown: このルールの誤ったコードの例

```ts
if (foo === 1) {
  // 1
} else if (foo === 2) {
  // 2
} else {
  // other
}
```

## :thumbsup: このルールの正しいコードの例

```ts
switch (foo) {
  case 1:
    // 1
    break
  case 2:
    // 2
    break
  default:
    // other
    break
}
```
