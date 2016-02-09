# demo-codecov
Used as an example repo to hook up to CodeCov

Initislise node with the command

```sh
npm init --y
```

(```--y``` skips filling in the package.json file and inputs blanks) 

Install codecov and istanbul as developer dependencies with the command

```sh
npm install codecov --save-dev
npm install istanbul --save-dev
```

In our package.json add

```javascript
"test": "node ./node_modules/.bin/istanbul cover test.js"
```

Create a test.js file - this is going to be what we will be testing the test coverage for
