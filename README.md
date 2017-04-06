# api documentation for  [cson (v4.0.0)](https://github.com/bevry/cson)  [![npm package](https://img.shields.io/npm/v/npmdoc-cson.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cson) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cson.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cson)
#### CoffeeScript-Object-Notation Parser. Same as JSON but for CoffeeScript objects.

[![NPM](https://nodei.co/npm/cson.png?downloads=true)](https://www.npmjs.com/package/cson)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cson/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cson_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cson/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cson/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cson/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "2012+ Bevry Pty Ltd",
        "email": "us@bevry.me",
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
            "slackin",
            "patreon",
            "gratipay",
            "flattr",
            "paypal",
            "bitcoin",
            "wishlist"
        ],
        "config": {
            "patreonUsername": "bevry",
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
            "email": "b@lupton.cc",
            "url": "http://balupton.com"
        },
        {
            "name": "Attila Oláh",
            "email": "attilaolah@google.com",
            "url": "http://attilaolah.eu/"
        },
        {
            "name": "evinugur",
            "url": "https://github.com/evinugur"
        },
        {
            "name": "Jason Karns",
            "email": "jason@karns.name",
            "url": "http://jasonkarns.com"
        },
        {
            "name": "Joël Perras",
            "email": "joel@nerderati.com",
            "url": "http://nerderati.com"
        },
        {
            "name": "Linus Gustav Larsson Thiel",
            "email": "linus@hanssonlarsson.se",
            "url": "http://yesbabyyes.se/"
        },
        {
            "name": "Tushar Kant",
            "email": "nanu.clickity@gmail.com",
            "url": "https://github.com/nanuclickity"
        },
        {
            "name": "Claudius Nicolae",
            "email": "claudius.nicolae@gmail.com",
            "url": "https://github.com/clyfe"
        },
        {
            "name": "Rob Loach",
            "email": "robloach@gmail.com",
            "url": "http://robloach.net"
        },
        {
            "name": "Ryan LeFevre",
            "email": "meltingice8917@gmail.com",
            "url": "http://meltingice.net"
        },
        {
            "name": "Zearin",
            "url": "https://github.com/Zearin"
        },
        {
            "name": "ZHANG Cheng",
            "email": "czhang.oss@gmail.com",
            "url": "http://about.me/zhangcheng77"
        }
    ],
    "dependencies": {
        "coffee-script": "^1.11.1",
        "cson-parser": "^1.3.4",
        "extract-opts": "^3.3.1",
        "requirefresh": "^2.1.0",
        "safefs": "^4.1.0"
    },
    "description": "CoffeeScript-Object-Notation Parser. Same as JSON but for CoffeeScript objects.",
    "devDependencies": {
        "assert-helpers": "^4.4.0",
        "biscotto": "^2.3.1",
        "coffeelint": "^1.16.0",
        "joe": "^1.8.0",
        "joe-reporter-console": "^1.2.1",
        "projectz": "^1.3.0",
        "safeps": "^6.3.0"
    },
    "directories": {},
    "dist": {
        "shasum": "61fe6d6e2e5653f6be5013dede74afe462586a52",
        "tarball": "https://registry.npmjs.org/cson/-/cson-4.0.0.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "0443cdfdfe7d76def631c95977ee17cdc093b062",
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
            "name": "balupton",
            "email": "b@lupton.cc"
        }
    ],
    "name": "cson",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/bevry/cson.git"
    },
    "scripts": {
        "clean": "rm -Rf ./docs ./es5",
        "compile": "npm run compile:coffeescript",
        "compile:coffeescript": "coffee -bco ./es5 ./src",
        "meta": "npm run meta:projectz",
        "meta:projectz": "projectz compile",
        "prepare": "npm run compile && npm run test && npm run meta",
        "pretest": "npm run test:coffeelint",
        "release": "npm run prepare && npm run release:publish && npm run release:tag && npm run release:push",
        "release:publish": "npm publish",
        "release:push": "git push origin master && git push origin --tags",
        "release:tag": "git tag v$npm_package_version -a",
        "setup": "npm install",
        "test:coffeelint": "coffeelint ./src"
    },
    "title": "CSON",
    "version": "4.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cson](#apidoc.module.cson)



# <a name="apidoc.module.cson"></a>[module cson](#apidoc.module.cson)



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
