# Eslint with StandardJS

# docs

+ [Eslint](https://github.com/eslint/eslint)
+ [prettier-eslint](https://github.com/prettier/prettier-eslint)
+ [prettier-standard](https://github.com/sheerun/prettier-standard)
+ [eslint-config-standard](https://github.com/standard/eslint-config-standard)

>note: prettier-standard is a formatter, not a linter. It'll never output any linting errors

see [#17](https://github.com/sheerun/prettier-standard/issues/17)

# install

```
> yarn add --dev prettier-standard
> yarn add --dev eslint-config-standard eslint-plugin-standard eslint-plugin-promise eslint-plugin-import eslint-plugin-node
```

# .eslintrc.js

```js
module.exports = {
  root: true,
  env: {
    node: true,
    es6: true
  },
  extends: 'standard', // see [eslint-config-standard](https://github.com/standard/eslint-config-standard)
  parserOptions: {
    sourceType: 'module'
  }
}
```

# start

```sh
> yarn
> yarn run format
```
