# Getting started with JavaScript development

This repository contains a minimal setup to get started with JavaScript development.
For an  excellent guide on the JavaScript language itself, see https://javascript.info

## Setup

Clone this repository by running
```cmd
git clone https://github.com/buildsofteu/learn-js.git .
```
in a folder of your choice.
Subsequently, make sure you have [Node js](https://nodejs.org/) installed and then run
```cmd
npm install
```

Now run `npm start` which will fire up a static file server and will copy its address to the clipboard.
Fire up Google Chrome and visit the address and then open the [JavaScript console](https://javascript.info/devtools).
You should see the message "Hello world from JavaScript!".
Congratulations, you're ready to get started!

## Development

The file `/playground/hello.js` can be used to start playing around.
Add any JavaScript to it you like and refresh the browser to see its effects in action!

You are encouraged to document your learning journey by commiting your work regularly.
Tried out something new and got it to work?
Cool, commit it so you can always get back to it later on if you break it in the future!

If you want to keep certain examples around, you can create a new `.html` file in the `/playground` folder with the standard
```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Title of the example</title>
  <script type="module" src="./source-file.js" async></script>
</head>
<body>
</body>
</html>
```
Give it a name and then it will be accessible on `http://localhost:port/file.html`.

## Linting

To enforce a consistent code style and reduce the risk of bugs, [eslint](https://eslint.org) is already set up in this repository.
To get live feedback on your code, you will need a plugin for the editor you're using.

If you're using [Sublime Text](https://www.sublimetext.com/), it's recommended to install [Sublime Linter](https://www.sublimelinter.com/en/stable/installation.html) and then the [SublimeLinter-eslint](https://github.com/SublimeLinter/SublimeLinter-eslint) plugin to get linting feedback in the editor.
**IMPORTANT** You have to install `SublimeLinter` **before** `SublimeLinter-eslint` or it WILL NOT WORK!

If you're use [VSCode](https://code.visualstudio.com/), you can use the [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) plugin.

## Unit tests

If you want to start learning how to perform unit tests in JavaScript, you can have a look at `/test/some-test.js`.
For unit tests we're using the combination of [Mocha](https://mochajs.org/) and the [Chai assertion library](https://www.chaijs.com/).
Feel free to add some test files in the `/test` folder and then see them in action by running `npm test` in the main folder.
