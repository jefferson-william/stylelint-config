# @jeffersonwilliammachado/stylelint-config

<p>
  <img src="https://img.shields.io/npm/v/@jeffersonwilliammachado/stylelint-config?style=flat-square&color=4677FF&labelColor=121212" alt="npm version" />
  <img alt="License" src="https://img.shields.io/github/license/jefferson-william/stylelint-config?style=flat-square&color=4677FF&labelColor=121212">
</p>

Shareable [`stylelint`](https://github.com/conventional-changelog/stylelint) config.

## Install

```sh
# pnpm
pnpm i -D @jeffersonwilliammachado/stylelint-config @stylelint/cli

# npm
npm i -D @jeffersonwilliammachado/stylelint-config @stylelint/cli

# Yarn
yarn add -D @jeffersonwilliammachado/stylelint-config @stylelint/cli
```

## Usage

After installing it, apply the config to `stylelint` by running the following command:

```sh
echo "module.exports = { extends: ['@jeffersonwilliammachado/stylelint-config'] };" > stylelint.config.js
```

## Bonus

To lint commits before they are created, install Husky and use the 'commit-msg' hook.

```sh
# npm
pnpm i -D husky

# npm
npm i -D husky

# yarn
yarn add -D husky
```

After that, you can create a `.huskyrc` file or add to your `package.json` the following code for

Husky v5:

```
# .husky/commit-msg
# pnpm
pnpx stylelint --quiet 'src/**/*.{css,scss,tsx}' --fix
# npm
npx stylelint --quiet 'src/**/*.{css,scss,tsx}' --fix
# yarn
yarn stylelint --quiet 'src/**/*.{css,scss,tsx}' --fix
```

## License

MIT License
