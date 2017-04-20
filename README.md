# npmdoc-xmlbuilder

#### api documentation for  [xmlbuilder (v8.2.2)](http://github.com/oozcitak/xmlbuilder-js)  [![npm package](https://img.shields.io/npm/v/npmdoc-xmlbuilder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xmlbuilder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xmlbuilder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xmlbuilder)

#### An XML builder for node.js

[![NPM](https://nodei.co/npm/xmlbuilder.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/xmlbuilder)

- [https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "xmlbuilder",
    "version": "8.2.2",
    "keywords": [
        "xml",
        "xmlbuilder"
    ],
    "homepage": "http://github.com/oozcitak/xmlbuilder-js",
    "description": "An XML builder for node.js",
    "author": "Ozgur Ozcitak <oozcitak@gmail.com>",
    "contributors": [],
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "git://github.com/oozcitak/xmlbuilder-js.git"
    },
    "bugs": {
        "url": "http://github.com/oozcitak/xmlbuilder-js/issues"
    },
    "main": "./lib/index",
    "engines": {
        "node": ">=4.0"
    },
    "dependencies": {},
    "devDependencies": {
        "coffee-script": "*",
        "mocha": "*",
        "coffee-coverage": "*",
        "istanbul": "*",
        "coveralls": "*"
    },
    "scripts": {
        "prepublish": "coffee -co lib src",
        "postpublish": "rm -rf lib",
        "test": "mocha && istanbul report text lcov"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
