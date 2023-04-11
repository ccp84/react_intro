# react_intro
 CI intro to react

## Install commands and file setup:
`npx create-react-app my-app --use-npm`
```
npm run build
Bundles the app into static files for production.

npm test
Starts the test runner.

npm run eject
Removes this tool and copies build dependencies, configuration files
and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:

cd my-app
npm start

Happy hacking!
```
* Installed ESLint and Prettier
```
npm install -D Eslint
npm install -D prettier@2.7.1
npm install -D eslint@8.24.0 eslint-config-prettier@8.5.0
npm install -D eslint-plugin-import@2.26.0 eslint-plugin-jsx-a11y@6.6.1 eslint-plugin-react@7.31.8
npm install -D eslint-plugin-react-hooks@4.6.0
```
* .eslintrc.json file
```
{
"extends": [
"eslint:recommended",
"plugin:import/errors",
"plugin:react/recommended",
"plugin:react-hooks/recommended",
"plugin:jsx-a11y/recommended",
"prettier"
],
"rules": {
"react/prop-types": 0,
"react/react-in-jsx-scope": 0
},
"plugins": ["react", "import", "jsx-a11y"],
"parserOptions": {
"ecmaVersion": 2022,
"sourceType": "module",
"ecmaFeatures": {
"jsx": true
}
},
"env": {
"es6": true,
"browser": true,
"node": true
},
"settings": {
"react": {
"version": "detect"
},
"import/resolver": {
"node": {
"extensions": [".js", ".jsx"]
}
}
}
}
```
* .prettierrc file
```
{}
```
* .gitignore
```
node_modules
.env
coverage/
.vscode/
```

