# @funboxteam/scss-lint-config

[![npm](https://img.shields.io/npm/v/@funboxteam/scss-lint-config.svg)](https://www.npmjs.com/package/@funboxteam/scss-lint-config)

Пакет с правилами для [Stylelint](https://stylelint.io), соответствующие принятому в компании стайлгайду для SCSS-файлов.

## Установка

Сперва необходимо установить версию Stylelint, удовлетворяющую требованиям, 
описанным в [peerDependencies](./package.json):

```bash
npm install --save-dev stylelint
```

Затем можно устанавливать сам конфиг:

```bash
npm install --save-dev @funboxteam/scss-lint-config
```

## Использование

Подключить в конфиг рабочего проекта, передав необходимые [опции](https://stylelint.io/user-guide/cli/):

```bash
stylelint "src/**/*.scss" --syntax scss --cache --config node_modules/@funboxteam/scss-lint-config/.stylelintrc`
```

Помимо этого можно описать локальный конфиг проекта, основанный на этом:

```js
module.exports = {
  extends: '@funboxteam/scss-lint-config/.stylelintrc.json',
  rules: [
    // доопределения правил
  ]
};
```

[![Sponsored by FunBox](https://funbox.ru/badges/sponsored_by_funbox_centered.svg)](https://funbox.ru)
