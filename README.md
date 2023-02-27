# eslint-config-nestjs

This package is extracted from [nestjs/typescript-starter](https://github.com/nestjs/typescript-starter). Its aim is to reduce the number of "direct" dependencies in your package.json file and keep your .eslintrc.js file clean.

## Installation

To use this package in your project, you can install it via npm:

```
npm i -D eslint-config-nestjs
```

## Usage

After installing the `eslint-config-nestjs` package, you can configure your `.eslintrc.js` file to use it as follows:

```js
module.exports = {
  extends: 'nestjs'
}
```

This will extend the `eslint-config-nestjs` configuration, which includes all of the necessary ESLint plugins and rules for NestJS projects. You can customize the configuration by adding additional rules or overrides as needed.

For example, to override a rule, you can add a rules object to your .eslintrc.js file:

```js
module.exports = {
  extends: 'nestjs',
  rules: {
    'no-console': 'off'
  }
}
```

## Removing Direct Dependencies

Since `eslint-config-nestjs` includes all of the necessary ESLint plugins and rules for NestJS projects, you can remove the direct dependencies from your `package.json` file.

To remove the direct dependencies, you can run the following command in your terminal:

```bash
npm uninstall @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-config-prettier eslint-plugin-prettier prettier
```
This will remove the following packages from your project:

- `@typescript-eslint/eslint-plugin`
- `@typescript-eslint/parser`
- `eslint`
- `eslint-config-prettier`
- `eslint-plugin-prettier`
- `prettier`
