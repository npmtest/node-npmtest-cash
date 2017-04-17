# test coverage for  [cash (v0.8.0)](https://github.com/dthree/cash#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-cash.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-cash) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-cash.svg)](https://travis-ci.org/npmtest/node-npmtest-cash)
#### Cross-platform Linux commands in pure ES6.

[![NPM](https://nodei.co/npm/cash.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cash)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-cash/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-cash/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-cash/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-cash/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-cash/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-cash/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-cash/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-cash/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-cash/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-cash/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-cash/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-cash/build/test-report.html](https://npmtest.github.io/node-npmtest-cash/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-cash/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-cash/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-cash/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cash/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cash/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cash/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-cash/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-cash/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "dthree"
    },
    "bin": {
        "$": "./bin/cash.js",
        "cash": "./bin/cash.js"
    },
    "bugs": {
        "url": "https://github.com/dthree/cash/issues"
    },
    "dependencies": {
        "array-shuffle": "^1.0.0",
        "chalk": "^1.1.0",
        "filesize": "^3.1.3",
        "fkill": "^3.1.0",
        "fs-extra": "^0.23.1",
        "glob": "^6.0.4",
        "lodash": "^4.0.0",
        "minimist": "^1.2.0",
        "user-home": "^2.0.0",
        "username": "^1.0.1",
        "vorpal": "^1.10.8",
        "vorpal-autocomplete-fs": "0.0.3",
        "vorpal-grep": "^0.1.2",
        "vorpal-less": "0.0.13"
    },
    "description": "Cross-platform Linux commands in pure ES6.",
    "devDependencies": {
        "babel-core": "^6.5.2",
        "babel-preset-es2015": "^6.5.0",
        "coveralls": "^2.11.6",
        "gulp": "^3.9.0",
        "gulp-babel": "^6.1.2",
        "gulp-changed": "^1.3.0",
        "gulp-eslint": "^2.0.0",
        "istanbul": "^0.4.2",
        "mocha": "^2.2.5",
        "shelljs": "^0.6.0",
        "should": "^7.0.3",
        "webpack": "^1.12.13",
        "xo": "^0.12.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0a0b289e87abccb30c504b006b6f975b8955c16b",
        "tarball": "https://registry.npmjs.org/cash/-/cash-0.8.0.tgz"
    },
    "engines": {
        "iojs": ">= 1.0.0",
        "node": ">= 4"
    },
    "files": [
        "commands.json",
        "dist",
        "bin"
    ],
    "gitHead": "e0e21e1a193adef6cb8a9cd6965d94d0fd34f939",
    "homepage": "https://github.com/dthree/cash#readme",
    "keywords": [
        "terminal",
        "emulator",
        "cygwin",
        "cli",
        "windows",
        "linux",
        "unix",
        "posix",
        "shell",
        "shelljs",
        "bash",
        "cash",
        "$",
        "tty",
        "util",
        "vorpal",
        "vorpal.js"
    ],
    "license": "MIT",
    "main": "./dist/index.js",
    "maintainers": [
        {
            "name": "aseemk"
        },
        {
            "name": "dthree"
        }
    ],
    "name": "cash",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dthree/cash.git"
    },
    "scripts": {
        "lint": "xo ./src/*.js ./src/**/*.js ./test/*.js",
        "test": "gulp builder; ./node_modules/istanbul/lib/cli.js cover --root './dist' -x './dist/lib/sugar.js' _mocha -- -R spec && npm run lint",
        "test-win": "mocha"
    },
    "version": "0.8.0",
    "xo": {
        "envs": [
            "node",
            "mocha"
        ],
        "space": true,
        "esnext": true,
        "rules": {
            "prefer-arrow-callback": 0,
            "no-loop-func": 0,
            "no-nested-ternary": 0,
            "no-constant-condition": 0,
            "no-use-extend-native/no-use-extend-native": 0,
            "no-negated-condition": 0,
            "no-inner-declarations": 0,
            "prefer-reflect": 0,
            "wrap-iife": 0,
            "no-unused-expressions": 0,
            "global-require": 0
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
