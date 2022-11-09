# no-node-env-staging

環境変数`NODE_ENV`に`staging`のような値を設定しないでください。
`development`、`production`、`test`などの値しか想定されていないツールを使用している場合、想定外の値として`development`にフォールバックされる可能性があります。
かわりにデプロイ先の環境を表す環境変数を別途用意してください。

## 参考

- [Do not use NODE_ENV for staging | Better world by better software](https://glebbahmutov.com/blog/do-not-use-node-env-for-staging/)
- [NODE_ENVにdevelopmentとproduction以外を入れると辛い - ぷらすのブログ](https://blog.p1ass.com/posts/node-env/)
