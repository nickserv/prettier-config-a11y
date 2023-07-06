# `prettier-config-a11y`

[Prettier](https://prettier.io/) config improving accessibility for visual, cognitive, and motor disabilities

## Installation

```sh
npm install --save-dev prettier prettier-config-a11y
```

```sh
yarn add --dev prettier prettier-config-a11y
```

```sh
pnpm add --save-dev prettier prettier-config-a11y
```

## Usage

### `package.json`

```json
"prettier": "prettier-config-a11y"
```

### [Other Prettier config](https://prettier.io/docs/en/configuration.html)

```json
"prettier-config-a11y"
```

## Rationale

Here's what I've changed from Prettier's config and why. Most of the defaults are already pretty good, so check out the [Prettier docs](https://prettier.io/docs/en/options.html) for more information.

### `"useTabs": true`

Indentations are easier for assistive technology to read when using tabs instead of spaces because they take up less characters. Visual representations of tab indentations can also be increased by users with visual and cognitive disabilities without affecting other users.

### Defaults

Prettier 3 already uses these defaults, but we set them explicitly to encourage accessibility, even with older versions of Prettier.

#### `"semi": true`

Disabled users are more likely to prefer semicolons (source: [Twitter poll](https://twitter.com/nickemccurdy/status/1624305594415955973)), likely because they make it easier to understand when lines of code end, even when Prettier wraps them.

#### `"singleQuote": false` and `"jsxSingleQuote": false`

Double quotes are easier for some assistive technology to read than single quotes because they may be spoken as "apostrophe", which is a syllable longer than "double quote", but sounds similar to "single quote". Double quotes are also larger, making them easier to see. Meanwhile, HTML and JSX code is typically formatted with double quotes, so consistently using double quotes in other languages makes code behave more consistently and potentially reduces cognitive load.

#### `"trailingComma": "all"`

Reduces the size of diffs, making them easier to read, especially with visual and cognitive disabilities.

#### `"arrowParens": "always"`

Keeps arguments in arrow functions consistent and easy to adjust, resulting in less work for those with cognitive and motor disabilities.

#### `"endOfLine": "lf"`

This reduces unnecessary end of line changes when switching operating systems, which can can be especially confusing for those with disabilities.
