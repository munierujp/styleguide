# no-enum

enumを使わないでください。それにはいくつかの問題があります。かわりにユニオン型の使用を検討してください。

:thumbsdown: このルールの誤ったコードの例：

```ts
enum Direction {
  Up = 'UP',
  Down = 'DOWN',
  Left = 'LEFT',
  Right = 'RIGHT'
}
```

:thumbsup: このルールの正しいコードの例：

```ts
export const Direction = {
  Up: 'UP',
  Down: 'DOWN',
  Left: 'LEFT',
  Right: 'RIGHT'
} as const

// 'UP' | 'DOWN' | 'LEFT' | 'RIGHT'
export type Direction = typeof Direction[keyof typeof Direction]

// ['UP', 'DOWN', 'LEFT', 'RIGHT']
const directions = Object.values(Direction)

// ユーザー定義型ガード関数
export const isDirection = (value: any): value is Direction => directions.includes(value)
```

## 参考

- [TypeScript: Handbook - Enums](https://www.typescriptlang.org/docs/handbook/enums.html#objects-vs-enums)
- [列挙型(enum)の問題点と代替手段 | TypeScript入門『サバイバルTypeScript』](https://typescriptbook.jp/reference/values-types-variables/enum/enum-problems-and-alternatives-to-enums)
- [さようなら、TypeScript enum - 株式会社カブク | 株式会社カブク](https://www.kabuku.co.jp/developers/good-bye-typescript-enum)
- [TypeScriptのenumを使わないほうがいい理由を、Tree-shakingの観点で紹介します](https://engineering.linecorp.com/ja/blog/typescript-enum-tree-shaking/)
