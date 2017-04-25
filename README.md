# npmdoc-cson

#### basic api documentation for  [cson (v4.1.0)](https://github.com/bevry/cson)  [![npm package](https://img.shields.io/npm/v/npmdoc-cson.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cson) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cson.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cson)

#### CoffeeScript-Object-Notation Parser. Same as JSON but for CoffeeScript objects.

[![NPM](https://nodei.co/npm/cson.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cson)

- [https://npmdoc.github.io/node-npmdoc-cson/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-cson/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cson/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cson/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cson/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cson/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "2012+ Bevry Pty Ltd",
        "url": "http://bevry.me"
    },
    "badges": {
        "list": [
            "travisci",
            "npmversion",
            "npmdownloads",
            "daviddm",
            "daviddmdev",
            "---",
            "patreon",
            "opencollective",
            "gratipay",
            "flattr",
            "paypal",
            "bitcoin",
            "wishlist",
            "---",
            "slackin"
        ],
        "config": {
            "patreonUsername": "bevry",
            "opencollectiveUsername": "bevry",
            "gratipayUsername": "bevry",
            "flattrUsername": "balupton",
            "paypalURL": "https://bevry.me/paypal",
            "bitcoinURL": "https://bevry.me/bitcoin",
            "wishlistURL": "https://bevry.me/wishlist",
            "slackinURL": "https://slack.bevry.me"
        }
    },
    "bin": {
        "cson2json": "bin/cson2json",
        "json2cson": "bin/json2cson"
    },
    "bugs": {
        "url": "https://github.com/bevry/cson/issues"
    },
    "contributors": [
        {
            "name": "Benjamin Lupton",
            "url": "http://balupton.com"
        },
        {
            "name": "Attila Oláh",
            "url": "http://attilaolah.eu/"
        },
        {
            "name": "evinugur",
            "url": "https://github.com/evinugur"
        },
        {
            "name": "Jason Karns",
            "url": "http://jasonkarns.com"
        },
        {
            "name": "Joël Perras",
            "url": "http://nerderati.com"
        },
        {
            "name": "Linus Gustav Larsson Thiel",
            "url": "http://yesbabyyes.se/"
        },
        {
            "name": "Tushar Kant",
            "url": "https://github.com/nanuclickity"
        },
        {
            "name": "Claudius Nicolae",
            "url": "https://github.com/clyfe"
        },
        {
            "name": "Rob Loach",
            "url": "http://robloach.net"
        },
        {
            "name": "Ryan LeFevre",
            "url": "http://meltingice.net"
        },
        {
            "name": "Zearin",
            "url": "https://github.com/Zearin"
        },
        {
            "name": "ZHANG Cheng",
            "url": "http://about.me/zhangcheng77"
        }
    ],
    "dependencies": {
        "coffee-script": "^1.12.4",
        "cson-parser": "^1.3.4",
        "extract-opts": "^3.3.1",
        "requirefresh": "^2.1.0",
        "safefs": "^4.1.0"
    },
    "description": "CoffeeScript-Object-Notation Parser. Same as JSON but for CoffeeScript objects.",
    "devDependencies": {
        "assert-helpers": "^4.5.0",
        "biscotto": "github:emmenko/biscotto#v2.4.0",
        "coffeelint": "^1.16.0",
        "joe": "^2.0.2",
        "joe-reporter-console": "^2.0.1",
        "projectz": "^1.4.0",
        "safeps": "^6.3.0",
        "surge": "^0.19.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b1075344fa9d9fe5cf88d80f21d9366296b865c7",
        "tarball": "https://registry.npmjs.org/cson/-/cson-4.1.0.tgz"
    },
    "editions": [
        {
            "description": "Source + CoffeeScript + Require",
            "directory": "source",
            "entry": "index.js",
            "syntaxes": [
                "coffeescript",
                "require"
            ]
        },
        {
            "description": "CoffeeScript Compiled + ES5 + Require",
            "directory": "es5",
            "entry": "index.js",
            "syntaxes": [
                "javascript",
                "es5",
                "require"
            ]
        }
    ],
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "0e913a90be66b2f29d2d75433b06ed52e83ba810",
    "homepage": "https://github.com/bevry/cson",
    "keywords": [
        "javascript",
        "coffeescript",
        "json",
        "cson",
        "parse",
        "stringify"
    ],
    "license": "MIT",
    "main": "es5/index.js",
    "maintainers": [
        {
            "name": "balupton"
        },
        {
            "name": "bevryme"
        }
    ],
    "name": "cson",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/bevry/cson.git"
    },
    "scripts": {
        "our:clean": "rm -Rf ./docs ./es2015 ./es5 ./out",
        "our:compile": "npm run our:compile:coffee",
        "our:compile:coffee": "coffee -bco ./es5 ./source",
        "our:meta": "npm run our:meta:projectz && npm run our:meta:biscotto",
        "our:meta:biscotto": "biscotto -n \"$npm_package_title\" --title \"$npm_package_title API Documentation\" --readme README.md --output-dir docs source - LICENSE.md HISTORY.md",
        "our:meta:projectz": "projectz compile",
        "our:release": "npm run our:release:prepare && npm run our:release:check && npm run our:release:tag && npm run our:release:push",
        "our:release:check": "npm run our:release:check:changelog && npm run our:release:check:dirty",
        "our:release:check:changelog": "cat ./HISTORY.md | grep v$npm_package_version || (echo add a changelog entry for v$npm_package_version && exit -1)",
        "our:release:check:dirty": "git diff --exit-code",
        "our:release:prepare": "npm run our:clean && npm run our:compile && npm run our:test && npm run our:meta",
        "our:release:push": "git push origin master && git push origin --tags",
        "our:release:tag": "export MESSAGE=$(cat ./HISTORY.md | sed -n \"/## v$npm_package_version/,/##/p\" | sed 's/## //' | awk 'NR>1{print buf}{buf = $0}') && test \"$MESSAGE\" || (echo 'proper changelog entry not found' && exit -1) && git tag v$npm_package_version -am \"$MESSAGE\"",
        "our:setup": "npm run our:setup:npm",
        "our:setup:npm": "npm install",
        "our:test": "npm run our:verify && npm test",
        "our:verify": "npm run our:verify:coffeelint",
        "our:verify:coffeelint": "coffeelint ./source",
        "test": "node --harmony es5/test.js --joe-reporter=console"
    },
    "title": "CSON",
    "version": "4.1.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
