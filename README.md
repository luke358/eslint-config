# @luke358/eslint-config

[![npm](https://img.shields.io/npm/v/@luke358/eslint-config?color=a1b858&label=)](https://npmjs.com/package/@luke358/eslint-config)

- eslint monorepo

## Usage

### Install

```bash
pnpm add -D eslint @luke358/eslint-config
npm i -D eslint @luke358/eslint-config
yarn add -D eslint @luke358/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@luke358"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## License

MIT