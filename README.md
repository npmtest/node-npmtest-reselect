# npmtest-reselect

#### basic test coverage for  [reselect (v3.0.0)](https://github.com/reactjs/reselect#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-reselect.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-reselect) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-reselect.svg)](https://travis-ci.org/npmtest/node-npmtest-reselect)

#### Selectors for Redux.

[![NPM](https://nodei.co/npm/reselect.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/reselect)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-reselect/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-reselect/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-reselect/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-reselect/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-reselect/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-reselect/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-reselect/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-reselect/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-reselect/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-reselect/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-reselect/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-reselect/build/test-report.html](https://npmtest.github.io/node-npmtest-reselect/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-reselect/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-reselect/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-reselect/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-reselect/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-reselect/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-reselect/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-reselect/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-reselect/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "authors": [
        "Lee Bannard",
        "Robert Binna",
        "Martijn Faassen",
        "Philip Spitzlinger"
    ],
    "betterScripts": {
        "test": {
            "command": "mocha --compilers js:babel-register --ui tdd --recursive",
            "env": {
                "NODE_ENV": "test"
            }
        },
        "test:cov": {
            "command": "nyc --reporter=lcov --reporter=text mocha --compilers js:babel-register --ui tdd",
            "env": {
                "NODE_ENV": "test",
                "COVERAGE": "true"
            }
        },
        "test:typescript": {
            "command": "typings-tester --dir typescript_test"
        },
        "compile:commonjs": {
            "command": "babel -d lib/ src/ && ncp ./src/index.d.ts ./lib/index.d.ts",
            "env": {
                "NODE_ENV": "commonjs"
            }
        },
        "compile:umd": {
            "command": "mkdirp dist/ && babel -o dist/reselect.js src/",
            "env": {
                "NODE_ENV": "umd"
            }
        }
    },
    "bugs": {
        "url": "https://github.com/reactjs/reselect/issues"
    },
    "contributors": [
        {
            "name": "Lee Bannard",
            "url": "https://github.com/ellbee"
        },
        {
            "name": "Martijn Faassen",
            "url": "https://github.com/faassen"
        },
        {
            "name": "Ian Ker-Seymer",
            "url": "https://github.com/ianks"
        },
        {
            "name": "Mike S",
            "url": "https://github.com/SpainTrain"
        },
        {
            "name": "Daniel Bugl",
            "url": "https://github.com/omnidan"
        },
        {
            "name": "Ryan",
            "url": "https://github.com/ryanatkn"
        },
        {
            "name": "Alex Guerra",
            "url": "https://github.com/HeyImAlex"
        },
        {
            "name": "speedskater",
            "url": "https://github.com/speedskater"
        },
        {
            "name": "Daniela Borges",
            "url": "https://github.com/sericaia"
        },
        {
            "name": "Brian Ng",
            "url": "https://github.com/existentialism"
        },
        {
            "name": "C. T. Lin",
            "url": "https://github.com/chentsulin"
        },
        {
            "name": "Jay",
            "url": "https://github.com/chungchiehlun"
        },
        {
            "name": "Christian Schuhmann",
            "url": "https://github.com/madebyherzblut"
        },
        {
            "name": "Daniel Barreto",
            "url": "https://github.com/volrath"
        },
        {
            "name": "Adam Royle",
            "url": "https://github.com/ifunk"
        },
        {
            "name": "Elliot Crosby-McCullough",
            "url": "https://github.com/elliotcm"
        },
        {
            "name": "frankwallis",
            "url": "https://github.com/frankwallis"
        },
        {
            "name": "Jason Huang",
            "url": "https://github.com/kaddopur"
        },
        {
            "name": "Josh Kelley",
            "url": "https://github.com/joshkel"
        },
        {
            "name": "Leon Aves",
            "url": "https://github.com/leonaves"
        },
        {
            "name": "Mark Dalgleish",
            "url": "https://github.com/markdalgleish"
        },
        {
            "name": "Max Goodman",
            "url": "https://github.com/chromakode"
        },
        {
            "name": "Michael Lancaster",
            "url": "https://github.com/weblancaster"
        },
        {
            "name": "Mihail Diordiev",
            "url": "https://github.com/zalmoxisus"
        },
        {
            "name": "PSpSynedra",
            "url": "https://github.com/PSpSynedra"
        },
        {
            "name": "Simen Bekkhus",
            "url": "https://github.com/SimenB"
        },
        {
            "name": "Wade Peterson",
            "url": "https://github.com/WadePeterson"
        },
        {
            "name": "长天之云",
            "url": "https://github.com/ambar"
        },
        {
            "name": "Courtland Allen",
            "url": "https://github.com/courthead"
        },
        {
            "name": "Henrik Joreteg",
            "url": "https://github.com/HenrikJoreteg"
        },
        {
            "name": "Kyle Davis",
            "url": "https://github.com/kyldvs"
        },
        {
            "name": "Salvador Hernandez",
            "url": "https://github.com/clickclickonsal"
        },
        {
            "name": "Nick Ball",
            "url": "https://github.com/npbee"
        },
        {
            "name": "mctep",
            "url": "https://github.com/mctep"
        },
        {
            "name": "Jacob Rask",
            "url": "https://github.com/jacobrask"
        },
        {
            "name": "Luqmaan Dawoodjee",
            "url": "https://github.com/luqmaan"
        },
        {
            "name": "Walter Breakell",
            "url": "https://github.com/wbreakell"
        },
        {
            "name": "Matthew Hetherington",
            "url": "https://github.com/matthetherington"
        },
        {
            "name": "Mike Wilcox",
            "url": "https://github.com/mjw56"
        },
        {
            "name": "David Edmondson",
            "url": "https://github.com/threehams"
        },
        {
            "name": "Andrey Zaytsev",
            "url": "https://github.com/zandroid"
        },
        {
            "name": "1ven",
            "url": "https://github.com/1ven"
        },
        {
            "name": "Alexey Yurchenko",
            "url": "https://github.com/alexesdev"
        },
        {
            "name": "Douglas Russell",
            "url": "https://github.com/dpwrussell"
        },
        {
            "name": "Yonatan Kogan",
            "url": "https://github.com/yoni-tock"
        },
        {
            "name": "Peter Petrov",
            "url": "https://github.com/pesho"
        },
        {
            "name": "Walter Breakell",
            "url": "https://github.com/wbreakell"
        },
        {
            "name": "Whien",
            "url": "https://github.com/madeinfree"
        },
        {
            "name": "Sergei Egorov",
            "url": "https://github.com/bsideup"
        },
        {
            "name": "Jim Bolla",
            "url": "https://github.com/jimbolla"
        },
        {
            "name": "Carl Bernardo",
            "url": "https://github.com/carlbernrdo"
        },
        {
            "name": "Daniel Lytkin",
            "url": "https://github.com/aikoven"
        },
        {
            "name": "John Haley",
            "url": "https://github.com/johnhaley81"
        },
        {
            "name": "Alexandre",
            "url": "https://github.com/alex3165"
        }
    ],
    "dependencies": {},
    "description": "Selectors for Redux.",
    "devDependencies": {
        "babel-cli": "^6.7.5",
        "babel-plugin-check-es2015-constants": "^6.7.2",
        "babel-plugin-transform-es2015-arrow-functions": "^6.5.2",
        "babel-plugin-transform-es2015-block-scoping": "^6.7.1",
        "babel-plugin-transform-es2015-function-name": "^6.5.0",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.7.4",
        "babel-plugin-transform-es2015-modules-umd": "^6.6.5",
        "babel-plugin-transform-es2015-parameters": "^6.7.0",
        "babel-plugin-transform-es2015-shorthand-properties": "^6.5.0",
        "babel-plugin-transform-es2015-spread": "^6.6.5",
        "babel-plugin-transform-es2015-template-literals": "^6.6.5",
        "babel-register": "^6.7.2",
        "better-npm-run": "0.0.8",
        "chai": "^3.0.0",
        "codecov.io": "^0.1.6",
        "coveralls": "^2.11.4",
        "eslint": "^2.11",
        "eslint-plugin-react": "^5.1.1",
        "lodash.memoize": "^4.1.0",
        "mkdirp": "^0.5.1",
        "mocha": "^2.2.5",
        "ncp": "^2.0.0",
        "nyc": "^6.4.0",
        "typescript": "^2.1.4",
        "typings-tester": "^0.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b2e35977f03048700028eaee3a8c0639e40e8f35",
        "tarball": "https://registry.npmjs.org/reselect/-/reselect-3.0.0.tgz"
    },
    "files": [
        "lib",
        "src",
        "dist",
        "es"
    ],
    "gitHead": "48e22889a3e185427387ff1da8e838591671effb",
    "homepage": "https://github.com/reactjs/reselect#readme",
    "jsnext:main": "es/index.js",
    "keywords": [
        "react",
        "redux"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "alex3165"
        },
        {
            "name": "ellbee"
        },
        {
            "name": "faassen"
        },
        {
            "name": "gaearon"
        },
        {
            "name": "threehams"
        }
    ],
    "name": "reselect",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/reactjs/reselect.git"
    },
    "scripts": {
        "compile": "npm run compile:commonjs && npm run compile:umd && npm run compile:es",
        "compile:commonjs": "better-npm-run compile:commonjs",
        "compile:es": "babel -d es/ src/",
        "compile:umd": "better-npm-run compile:umd",
        "lint": "eslint src test",
        "prepublish": "npm run compile",
        "test": "better-npm-run test",
        "test:cov": "better-npm-run test:cov",
        "test:typescript": "better-npm-run test:typescript"
    },
    "typings": "lib/index.d.ts",
    "version": "3.0.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
