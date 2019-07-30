# ESLint config for 🍷Sherry🍷

[![Greenkeeper badge](https://badges.greenkeeper.io/ulivz/eslint-config-sherry.svg)](https://greenkeeper.io/)

<img src="./media/vermouth.jpeg" alt="sherry" width="300">

This config is supposed to work with [XO](https://github.com/sindresorhus/xo) or [eslint-config-xo](https://github.com/sindresorhus/eslint-config-xo).

## Features

- Indent with 2 spaces and no semicolon
- [Lint code blocks in Markdown!](#lint-code-blocks-in-markdown)
- [Enforce consistent spacing inside](https://eslint.org/docs/rules/object-curly-spacing)
- [Require Following Curly Brace Conventions with `multi` option](https://eslint.org/docs/rules/curly#multi)
- [Disallow unused expressions](https://eslint.org/docs/rules/no-unused-expressions)

## Install

```bash
yarn add -D eslint-config-sherry
# OR: npm install -D eslint eslint-config-sherry
```

## Usage

In ESLint:

```js
/* package.json */
{
  "eslintConfig": {
    "extends": ["xo/esnext", "sherry"]
  }
}
```

Or in XO:

```js
/* package.json */
{
  "xo": {
    "extends": "sherry"
  }
}
```

### Use Prettier

```js
/* package.json */
{
  "xo": {
    "extends": "sherry/prettier"
  }
}
```

### Lint code blocks in markdown

It uses [eslint-plugin-markdown](https://github.com/eslint/eslint-plugin-markdown):

```json
{
  "xo": {
    "extensions": ["md"]
  }
}
```

## License

[MIT](./LICENSE)

Copyright (c) 2018-present, ULIVZ & SHERRY
