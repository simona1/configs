# Prettier

## Installation

There's only one package needed:

```
yarn add --dev --exact prettier
```

## Configuration

The defaults are great, but to be explicit add a `.prettierrc.json`.

```
echo {} > .prettierrc.json
```

Or use these preferred options:

```
{
  "bracketSameLine": true,
  "quoteProps": "consistent",
  "singleQuote": true,
  "trailingComma": "all"
}
```

Shortcut:

```
curl https://raw.githubusercontent.com/simona1/configs/main/prettier/.prettierrc.json > .prettierrc.json
```

Full documentation at: https://prettier.io/docs/en/options.html

## Additional

To ignore files add a `.prettierignore` file in the root of your project. Format is similar to `.gitignore`. By default Prettier ignores files in version control systems directories (`.git`, `.svn` and `.hg`) and `node_modules` (unless run with `--with-node-modules` on the command line).

```
cp .gitignore .prettierignore
```

For an npm/yarn script add to `package.json`:

```
{
  "scripts": {
    "format": "prettier --write ."
  }
}
```
