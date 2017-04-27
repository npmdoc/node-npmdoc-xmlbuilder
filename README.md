# npmdoc-xmlbuilder

#### basic api documentation for  [xmlbuilder (v8.2.2)](http://github.com/oozcitak/xmlbuilder-js)  [![npm package](https://img.shields.io/npm/v/npmdoc-xmlbuilder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xmlbuilder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xmlbuilder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xmlbuilder)

#### An XML builder for node.js

[![NPM](https://nodei.co/npm/xmlbuilder.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/xmlbuilder)

- [https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xmlbuilder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ozgur Ozcitak"
    },
    "bugs": {
        "url": "http://github.com/oozcitak/xmlbuilder-js/issues"
    },
    "contributors": [],
    "dependencies": {},
    "description": "An XML builder for node.js",
    "devDependencies": {
        "coffee-coverage": "*",
        "coffee-script": "*",
        "coveralls": "*",
        "istanbul": "*",
        "mocha": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "69248673410b4ba42e1a6136551d2922335aa773",
        "tarball": "https://registry.npmjs.org/xmlbuilder/-/xmlbuilder-8.2.2.tgz"
    },
    "engines": {
        "node": ">=4.0"
    },
    "gitHead": "ab5987b12bc06e4da8c37cd7fec8f93085d96d28",
    "homepage": "http://github.com/oozcitak/xmlbuilder-js",
    "keywords": [
        "xml",
        "xmlbuilder"
    ],
    "license": "MIT",
    "main": "./lib/index",
    "maintainers": [
        {
            "name": "oozcitak"
        }
    ],
    "name": "xmlbuilder",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/oozcitak/xmlbuilder-js.git"
    },
    "scripts": {
        "postpublish": "rm -rf lib",
        "prepublish": "coffee -co lib src",
        "test": "mocha && istanbul report text lcov"
    },
    "version": "8.2.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
