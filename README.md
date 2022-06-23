# `prettier-config-nick`

My opinionated yet practical [Prettier](https://prettier.io/) config for modern JavaScript

## Rationale

Here's what I've changed from Prettier's config and why. Most of the defaults are already pretty good, so check out the [Prettier docs](https://prettier.io/docs/en/options.html) for more information.

### `"semi": false`

Getting rid of semicolons makes it easier to read, write, and reorder lines of code

### `"trailingComma": "all"`

Modern browsers support adding trailing commas everywhere for more consistent code with clean diffs

## Installation

```sh
npm install --save-dev prettier prettier-config-nick
```

```sh
yarn add --dev prettier prettier-config-nick
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

## Environment support

This config uses features from ES2017 which are supported by Chrome, Firefox, and Safari. Legacy browsers like Internet Explorer require build tools like https://babeljs.io/docs/en/babel-preset-env.

### Node

8.0.0+

### TypeScript

2.7+
