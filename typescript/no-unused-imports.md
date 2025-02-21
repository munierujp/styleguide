# no-unused-imports

未使用のimport文を書かないでください。

## :thumbsdown: 悪い例

```ts
import foo from './foo'
import bar from './bar'

foo()
```

## :thumbsup: 良い例

```ts
import foo from './foo'

foo()
```
