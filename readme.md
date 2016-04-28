# Jest CSS Modules
A [Jest](https://facebook.github.io/jest/) [script processor](https://facebook.github.io/jest/docs/api.html#config-scriptpreprocessor-string) that prevents [CSS module](https://github.com/css-modules/css-modules) parse errors.

## Installation

```shell
npm install --save-dev jest-css-modules
```

Update your package.json file's `jest` configuration:

```json
{
  "jest": {
    "scriptPreprocessor": "<rootDir>/node_modules/jest-css-modules",
  }
}
```

Now, imports such as `import styles from './MyModule.css';` will pass through Jest without causing any pain.

Supports `.css`, `.less`, `.scss` and `.styl` extensions.