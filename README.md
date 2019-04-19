# @hellroot/stylelint-config

[![npm](https://img.shields.io/npm/v/@hellroot/stylelint-config.svg)](https://www.npmjs.com/package/@hellroot/stylelint-config)
[![dependencies status](https://img.shields.io/david/hellroot/stylelint-config.svg)](https://david-dm.org/hellroot/stylelint-config)
[![dev dependencies status](https://img.shields.io/david/dev/hellroot/stylelint-config.svg)](https://david-dm.org/hellroot/stylelint-config?type=dev)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier) [![Greenkeeper badge](https://badges.greenkeeper.io/hellroot/stylelint-config.svg)](https://greenkeeper.io/)

A StyleLint config compatible with [Prettier](https://prettier.io).

## Installation

```bash
npm install --save-dev prettier stylelint @hellroot/stylelint-config
```

## Configuration

Extend your StyleLint config:

`.stylelintrc`

```json
{
  "extends": ["@hellroot/stylelint-config"]
}
```

Configure EditorConfig:

`.editorconfig`

```editorconfig
root = true

[*]
charset = utf-8
indent_size = 2
end_of_line = lf
indent_style = space
max_line_length = 100
insert_final_newline = true
trim_trailing_whitespace = true

[*.md]
trim_trailing_whitespace = false
```

Configure Prettier:

`.prettierrc.json`

```json
{
  "singleQuote": true,
  "trailingComma": "none"
}
```

## Fix errors

Most of errors can be fixed automatically:

```bash
npx stylelint --fix '**/*.css'
```

## Migration

Format all your styles:

```bash
npx prettier --write '**/*.css'
```
