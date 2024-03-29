# `@typeskill/eslint-config`

Lint standard for typeskill compliant codestyle.

## Setup

1. You must install the config, and then provide all dependencies listed in `peerDependencies`.

```bash
npm install --save-dev @typeskill/eslint-config eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-config-prettier eslint-plugin-prettier eslint-plugin-react prettier eslint-plugin-react-hooks 
```

2. Add this to the root `.eslintrc.js` file:

```javascript
module.exports = {
  plugins: [
    "react-hooks", // optional
  ],
  extends: [
    "@typeskill/eslint-config",
  ],
  parserOptions: {
    project: './tsconfig.json' // change tsconfig to whichever appropriate config file
  },
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

Check prettier IDE integration here: [https://prettier.io/docs/en/editors.html](https://prettier.io/docs/en/editors.html).