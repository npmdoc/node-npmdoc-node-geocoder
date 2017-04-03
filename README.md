# api documentation for  [node-geocoder (v3.16.0)](https://github.com/nchaulet/node-geocoder#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-geocoder.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-geocoder) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-geocoder.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-geocoder)
#### Node Geocoder, node geocoding library, supports google maps, mapquest, open street map, tom tom, promise

[![NPM](https://nodei.co/npm/node-geocoder.png?downloads=true)](https://www.npmjs.com/package/node-geocoder)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-geocoder_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-geocoder/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-geocoder/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "nchaulet"
    },
    "bugs": {
        "url": "https://github.com/nchaulet/node-geocoder/issues"
    },
    "dependencies": {
        "bluebird": "^3.4.6",
        "request": "^2.74.0",
        "request-promise": "^4.1.1"
    },
    "description": "Node Geocoder, node geocoding library, supports google maps, mapquest, open street map, tom tom, promise",
    "devDependencies": {
        "chai": "^3.5.0",
        "eslint": "^3.11.0",
        "mocha": "^3.2.0",
        "sinon": "^1.17.3"
    },
    "directories": {},
    "dist": {
        "shasum": "6aa520c06f46fdf723838c0172b61eb646ea7921",
        "tarball": "https://registry.npmjs.org/node-geocoder/-/node-geocoder-3.16.0.tgz"
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
    },
    "gitHead": "0a1ab93af3bc5eaa215fee82946daa255af0c0f3",
    "homepage": "https://github.com/nchaulet/node-geocoder#readme",
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
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "nchaulet",
            "email": "n.chaulet@gmail.com"
        }
    ],
    "name": "node-geocoder",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nchaulet/node-geocoder.git"
    },
    "scripts": {
        "ci": "npm run lint && npm run test",
        "lint": "eslint lib",
        "test": "mocha --check-leaks"
    },
    "version": "3.16.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-geocoder](#apidoc.module.node-geocoder)
1.  [function <span class="apidocSignatureSpan">node-geocoder.</span>geocoder (geocoder, formatter)](#apidoc.element.node-geocoder.geocoder)
1.  object <span class="apidocSignatureSpan">node-geocoder.</span>geocoder.prototype
1.  object <span class="apidocSignatureSpan">node-geocoder.</span>geocoderfactory
1.  object <span class="apidocSignatureSpan">node-geocoder.</span>helper

#### [module node-geocoder.geocoder](#apidoc.module.node-geocoder.geocoder)
1.  [function <span class="apidocSignatureSpan">node-geocoder.</span>geocoder (geocoder, formatter)](#apidoc.element.node-geocoder.geocoder.geocoder)

#### [module node-geocoder.geocoder.prototype](#apidoc.module.node-geocoder.geocoder.prototype)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>_filter (value, data)](#apidoc.element.node-geocoder.geocoder.prototype._filter)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>_format (data)](#apidoc.element.node-geocoder.geocoder.prototype._format)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>batchGeocode (values, callback)](#apidoc.element.node-geocoder.geocoder.prototype.batchGeocode)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>geocode (value, callback)](#apidoc.element.node-geocoder.geocoder.prototype.geocode)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>reverse (query, callback)](#apidoc.element.node-geocoder.geocoder.prototype.reverse)

#### [module node-geocoder.geocoderfactory](#apidoc.module.node-geocoder.geocoderfactory)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>_getFormatter (formatterName, extra)](#apidoc.element.node-geocoder.geocoderfactory._getFormatter)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>_getGeocoder (geocoderName, adapter, extra)](#apidoc.element.node-geocoder.geocoderfactory._getGeocoder)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>_getHttpAdapter (adapterName, options)](#apidoc.element.node-geocoder.geocoderfactory._getHttpAdapter)
1.  [function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>getGeocoder (geocoderAdapter, httpAdapter, extra)](#apidoc.element.node-geocoder.geocoderfactory.getGeocoder)

#### [module node-geocoder.helper](#apidoc.module.node-geocoder.helper)
1.  [function <span class="apidocSignatureSpan">node-geocoder.helper.</span>isString (testVar)](#apidoc.element.node-geocoder.helper.isString)



# <a name="apidoc.module.node-geocoder"></a>[module node-geocoder](#apidoc.module.node-geocoder)

#### <a name="apidoc.element.node-geocoder.geocoder"></a>[function <span class="apidocSignatureSpan">node-geocoder.</span>geocoder (geocoder, formatter)](#apidoc.element.node-geocoder.geocoder)
- description and source-code
```javascript
geocoder = function (geocoder, formatter) {
  this._geocoder = geocoder;
  this._formatter = formatter;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-geocoder.geocoder"></a>[module node-geocoder.geocoder](#apidoc.module.node-geocoder.geocoder)

#### <a name="apidoc.element.node-geocoder.geocoder.geocoder"></a>[function <span class="apidocSignatureSpan">node-geocoder.</span>geocoder (geocoder, formatter)](#apidoc.element.node-geocoder.geocoder.geocoder)
- description and source-code
```javascript
geocoder = function (geocoder, formatter) {
  this._geocoder = geocoder;
  this._formatter = formatter;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-geocoder.geocoder.prototype"></a>[module node-geocoder.geocoder.prototype](#apidoc.module.node-geocoder.geocoder.prototype)

#### <a name="apidoc.element.node-geocoder.geocoder.prototype._filter"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>_filter (value, data)](#apidoc.element.node-geocoder.geocoder.prototype._filter)
- description and source-code
```javascript
_filter = function (value, data) {
  if (!data || !data.length) {
    return data;
  }

  if (value.minConfidence) {
    data = data.filter(function(geocodedAddress) {
      if (geocodedAddress.extra && geocodedAddress.extra.confidence) {
        return geocodedAddress.extra.confidence >= value.minConfidence;
      }
    });
  }

  return data;
}
```
- example usage
```shell
...
    .bind(this)
    .then(function() {
      return BPromise.fromCallback(function(callback) {
        this._geocoder.geocode(value, callback);
      }.bind(this));
    })
    .then(function(data) {
      return this._filter(value, data);
    })
    .then(function(data) {
      return this._format(data);
    })
    .asCallback(callback);
};
...
```

#### <a name="apidoc.element.node-geocoder.geocoder.prototype._format"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>_format (data)](#apidoc.element.node-geocoder.geocoder.prototype._format)
- description and source-code
```javascript
_format = function (data) {
  var _this = this;
  return BPromise.resolve()
    .bind(this)
    .then(function() {
      if (!data) {
        return data;
      }

      var _raw = data.raw;

      data = data.map(function(result) {
        result.provider = _this._geocoder.name;

        return result;
      });

      data.raw = _raw;
      Object.defineProperty(data,'raw',{configurable:false, enumerable:false, writable:false});

      return data;
    })
    .then(function(data) {
      var _data = data;
      if (this._formatter && this._formatter !== 'undefined') {
        _data = this._formatter.format(_data);
      }

      return _data;
    });
}
```
- example usage
```shell
...
        this._geocoder.geocode(value, callback);
      }.bind(this));
    })
    .then(function(data) {
      return this._filter(value, data);
    })
    .then(function(data) {
      return this._format(data);
    })
    .asCallback(callback);
};

/**
* Reverse geocoding
* @param {lat:<number>,lon:<number>}  lat: Latitude, lon: Longitude
...
```

#### <a name="apidoc.element.node-geocoder.geocoder.prototype.batchGeocode"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>batchGeocode (values, callback)](#apidoc.element.node-geocoder.geocoder.prototype.batchGeocode)
- description and source-code
```javascript
batchGeocode = function (values, callback) {
  return BPromise.resolve(values)
    .bind(this)
    .map(function(value) {
      return this.geocode(value)
        .then(function(value) {
          return {
            error: null,
            value: value
          };
        })
        .catch(function(error) {
          return {
            error: error,
            value: null
          };
        });
    })
    .asCallback(callback);
}
```
- example usage
```shell
...
  })
  .catch(function(err) {
    console.log(err);
  });

// Batch geocode

geocoder.batchGeocode(['13 rue sainte catherine', 'another adress'], function (err, results) {
  // Return an array of type {error: false, value: []}
  console.log(results) ;
});

// Set specific http request headers:
var HttpsAdapter = require('node-geocoder/lib/httpadapter/httpsadapter.js')
var httpAdapter = new HttpsAdapter(null, {
...
```

#### <a name="apidoc.element.node-geocoder.geocoder.prototype.geocode"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>geocode (value, callback)](#apidoc.element.node-geocoder.geocoder.prototype.geocode)
- description and source-code
```javascript
geocode = function (value, callback) {
  return BPromise.resolve()
    .bind(this)
    .then(function() {
      return BPromise.fromCallback(function(callback) {
        this._geocoder.geocode(value, callback);
      }.bind(this));
    })
    .then(function(data) {
      return this._filter(value, data);
    })
    .then(function(data) {
      return this._format(data);
    })
    .asCallback(callback);
}
```
- example usage
```shell
...
apiKey: 'YOUR_API_KEY', // for Mapquest, OpenCage, Google Premier
formatter: null         // 'gpx', 'string', ...
};

var geocoder = NodeGeocoder(options);

// Using callback
geocoder.geocode('29 champs elysée paris', function(err, res) {
console.log(res);
});

// Or using Promise
geocoder.geocode('29 champs elysée paris')
.then(function(res) {
  console.log(res);
...
```

#### <a name="apidoc.element.node-geocoder.geocoder.prototype.reverse"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoder.prototype.</span>reverse (query, callback)](#apidoc.element.node-geocoder.geocoder.prototype.reverse)
- description and source-code
```javascript
reverse = function (query, callback) {
  return BPromise.resolve()
    .bind(this)
    .then(function() {
      return BPromise.fromCallback(function(callback) {
        this._geocoder.reverse(query, callback);
      }.bind(this));
    })
    .then(function(data) {
      return this._format(data);
    })
    .asCallback(callback);
}
```
- example usage
```shell
...
geocoder.geocode({address: '29 champs elysée', countryCode: 'fr', minConfidence: 0.5, limit: 5}, function(err, res) {
console.log(res);
});

// Reverse example

// Using callback
geocoder.reverse({lat:45.767, lon:4.833}, function(err, res) {
console.log(res);
});

// Or using Promise
geocoder.reverse({lat:45.767, lon:4.833})
.then(function(res) {
  console.log(res);
...
```



# <a name="apidoc.module.node-geocoder.geocoderfactory"></a>[module node-geocoder.geocoderfactory](#apidoc.module.node-geocoder.geocoderfactory)

#### <a name="apidoc.element.node-geocoder.geocoderfactory._getFormatter"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>_getFormatter (formatterName, extra)](#apidoc.element.node-geocoder.geocoderfactory._getFormatter)
- description and source-code
```javascript
_getFormatter = function (formatterName, extra) {
  if (formatterName === 'gpx') {
    var GpxFormatter = require('./formatter/gpxformatter.js');

    return new GpxFormatter();
  }

  if (formatterName === 'string') {
    var StringFormatter = require('./formatter/stringformatter.js');

    return new StringFormatter(extra.formatterPattern);
  }
}
```
- example usage
```shell
...
    if (Helper.isString(geocoderAdapter)) {
      geocoderAdapter = this._getGeocoder(geocoderAdapter, httpAdapter, extra);
    }

    var formatter = extra.formatter;

    if (Helper.isString(formatter)) {
      formatter = this._getFormatter(formatter, extra);
    }

    return new Geocoder(geocoderAdapter, formatter);
  }
};

module.exports = GeocoderFactory;
...
```

#### <a name="apidoc.element.node-geocoder.geocoderfactory._getGeocoder"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>_getGeocoder (geocoderName, adapter, extra)](#apidoc.element.node-geocoder.geocoderfactory._getGeocoder)
- description and source-code
```javascript
_getGeocoder = function (geocoderName, adapter, extra) {
  if (geocoderName === 'google') {
    return new GoogleGeocoder(adapter, {clientId: extra.clientId, apiKey: extra.apiKey, language: extra.language, region: extra.
region, excludePartialMatches: extra.excludePartialMatches, channel: extra.channel});
  }
  if (geocoderName === 'here') {
    return new HereGeocoder(adapter, {appId: extra.appId, appCode: extra.appCode, language: extra.language, politicalView: extra
.politicalView, country: extra.country, state: extra.state});
  }
  if (geocoderName === 'agol') {
    return new AGOLGeocoder(adapter, {client_id: extra.client_id, client_secret: extra.client_secret});
  }
  if (geocoderName === 'freegeoip') {
    return new FreegeoipGeocoder(adapter);
  }
  if (geocoderName === 'datasciencetoolkit') {
    return new DataScienceToolkitGeocoder(adapter, {host: extra.host});
  }
  if (geocoderName === 'openstreetmap') {
    return new OpenStreetMapGeocoder(adapter, {language: extra.language});
  }
  if (geocoderName === 'locationiq') {
    return new LocationIQGeocoder(adapter, extra.apiKey);
  }
  if (geocoderName === 'mapquest') {
    return new MapQuestGeocoder(adapter, extra.apiKey);
  }
  if (geocoderName === 'openmapquest') {
    return new OpenMapQuestGeocoder(adapter, extra.apiKey);
  }
  if (geocoderName === 'yandex') {
    return new YandexGeocoder(adapter, {language: extra.language});
  }
  if (geocoderName === 'geocodio') {
    return new GeocodioGeocoder(adapter, extra.apiKey);
  }
  if (geocoderName === 'opencage') {
    return new OpenCageGeocoder(adapter, extra.apiKey, extra);
  }
  if (geocoderName === 'nominatimmapquest') {
    return new NominatimMapquestGeocoder(adapter, {language: extra.language, apiKey: extra.apiKey});
  }
  if (geocoderName === 'tomtom') {
    return new TomTomGeocoder(adapter, {apiKey: extra.apiKey});
  }
  if (geocoderName === 'smartystreets') {
    return new SmartyStreets(adapter, extra.auth_id, extra.auth_token);
  }
  if (geocoderName === 'teleport') {
    return new TeleportGeocoder(adapter, extra.apiKey, extra);
  }
  if (geocoderName === 'opendatafrance') {
    return new OpendataFranceGeocoder(adapter);
  }

  throw new Error('No geocoder provider find for : ' + geocoderName);
}
```
- example usage
```shell
...
}

if (Helper.isString(httpAdapter)) {
  httpAdapter = this._getHttpAdapter(httpAdapter, extra);
}

if (Helper.isString(geocoderAdapter)) {
  geocoderAdapter = this._getGeocoder(geocoderAdapter, httpAdapter, extra);
}

var formatter = extra.formatter;

if (Helper.isString(formatter)) {
  formatter = this._getFormatter(formatter, extra);
}
...
```

#### <a name="apidoc.element.node-geocoder.geocoderfactory._getHttpAdapter"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>_getHttpAdapter (adapterName, options)](#apidoc.element.node-geocoder.geocoderfactory._getHttpAdapter)
- description and source-code
```javascript
_getHttpAdapter = function (adapterName, options) {
  if (adapterName === 'http') {
    return new HttpAdapter(null, options);
  }
  if (adapterName === 'https') {
    return new HttpsAdapter(null, options);
  }
  if (adapterName === 'request') {
    return new RequestAdapter(null, options);
  }
}
```
- example usage
```shell
...
}

if (!geocoderAdapter) {
  geocoderAdapter = 'google';
}

if (Helper.isString(httpAdapter)) {
  httpAdapter = this._getHttpAdapter(httpAdapter, extra);
}

if (Helper.isString(geocoderAdapter)) {
  geocoderAdapter = this._getGeocoder(geocoderAdapter, httpAdapter, extra);
}

var formatter = extra.formatter;
...
```

#### <a name="apidoc.element.node-geocoder.geocoderfactory.getGeocoder"></a>[function <span class="apidocSignatureSpan">node-geocoder.geocoderfactory.</span>getGeocoder (geocoderAdapter, httpAdapter, extra)](#apidoc.element.node-geocoder.geocoderfactory.getGeocoder)
- description and source-code
```javascript
getGeocoder = function (geocoderAdapter, httpAdapter, extra) {
  if (typeof geocoderAdapter === 'object') {
    extra = geocoderAdapter;
    geocoderAdapter = null;
    httpAdapter = null;
  }

  if (!extra) {
    extra = {};
  }

  if (extra.httpAdapter) {
    httpAdapter = extra.httpAdapter;
  }

  if (extra.provider) {
    geocoderAdapter = extra.provider;
  }

  if (!httpAdapter) {
    httpAdapter = 'https';
  }

  if (!geocoderAdapter) {
    geocoderAdapter = 'google';
  }

  if (Helper.isString(httpAdapter)) {
    httpAdapter = this._getHttpAdapter(httpAdapter, extra);
  }

  if (Helper.isString(geocoderAdapter)) {
    geocoderAdapter = this._getGeocoder(geocoderAdapter, httpAdapter, extra);
  }

  var formatter = extra.formatter;

  if (Helper.isString(formatter)) {
    formatter = this._getFormatter(formatter, extra);
  }

  return new Geocoder(geocoderAdapter, formatter);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-geocoder.helper"></a>[module node-geocoder.helper](#apidoc.module.node-geocoder.helper)

#### <a name="apidoc.element.node-geocoder.helper.isString"></a>[function <span class="apidocSignatureSpan">node-geocoder.helper.</span>isString (testVar)](#apidoc.element.node-geocoder.helper.isString)
- description and source-code
```javascript
isString = function (testVar) {
  return typeof testVar === 'string' || testVar instanceof String;
}
```
- example usage
```shell
...
  httpAdapter = 'https';
}

if (!geocoderAdapter) {
  geocoderAdapter = 'google';
}

if (Helper.isString(httpAdapter)) {
  httpAdapter = this._getHttpAdapter(httpAdapter, extra);
}

if (Helper.isString(geocoderAdapter)) {
  geocoderAdapter = this._getGeocoder(geocoderAdapter, httpAdapter, extra);
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
