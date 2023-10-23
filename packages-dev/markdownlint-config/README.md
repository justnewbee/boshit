# @boshit/markdownlint-config

A shareable markdown lint config, which can be used with `markdownlint-cli` or `markdownlint-cli2`.

## Inherit

`@boshit/markdownlint-config` ← _BASE_

## Install & Setup

```bash
npm i -D markdownlint-cli2 @boshit/markdownlint-config
pnpm add -D markdownlint-cli2 @boshit/markdownlint-config
yarn add -D markdownlint-cli2 @boshit/markdownlint-config
```

In your `.markdownlint.yaml`:

```yml
extends: "@boshit/markdownlint-config"
```

## Usage

### Terminal

```bash
npx markdownlint-cli2 ./README.md
```

### npm-scripts

```bash
npm pkg set scripts.lint:md="markdownlint-cli2 **/*.md #node_modules"
```

## With `lint-staged`

```json
{
  "lint-staged": {
    "*.md": "markdownlint-cli2"
  }
}
```