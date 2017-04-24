# npmdoc-history

#### api documentation for  [history (v4.6.1)](https://github.com/reacttraining/history#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-history.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-history) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-history.svg)](https://travis-ci.org/npmdoc/node-npmdoc-history)

#### Manage session history with JavaScript

[![NPM](https://nodei.co/npm/history.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/history)

- [https://npmdoc.github.io/node-npmdoc-history/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-history/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-history/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-history/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-history/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-history/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michael Jackson"
    },
    "browserify": {
        "transform": [
            "loose-envify"
        ]
    },
    "bugs": {
        "url": "https://github.com/reacttraining/history/issues"
    },
    "dependencies": {
        "invariant": "^2.2.1",
        "loose-envify": "^1.2.0",
        "resolve-pathname": "^2.0.0",
        "value-equal": "^0.2.0",
        "warning": "^3.0.0"
    },
    "description": "Manage session history with JavaScript",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-core": "^6.23.1",
        "babel-eslint": "^7.0.0",
        "babel-loader": "^6.2.10",
        "babel-plugin-dev-expression": "^0.2.1",
        "babel-plugin-transform-object-assign": "^6.8.0",
        "babel-preset-es2015": "^6.9.0",
        "babel-preset-stage-1": "^6.5.0",
        "eslint": "^3.3.0",
        "eslint-plugin-import": "^2.0.0",
        "expect": "^1.20.1",
        "gzip-size": "^3.0.0",
        "in-publish": "^2.0.0",
        "karma": "^1.2.0",
        "karma-browserstack-launcher": "^1.0.1",
        "karma-chrome-launcher": "^2.0.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.0.1",
        "karma-mocha-reporter": "^2.0.4",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^2.0.1",
        "mocha": "^3.0.2",
        "pretty-bytes": "^4.0.2",
        "readline-sync": "^1.4.4",
        "webpack": "^1.13.1",
        "webpack-dev-server": "^1.14.1"
    },
    "directories": {},
    "dist": {
        "shasum": "911cf8eb65728555a94f2b12780a0c531a14d2fd",
        "tarball": "https://registry.npmjs.org/history/-/history-4.6.1.tgz"
    },
    "files": [
        "DOMUtils.js",
        "ExecutionEnvironment.js",
        "LocationUtils.js",
        "PathUtils.js",
        "createBrowserHistory.js",
        "createHashHistory.js",
        "createMemoryHistory.js",
        "createTransitionManager.js",
        "es",
        "index.js",
        "umd"
    ],
    "gitHead": "a647c5d1e5442998855700195b80a8a60b7f7656",
    "homepage": "https://github.com/reacttraining/history#readme",
    "keywords": [
        "history",
        "location"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "mjackson"
        }
    ],
    "name": "history",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/reacttraining/history.git"
    },
    "scripts": {
        "build": "node ./tools/build.js",
        "clean": "git clean -e '!node_modules' -fdX .",
        "lint": "eslint modules",
        "prepublish": "node ./tools/build.js",
        "release": "node ./tools/release.js",
        "start": "webpack-dev-server -d --content-base ./ --history-api-fallback --inline modules/index.js",
        "test": "karma start --single-run"
    },
    "version": "4.6.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
