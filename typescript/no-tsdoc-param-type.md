# no-tsdoc-param-type

[TSDoc](https://tsdoc.org/)の[`@param`](https://tsdoc.org/pages/tags/param/)に型を書かないでください。それは[JSDoc](https://jsdoc.app/)の[`@param`](https://jsdoc.app/tags-param)の記法です。TypeScriptは型情報を持っているので、コメントで型情報を付与する必要はありません。

## :thumbsdown: このルールの誤ったコードの例

```ts
/**
 * @param {string} somebody
 */
const sayHello = (somebody: string): void => {
  window.alert(`Hello ${somebody}`)
}
```

## :thumbsup: このルールの正しいコードの例

```ts
/**
 * @param somebody
 */
const sayHello = (somebody: string): void => {
  window.alert(`Hello ${somebody}`)
}
```
