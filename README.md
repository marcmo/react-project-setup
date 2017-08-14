# Basic React Project Setup

## Create initial Project

Install **react-create-app** from [github](https://github.com/facebookincubator/create-react-app)

    react-create-app my-awesome-app

will create a react project based upon facebook's latest recommendations.

## Setup eslint, prettier and flowtypes

Copy some configuration files into the **my-awesome-app** folder

    .editorconfig
    .eslintrc.json
    .eslintignore
    .flowconfig

### Install required npm packages

wait: yarn add --dev eslint-config-airbnb-standard

    yarn add --dev flow-bin
    yarn add --dev prettier
    yarn add --dev prettier-eslint
    yarn add --dev eslint-config-prettier
    yarn add --dev eslint-config-airbnb
    yarn add --dev eslint-plugin-import
    yarn add --dev eslint-plugin-prettier
    yarn add --dev eslint-plugin-react

### Add dev scripts to package.json

    "scripts": {
      "flow": "flow",
      "lint": "eslint src",
      "eslint-check": "eslint --print-config .eslintrc.json | eslint-config-prettier-check",
    },

## Optional: Add bootstrap css framework

    yarn add bootstrap@4.0.0-beta

### Add import to src/index.js

    import '../node_modules/bootstrap/dist/css/bootstrap.min.css';


