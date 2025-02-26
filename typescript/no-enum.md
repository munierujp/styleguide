# no-enum

[Enum](https://www.typescriptlang.org/docs/handbook/enums.html)を使わないでください。かわりにユニオン型やオブジェクトの使用を検討してください。

## :thumbsdown: 悪い例

```ts
enum Direction {
  Up = 'UP',
  Down = 'DOWN',
  Left = 'LEFT',
  Right = 'RIGHT'
}
```

## :thumbsup: 良い例

ユニオン型を使う場合：

```ts
type Direction = 'UP' | 'DOWN' | 'LEFT' | 'RIGHT'
```

オブジェクトを使う場合：

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
export const directions = Object.values(Direction)

// ユーザー定義型ガード関数
export const isDirection = (value: any): value is Direction => directions.includes(value)
```

## 関連リンク

- [TypeScript: Handbook - Enums](https://www.typescriptlang.org/docs/handbook/enums.html#objects-vs-enums)
- [列挙型(enum)の問題点と代替手段 | TypeScript入門『サバイバルTypeScript』](https://typescriptbook.jp/reference/values-types-variables/enum/enum-problems-and-alternatives-to-enums)
- [さようなら、TypeScript enum - 株式会社カブク | 株式会社カブク](https://www.kabuku.co.jp/developers/good-bye-typescript-enum)
- [TypeScriptのenumを使わないほうがいい理由を、Tree-shakingの観点で紹介します](https://engineering.linecorp.com/ja/blog/typescript-enum-tree-shaking/)
