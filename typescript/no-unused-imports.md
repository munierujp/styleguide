# no-unused-imports

未使用のimport文を書かないでください。

## :thumbsdown: このルールの誤ったコードの例

```ts
import foo from './foo'
import bar from './bar'

foo()
```

## :thumbsup: このルールの正しいコードの例

```ts
import foo from './foo'

foo()
```
