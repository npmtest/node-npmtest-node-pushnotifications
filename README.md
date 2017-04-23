# npmtest-node-pushnotifications

#### basic test coverage for  [node-pushnotifications (v1.0.18)](https://github.com/appfeel/node-pushnotifications)  [![npm package](https://img.shields.io/npm/v/npmtest-node-pushnotifications.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-node-pushnotifications) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-node-pushnotifications.svg)](https://travis-ci.org/npmtest/node-npmtest-node-pushnotifications)

#### A cross-platform push service for node.js

[![NPM](https://nodei.co/npm/node-pushnotifications.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-pushnotifications)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-node-pushnotifications/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-node-pushnotifications/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-node-pushnotifications/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-node-pushnotifications/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-node-pushnotifications/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-node-pushnotifications/build/test-report.html](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-node-pushnotifications/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-pushnotifications/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-pushnotifications/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-pushnotifications/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-node-pushnotifications/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "AppFeel"
    },
    "bugs": {
        "url": "https://github.com/appfeel/node-pushnotifications"
    },
    "contributors": [
        {
            "name": "Alexander Friedl",
            "url": "https://github.com/alex-friedl"
        }
    ],
    "dependencies": {
        "apn": "^2.1.1",
        "node-adm": "^0.9.1",
        "node-gcm": "^0.14.4",
        "wns": "^0.5.3"
    },
    "description": "A cross-platform push service for node.js",
    "devDependencies": {
        "babel-cli": "^6.16.0",
        "babel-core": "^6.17.0",
        "babel-preset-es2015": "^6.16.0",
        "chai": "^3.5.0",
        "coveralls": "^2.11.16",
        "eslint": "^3.8.0",
        "eslint-config-airbnb": "^12.0.0",
        "eslint-plugin-import": "^1.16.0",
        "eslint-plugin-jsx-a11y": "^2.2.3",
        "eslint-plugin-react": "^6.4.1",
        "istanbul": "^1.1.0-alpha.1",
        "mocha": "^3.1.2",
        "opn-cli": "^3.1.0",
        "sinon": "^1.17.6"
    },
    "directories": {},
    "dist": {
        "shasum": "a54863b04879ef7f01f811ddc8c81db04f8e2bc3",
        "tarball": "https://registry.npmjs.org/node-pushnotifications/-/node-pushnotifications-1.0.18.tgz"
    },
    "engines": {
        "node": ">= 4.6.0"
    },
    "eslintConfig": {
        "ecmaVersion": 6,
        "env": {
            "es6": true,
            "node": true
        }
    },
    "gitHead": "94306de4310e9fbe37f2149c754a8e263b9c4a7e",
    "homepage": "https://github.com/appfeel/node-pushnotifications",
    "keywords": [
        "notifications",
        "push",
        "push notifications",
        "apple",
        "ios",
        "iphone",
        "ipad",
        "apns",
        "google",
        "android",
        "gcm",
        "fcm",
        "amazon",
        "kindle",
        "adm",
        "microsoft",
        "windows",
        "wphone",
        "windows phone",
        "wns",
        "mpns"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "appfeel"
        }
    ],
    "name": "node-pushnotifications",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/appfeel/node-pushnotifications.git"
    },
    "scripts": {
        "build": "babel src -d lib",
        "coveralls": "cat ./coverage/lcov.info | coveralls",
        "lint": "eslint src/**/*.js",
        "prepublish": "npm run lint && npm test && npm run build",
        "test": "istanbul cover ./node_modules/.bin/_mocha -- test/ --compilers jsx:babel-core/register --recursive --report lcovonly",
        "test-alone": "_mocha test/ --compilers jsx:babel-core/register --recursive -w",
        "test-cover": "istanbul cover ./node_modules/.bin/_mocha -- test/ --compilers jsx:babel-core/register --recursive; opn ./coverage/lcov-report/index.html"
    },
    "version": "1.0.18",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
