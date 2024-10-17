# no-node-env-staging

環境変数`NODE_ENV`に`staging`のような値を設定しないでください。`NODE_ENV`に設定される値として`development`、`production`、`test`などしか想定されていないツールを使用している場合、想定外の値として`development`にフォールバックされる可能性があります。かわりにデプロイ先の環境を表す環境変数（`APP_ENV`など）を別途用意してください。

## 参考

- [Node.js — Node.js, the difference between development and production](https://nodejs.org/en/learn/getting-started/nodejs-the-difference-between-development-and-production)
- [Non-Standard `NODE_ENV` | Next.js](https://nextjs.org/docs/messages/non-standard-node-env)
- [Do not use NODE_ENV for staging | Better world by better software](https://glebbahmutov.com/blog/do-not-use-node-env-for-staging/)
- [NODE_ENVにdevelopmentとproduction以外を入れると辛い - ぷらすのブログ](https://blog.p1ass.com/posts/node-env/)
