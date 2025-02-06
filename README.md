# npx mohammedkhan 

> Get to know Mohammed  via npm. Just run npx mohammedkhan

## Usage

To use this CLI run the following command

```sh

npx mohammedkhan 

```

## Steps for ESlint Integration process:

### Verify Your Project Setup

Open your project in Visual Studio Code.
Ensure that your project directory contains a valid package.json file.
Ensure you can open an integrated terminal running a bash/zsh shell in the root folder.

### Install ESLint

Install ESLint as a development dependency using npm.

```sh

npm install eslint --save-dev

```
After running this command, ESLint will be listed under devDependencies in your package.json file, and you can configure it according to your project’s requirements.

### Run ESLint Initialization

In the integrated terminal, run the ESLint initialization command.

```sh

npm init @eslint/config

```
Follow the interactive prompts to answer configuration questions tailored to your project.

ESLint finishes resulting in an eslint.config.mjs file.

If needed, you can run this init script again if you need to change any answer.

### Configure the Generated File

Open the generated eslint.config.mjs file in Visual Studio Code.

Review the default settings and adjust them as necessary to match your project’s coding style and requirements.

Ensure that the configuration includes all desired rules and plugins relevant to your project. 

### Add a Lint Script to package.json

Open your package.json file in Visual Studio Code.

Add a script entry that allows you to run ESLint on your code.

Ensure the commas is configured correctly to target the files you wish to lint.

```sh

"scripts": {
    "test": "echo \"error: no test specified\" && exit 1",
    "lint": "eslint index.js"

},

```
### Run the Linting Process

Use the integrated terminal to execute the lint script you added.

```sh

npm run lint

```

or use npx

```sh

npx eslint index.js

```

Review the output carefully, noting any issues that ESLint reports.

### Fix Reported Issues

Address each linting error or warning by updating your code accordingly.

Continue running the lint command until your code passes all linting checks.

Repeat this as needed when you add more code to this project.
