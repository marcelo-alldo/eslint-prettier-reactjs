# eslint-prettier-reactjs

How to init project ReactJS with eslint and prettier
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Config Eslint and Prettier

In the project directory, you can install:

### `npm init @eslint/config`

Steps set in the project.\
❯ To check syntax, find problems, and enforce code style\
❯ JavaScript modules (import/export)\
❯ React\
? Does your project use TypeScript? › No / Yes (Yes)\
✔ Browser\
❯ Answer questions about your style\
❯ JSON\
❯ Spaces\
❯ Single\
❯ Unix\
? Do you require semicolons? › No / Yes (Yes)\
? Would you like to install them now? › No / Yes (Yes)\
❯ npm\

### `npm install --save-dev --save-exact prettier`

Create a file **_.prettierrc_** in ./

Put config JSON

```
{
	"printWidth": 120,
	"singleQuote": true,
	"tabWidth": 2,
	"useTabs": false,
	"trailingComma": "none",
	"arrowParens": "avoid"
}

```

### `npm install --save-dev eslint-config-prettier`

Then, add "prettier" to the "extends" array in your .eslintrc.\* file. Make sure to put it last, so it gets the chance to override other configs.

```
{
  "extends": [
    "some-other-config-you-use",
    "prettier"
  ]
}
```

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
To learn Eslint, check doc started [Eslint](https://eslint.org/docs/latest/user-guide/getting-started)
