# @myowncake/config

An NPM package providing my own miscellaneous configuration.

## Install

```bash
$ npm i -D @myowncake/config
```

## Setup

### TypeScript

* Extend `dist/tsconfig.*.json`

### ESLint and Prettier

* Install Packages
  * @typescript-eslint/eslint-plugin
  * @typescript-eslint/parser
  * eslint
  * eslint-config-prettier
  * prettier
* Create eslintrc, extends `dist/.eslintrc.*.json` and set parserOptions like:
  ```json
  {
    "root": true,
    "extends": "./node_modules/@myowncake/config/dist/.eslintrc.node14.json",
    "parserOptions": {
      "project": ["./tsconfig.json"]
    }
  }
  ```
* Create prettierrc and require `dist/.prettierrc.general.js`:
  ```js
  module.exports = {
    ...require('@myowncake/config/dist/.prettierrc.general'),
    /* additional settings */
  }
  ```
