# npmtest-vuex-persistedstate

#### basic test coverage for  [vuex-persistedstate (v1.4.0)](https://github.com/robinvdvleuten/vuex-persistedstate#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-vuex-persistedstate.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-vuex-persistedstate) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-vuex-persistedstate.svg)](https://travis-ci.org/npmtest/node-npmtest-vuex-persistedstate)

#### Persist Vuex state with localStorage.

[![NPM](https://nodei.co/npm/vuex-persistedstate.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/vuex-persistedstate)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-vuex-persistedstate/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-vuex-persistedstate/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-vuex-persistedstate/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-vuex-persistedstate/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/test-report.html](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-vuex-persistedstate/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-vuex-persistedstate/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vuex-persistedstate/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vuex-persistedstate/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-vuex-persistedstate/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Robin van der Vleuten"
    },
    "ava": {
        "require": [
            "./test/helpers/setup.js"
        ]
    },
    "bugs": {
        "url": "https://github.com/robinvdvleuten/vuex-persistedstate/issues"
    },
    "dependencies": {
        "husky": "^0.13.3",
        "lodash.merge": "^4.6.0",
        "object-path": "^0.11.2"
    },
    "description": "Persist Vuex state with localStorage.",
    "devDependencies": {
        "ava": "^0.17.0",
        "browser-env": "^2.0.16",
        "dom-storage": "^2.0.2",
        "eslint": "^3.11.1",
        "lint-staged": "^3.4.0",
        "prettier": "^1.1.0",
        "rollup": "^0.36.0",
        "rollup-plugin-buble": "^0.14.0",
        "sinon": "^1.17.6",
        "uglify-js": "^2.7.3",
        "vue": "^2.0.0",
        "vuex": "^2.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "1b1cd9c1244d4a97bbb2f805cf77824b89f8ad6f",
        "tarball": "https://registry.npmjs.org/vuex-persistedstate/-/vuex-persistedstate-1.4.0.tgz"
    },
    "files": [
        "dist/vuex-persistedstate.js",
        "dist/vuex-persistedstate.min.js",
        "src",
        "LICENSE",
        "README.md"
    ],
    "gitHead": "6febfa0f95864a539510ba8c90722751bc6ce399",
    "homepage": "https://github.com/robinvdvleuten/vuex-persistedstate#readme",
    "keywords": [
        "vue",
        "vuex",
        "plugin"
    ],
    "license": "MIT",
    "lint-staged": {
        "src/**/*.js": [
            "prettier --single-quote --write",
            "git add"
        ]
    },
    "main": "dist/vuex-persistedstate.js",
    "maintainers": [
        {
            "name": "robinvdvleuten"
        }
    ],
    "name": "vuex-persistedstate",
    "optionalDependencies": {},
    "peerDependencies": {
        "vue": "^2.0.0",
        "vuex": "^2.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/robinvdvleuten/vuex-persistedstate.git"
    },
    "scripts": {
        "build": "rollup --environment NODE_ENV:production -c build/rollup.config.js && uglifyjs dist/vuex-persistedstate.js --comments -o dist/vuex-persistedstate.min.js",
        "precommit": "npm run build && lint-staged",
        "prepublish": "npm run build",
        "test": "npm run build && ava --serial"
    },
    "version": "1.4.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
