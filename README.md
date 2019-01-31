# Gatsby testing boilerplate

Steps and files on how to include basic testing (with jest) and linting (eslint, a11y) and code formatting to your gatsby starter.

## How to use

1. Install eslint, babel-eslint, and prettier. Other dependencies are plugins for eslint. (react, jsx-a11y, gatsby plugin, prettier eslint plugin)

```shell
npm install eslint prettier babel-eslint babel-preset-gatsby eslint-config-prettier eslint-plugin-prettier eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react gatsby-plugin-eslint --save-dev
```

2. Add `.eslintrc`, `.eslintignore`, and `.prettierrc` file. The file config is found on this repo.

3. Install jest, and it's dependencies.

```shell
npm install identity-obj-proxy jest jest-dom react-testing-library --save-dev
```

4. Include these files on the root file of your gatsby project.

- `__mocks__` folder
- `jest-preprocess.js`
- `jest.config.js`
- `jest.setup.js`
- `loadershim.js`

5. Add these scripts on your `package.json` file

```json
{
  "scripts": {
    "test": "jest",
    "test:watch": "npm run test -- --watch"
  }
}
```

You're good to go!
