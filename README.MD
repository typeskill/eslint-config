# `@typeskill/eslint-config`

Lint standard for typeskill compliant codestyle.

## Setup

1. You must install the config, and then provide all dependencies listed in `peerDependencies`.

```bash
npm install --save-dev @typeskill/eslint-config
npm install --save-dev @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-config-prettier eslint-plugin-prettier eslint-plugin-react prettier
```

2. Add this to the root `.eslintrc.js` file:

```javascript
module.exports = {
  extends: [
    "@typeskill/eslint-config",
  ],
}
```

3. Add this to the root `.prettierrc.js` file:

```javascript
module.exports = {
  semi: false,
  trailingComma: "all",
  singleQuote: true,
  printWidth: 120,
  tabWidth: 2
}
```

### IDE integration

Check your IDE integration here: [https://prettier.io/docs/en/editors.html](https://prettier.io/docs/en/editors.html).