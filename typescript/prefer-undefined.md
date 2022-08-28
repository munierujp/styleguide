# prefer-undefined

nullよりもundefinedを使用してください。

:thumbsdown: このルールの誤ったコードの例：

```ts
const findNegativeNumber = (...numbers: number[]): number | null => {
  return numbers.find(number => number < 0) ?? null
}
```

:thumbsup: このルールの正しいコードの例：

```ts
const findNegativeNumber = (...numbers: number[]): number | undefined => {
  return numbers.find(number => number < 0)
};
```

## 参考

- [Coding guidelines · microsoft/TypeScript Wiki](https://github.com/Microsoft/TypeScript/wiki/Coding-guidelines#null-and-undefined)
- [スタイルガイド（コーディング規約） - TypeScript Deep Dive 日本語版](https://typescript-jp.gitbook.io/deep-dive/styleguide#null-vs-undefined)
- [undefinedとnullの違い | TypeScript入門『サバイバルTypeScript』](https://typescriptbook.jp/reference/values-types-variables/undefined-vs-null)
