# @phts/prettier-config

[![npm](https://img.shields.io/npm/v/@phts/prettier-config.svg)](https://www.npmjs.com/package/@phts/prettier-config)

My Prettier config.
Works best with [`@phts/eslint-config`](https://github.com/phts/eslint-config).

## Install

```bash
$ npm i -D @phts/prettier-config
```

To able to support [`@phts/eslint-config`](https://github.com/phts/eslint-config) additionally
install [`prettier-eslint-cli`](https://www.npmjs.com/package/prettier-eslint) globally:

```bash
$ npm i -g prettier-eslint-cli
```

## Usage

`.prettierrc.js`:

```js
module.exports = require('@phts/prettier-config')
```

## Sublime Text integration

Install [JsPrettier](https://packagecontrol.io/packages/JsPrettier) package and put this into `JsPrettier.sublime-settings`:

```json
{
  "auto_format_on_save": true,
  "auto_format_on_save_excludes": ["*/node_modules/*"],
  "auto_format_on_save_requires_prettier_config": true,
  "prettier_cli_path": "%APPDATA%\\npm\\prettier-eslint.cmd", // windows
  "prettier_cli_path": "/usr/local/bin/prettier-eslint"       // *nix
}
```
