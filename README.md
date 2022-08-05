# @funboxteam/scss-lint-config

[![npm](https://img.shields.io/npm/v/@funboxteam/scss-lint-config.svg)](https://www.npmjs.com/package/@funboxteam/scss-lint-config)

[Stylelint](https://stylelint.io) rules that follow our style guide for SCSS.

[По-русски](./README.ru.md)

## Installation

First, install Stylelint that meets 
the [peerDependencies requirements](./package.json):

```bash
npm install --save-dev stylelint
```

If using Stylelint v14 or higher, also install Postcss-scss:

```bash
npm install --save-dev postcss-scss
```

Then install the config:

```bash
npm install --save-dev @funboxteam/scss-lint-config
```

## Usage

Include into a project config and pass desired [options](https://stylelint.io/user-guide/cli/):

```bash
stylelint "src/**/*.scss" --cache --config node_modules/@funboxteam/scss-lint-config/.stylelintrc
```

For Stylelint v13 `--syntax scss` option is required.

Also you can create your own config based on this one:

```js
module.exports = {
  extends: '@funboxteam/scss-lint-config/.stylelintrc.json',
  rules: [
    // your rule settings here
  ]
};
```

[![Sponsored by FunBox](https://funbox.ru/badges/sponsored_by_funbox_centered.svg)](https://funbox.ru)
