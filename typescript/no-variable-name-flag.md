# no-variable-name-flag

`boolean`型の変数に`flag`という名前をつけないでください。それは、条件式で使用したときに不自然に見えます。

## :thumbsdown: このルールの誤ったコードの例

```ts
const emptyFlag = values.length === 0

if (emptyFlag) {
  console.log('values is empty.')
}
```

## :thumbsup: このルールの正しいコードの例

```ts
const isEmpty = values.length === 0

if (isEmpty) {
  console.log('values is empty.')
}
```

## 参考

- [プログラミング ワンポイント – boolean型の変数の名前は命題にする](https://www.dcom-web.co.jp/blog/2016/0601)
- [C#でフラグ扱いの変数名にフラグと命名してはいけない - PG日誌](https://takap-tech.com/entry/2018/02/21/012100)
