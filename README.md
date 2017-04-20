# npmdoc-node-geocoder

#### api documentation for  node-geocoder (v3.16.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-geocoder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-geocoder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-geocoder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-geocoder)

#### Node Geocoder, node geocoding library, supports google maps, mapquest, open street map, tom tom, promise

[![NPM](https://nodei.co/npm/node-geocoder.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-geocoder)

- [https://npmdoc.github.io/node-npmdoc-node-geocoder/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "node-geocoder",
    "version": "3.16.0",
    "description": "Node Geocoder, node geocoding library, supports google maps, mapquest, open street map, tom tom, promise",
    "main": "index.js",
    "scripts": {
        "test": "mocha --check-leaks",
        "lint": "eslint lib",
        "ci": "npm run lint && npm run test"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/nchaulet/node-geocoder.git"
    },
    "keywords": [
        "geocoder",
        "geocoding",
        "geo",
        "google",
        "maps",
        "mapquest",
        "agol",
        "arcgis",
        "tomtom"
    ],
    "author": "nchaulet",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/nchaulet/node-geocoder/issues"
    },
    "dependencies": {
        "bluebird": "^3.4.6",
        "request": "^2.74.0",
        "request-promise": "^4.1.1"
    },
    "devDependencies": {
        "chai": "^3.5.0",
        "eslint": "^3.11.0",
        "mocha": "^3.2.0",
        "sinon": "^1.17.3"
    },
    "eslintConfig": {
        "env": {
            "node": true
        },
        "rules": {
            "strict": 0,
            "quotes": [
                1,
                "single"
            ],
            "no-console": 1,
            "camelcase": 0,
            "no-underscore-dangle": 0,
            "no-shadow": 0,
            "no-multi-spaces": 0,
            "eqeqeq": 0,
            "key-spacing": 0,
            "comma-spacing": 0,
            "no-unreachable": 1
        }
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
