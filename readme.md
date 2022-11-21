## Initialise a node project

Create your project folder and open it in VSCode, and then open the embedded terminal, and initialise node project by running the command:
`npm init -y`

## Webpack initialisation

Now we need to install the core tool for the building process — Webpack 5 (it’s the latest version on writing day).
`npm install webpack webpack-cli --save-dev`

## Webpack configurations

To be more production-ready, we will create multiple webpack configs, one for development, another one for building production artifacts.

## TypeScript integration

`npm install --save-dev typescript ts-loader`

### configure the ts-loader to load and transpile ts/tsx files

See the rules array of webpack.common.js to see how the ts-loader is setup with webpack.

## Webpack plugins

- `clean-webpack-plugin`: to clean the dist folder each time, when we do a new build.
- `html-webpack-plugin`: to generate index.html file from a template with scripts and style tags.
- `fork-ts-checker-webpack-plugin` - this plugin allows us to check typescript typings as a separate process. It will improve build performance.
- `copy-webpack-plugin` - This plugin gives us the ability to copy the assets folder with its content to dist folder.

`npm install clean-webpack-plugin copy-webpack-plugin fork-ts-checker-webpack-plugin html-webpack-plugin --save-dev`

## Jest Unit Testing framework

`npm install --save-dev jest ts-jest @types/jest `

## ESLint configuration

`npm i @typescript-eslint/eslint-plugin @typescript-eslint/parser — save-dev`
