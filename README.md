# `prettier-config-nick`

My opinionated yet practical [Prettier](https://prettier.io/) config for modern JavaScript

## Rationale

Here's what I've changed from Prettier's config and why. Most of the defaults are already pretty good, so check out the [Prettier docs](https://prettier.io/docs/en/options.html) for more information.

### `"semi": false`

Getting rid of semicolons makes it easier to read, write, and reorder (see [prettier#13317](https://github.com/prettier/prettier/issues/13317)) lines of code

### Defaults

Prettier 3 already uses these defaults, but we set them explicitly so you can use older versions consistently

- `"trailingComma": "all"`
- `"arrowParens": "always"`
- `"endOfLine": "lf"`

## Installation

```sh
npm install --save-dev prettier prettier-config-nick
```

```sh
yarn add --dev prettier prettier-config-nick
```

```sh
pnpm add --save-dev prettier prettier-config-nick
```

## Usage

### `package.json`

```json
"prettier": "prettier-config-nick"
```

### [Other Prettier config](https://prettier.io/docs/en/configuration.html)

```json
"prettier-config-nick"
```
