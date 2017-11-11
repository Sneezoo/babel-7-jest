# babel-7-jest
[Babel](https://github.com/babel/babel) [jest](https://github.com/facebook/jest)
plugin

babel-jest didn't work with `@babel/*` packages so I made it to do so.

## Setup

```
npm install --save-dev babel-jest
```

Add it to your jest configuration like this:
```
"jest": {
  "transform": {
    ".js$": "babel-7-jest"
  }
}
```

For more information have a look at the
[jest docs](http://facebook.github.io/jest/docs/configuration.html#transform-object-string-string)
