# babel-7-jest
[Babel](https://github.com/babel/babel) [jest](https://github.com/facebook/jest)
plugin

babel-jest didn't work with `@babel/*` packages so I made it to do so.

## Setup

```
npm install --save-dev babel-7-jest
```

Add it to your jest configuration like this:
```
"jest": {
  "transform": {
    ".js$": "babel-7-jest"
  }
}
```

A minimal `package.json` would look like this:
```
{
  "name": "example",
  "version": "0.0.1",
  "description": "Example of jest and babel 7",
  "main": "server.js",
  "scripts": {
    "test": "jest",
    "dev:test": "jest --watch"
  },
  "jest": {
    "transform": {
      ".js$": "babel-7-jest"
    }
  },
  "author": "Sneezoo",
  "license": "MIT",
  "devDependencies": {
    "@babel/core": "^7.0.0-beta.31",
    "babel-7-jest": "^21.3.1",
    "jest": "^21.2.1"
  },
  "dependencies": {}
}
```
Be aware of `@babel/core`, which you will need to add to your devDepenencies!

For more information have a look at the
[jest docs](http://facebook.github.io/jest/docs/configuration.html#transform-object-string-string)
