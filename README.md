# api documentation for  [js-base64 (v2.1.9)](https://github.com/dankogai/js-base64#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-js-base64.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-js-base64) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-js-base64.svg)](https://travis-ci.org/npmdoc/node-npmdoc-js-base64)
#### Yet another Base64 transcoder in pure-JS

[![NPM](https://nodei.co/npm/js-base64.png?downloads=true)](https://www.npmjs.com/package/js-base64)

[![apidoc](https://npmdoc.github.io/node-npmdoc-js-base64/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-js-base64_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-js-base64/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-js-base64/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-js-base64/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dan Kogai"
    },
    "bugs": {
        "url": "https://github.com/dankogai/js-base64/issues"
    },
    "dependencies": {},
    "description": "Yet another Base64 transcoder in pure-JS",
    "devDependencies": {
        "mocha": "*"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "f0e80ae039a4bd654b5f281fc93f04a914a7fcce",
        "tarball": "https://registry.npmjs.org/js-base64/-/js-base64-2.1.9.tgz"
    },
    "gitHead": "8bfa436f733bec60c95c720e1d720c28b43ae0b2",
    "homepage": "https://github.com/dankogai/js-base64#readme",
    "keywords": [
        "base64"
    ],
    "license": "BSD",
    "main": "base64.js",
    "maintainers": [
        {
            "name": "dankogai",
            "email": "dankogai+github@gmail.com"
        }
    ],
    "name": "js-base64",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/dankogai/js-base64.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "2.1.9"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module js-base64](#apidoc.module.js-base64)
1.  object <span class="apidocSignatureSpan">js-base64.</span>Base64

#### [module js-base64.Base64](#apidoc.module.js-base64.Base64)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>atob (a)](#apidoc.element.js-base64.Base64.atob)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>btoa (b)](#apidoc.element.js-base64.Base64.btoa)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>btou (b)](#apidoc.element.js-base64.Base64.btou)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>decode (a)](#apidoc.element.js-base64.Base64.decode)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>encode (u, urisafe)](#apidoc.element.js-base64.Base64.encode)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>encodeURI (u)](#apidoc.element.js-base64.Base64.encodeURI)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>extendString ()](#apidoc.element.js-base64.Base64.extendString)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>fromBase64 (a)](#apidoc.element.js-base64.Base64.fromBase64)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>noConflict ()](#apidoc.element.js-base64.Base64.noConflict)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>toBase64 (u, urisafe)](#apidoc.element.js-base64.Base64.toBase64)
1.  [function <span class="apidocSignatureSpan">js-base64.Base64.</span>utob (u)](#apidoc.element.js-base64.Base64.utob)
1.  string <span class="apidocSignatureSpan">js-base64.Base64.</span>VERSION



# <a name="apidoc.module.js-base64"></a>[module js-base64](#apidoc.module.js-base64)



# <a name="apidoc.module.js-base64.Base64"></a>[module js-base64.Base64](#apidoc.module.js-base64.Base64)

#### <a name="apidoc.element.js-base64.Base64.atob"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>atob (a)](#apidoc.element.js-base64.Base64.atob)
- description and source-code
```javascript
atob = function (a){
    return a.replace(/[\s\S]{1,4}/g, cb_decode);
}
```
- example usage
```shell
...
        fromCharCode((n >>>  8) & 0xff),
        fromCharCode( n         & 0xff)
    ];
    chars.length -= [0, 0, 2, 1][padlen];
    return chars.join('');
};
var atob = global.atob ? function(a) {
    return global.atob(a);
} : function(a){
    return a.replace(/[\s\S]{1,4}/g, cb_decode);
};
var _decode = buffer ? function(a) {
    return (a.constructor === buffer.constructor
            ? a : new buffer(a, 'base64')).toString();
}
...
```

#### <a name="apidoc.element.js-base64.Base64.btoa"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>btoa (b)](#apidoc.element.js-base64.Base64.btoa)
- description and source-code
```javascript
btoa = function (b) {
    return b.replace(/[\s\S]{1,3}/g, cb_encode);
}
```
- example usage
```shell
...
        b64chars.charAt((ord >>> 12) & 63),
        padlen >= 2 ? '=' : b64chars.charAt((ord >>> 6) & 63),
        padlen >= 1 ? '=' : b64chars.charAt(ord & 63)
    ];
    return chars.join('');
};
var btoa = global.btoa ? function(b) {
    return global.btoa(b);
} : function(b) {
    return b.replace(/[\s\S]{1,3}/g, cb_encode);
};
var _encode = buffer ? function (u) {
    return (u.constructor === buffer.constructor ? u : new buffer(u))
    .toString('base64')
}
...
```

#### <a name="apidoc.element.js-base64.Base64.btou"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>btou (b)](#apidoc.element.js-base64.Base64.btou)
- description and source-code
```javascript
btou = function (b) {
    return b.replace(re_btou, cb_btou);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-base64.Base64.decode"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>decode (a)](#apidoc.element.js-base64.Base64.decode)
- description and source-code
```javascript
decode = function (a){
    return _decode(
        String(a).replace(/[-_]/g, function(m0) { return m0 == '-' ? '+' : '/' })
            .replace(/[^A-Za-z0-9\+\/]/g, '')
    );
}
```
- example usage
```shell
...
## SYNOPSIS

''''javascript
Base64.encode('dankogai');  // ZGFua29nYWk=
Base64.encode('小飼弾');    // 5bCP6aO85by+
Base64.encodeURI('小飼弾'); // 5bCP6aO85by-

Base64.decode('ZGFua29nYWk=');  // dankogai
Base64.decode('5bCP6aO85by+');  // 小飼弾
// note .decodeURI() is unnecessary since it accepts both flavors
Base64.decode('5bCP6aO85by-');  // 小飼弾
''''

### String Extension for ES5
...
```

#### <a name="apidoc.element.js-base64.Base64.encode"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>encode (u, urisafe)](#apidoc.element.js-base64.Base64.encode)
- description and source-code
```javascript
encode = function (u, urisafe) {
    return !urisafe
        ? _encode(String(u))
        : _encode(String(u)).replace(/[+\/]/g, function(m0) {
            return m0 == '+' ? '-' : '_';
        }).replace(/=/g, '');
}
```
- example usage
```shell
...
var Base64 = require('./base64.js').Base64;
''''


## SYNOPSIS

''''javascript
Base64.encode('dankogai');  // ZGFua29nYWk=
Base64.encode('小飼弾');    // 5bCP6aO85by+
Base64.encodeURI('小飼弾'); // 5bCP6aO85by-

Base64.decode('ZGFua29nYWk=');  // dankogai
Base64.decode('5bCP6aO85by+');  // 小飼弾
// note .decodeURI() is unnecessary since it accepts both flavors
Base64.decode('5bCP6aO85by-');  // 小飼弾
...
```

#### <a name="apidoc.element.js-base64.Base64.encodeURI"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>encodeURI (u)](#apidoc.element.js-base64.Base64.encodeURI)
- description and source-code
```javascript
encodeURI = function (u) { return encode(u, true) }
```
- example usage
```shell
...


## SYNOPSIS

''''javascript
Base64.encode('dankogai');  // ZGFua29nYWk=
Base64.encode('小飼弾');    // 5bCP6aO85by+
Base64.encodeURI('小飼弾'); // 5bCP6aO85by-

Base64.decode('ZGFua29nYWk=');  // dankogai
Base64.decode('5bCP6aO85by+');  // 小飼弾
// note .decodeURI() is unnecessary since it accepts both flavors
Base64.decode('5bCP6aO85by-');  // 小飼弾
''''
...
```

#### <a name="apidoc.element.js-base64.Base64.extendString"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>extendString ()](#apidoc.element.js-base64.Base64.extendString)
- description and source-code
```javascript
extendString = function () {
    Object.defineProperty(
        String.prototype, 'fromBase64', noEnum(function () {
            return decode(this)
        }));
    Object.defineProperty(
        String.prototype, 'toBase64', noEnum(function (urisafe) {
            return encode(this, urisafe)
        }));
    Object.defineProperty(
        String.prototype, 'toBase64URI', noEnum(function () {
            return encode(this, true)
        }));
}
```
- example usage
```shell
...
''''

### String Extension for ES5

''''javascript
if (Base64.extendString) {
// you have to explicitly extend String.prototype
Base64.extendString();
// once extended, you can do the following
'dankogai'.toBase64();       // ZGFua29nYWk=
'小飼弾'.toBase64();         // 5bCP6aO85by+
'小飼弾'.toBase64(true);     // 5bCP6aO85by-
'小飼弾'.toBase64URI();      // 5bCP6aO85by-
'ZGFua29nYWk='.fromBase64(); // dankogai
'5bCP6aO85by+'.fromBase64(); // 小飼弾
...
```

#### <a name="apidoc.element.js-base64.Base64.fromBase64"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>fromBase64 (a)](#apidoc.element.js-base64.Base64.fromBase64)
- description and source-code
```javascript
fromBase64 = function (a){
    return _decode(
        String(a).replace(/[-_]/g, function(m0) { return m0 == '-' ? '+' : '/' })
            .replace(/[^A-Za-z0-9\+\/]/g, '')
    );
}
```
- example usage
```shell
...
    // you have to explicitly extend String.prototype
    Base64.extendString();
    // once extended, you can do the following
    'dankogai'.toBase64();       // ZGFua29nYWk=
    '小飼弾'.toBase64();         // 5bCP6aO85by+
    '小飼弾'.toBase64(true);     // 5bCP6aO85by-
    '小飼弾'.toBase64URI();      // 5bCP6aO85by-
    'ZGFua29nYWk='.fromBase64(); // dankogai
    '5bCP6aO85by+'.fromBase64(); // 小飼弾
    '5bCP6aO85by-'.fromBase64(); // 小飼弾
}
''''

## SEE ALSO
...
```

#### <a name="apidoc.element.js-base64.Base64.noConflict"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>noConflict ()](#apidoc.element.js-base64.Base64.noConflict)
- description and source-code
```javascript
noConflict = function () {
    var Base64 = global.Base64;
    global.Base64 = _Base64;
    return Base64;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-base64.Base64.toBase64"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>toBase64 (u, urisafe)](#apidoc.element.js-base64.Base64.toBase64)
- description and source-code
```javascript
toBase64 = function (u, urisafe) {
    return !urisafe
        ? _encode(String(u))
        : _encode(String(u)).replace(/[+\/]/g, function(m0) {
            return m0 == '+' ? '-' : '_';
        }).replace(/=/g, '');
}
```
- example usage
```shell
...
### String Extension for ES5

''''javascript
if (Base64.extendString) {
    // you have to explicitly extend String.prototype
    Base64.extendString();
    // once extended, you can do the following
    'dankogai'.toBase64();       // ZGFua29nYWk=
    '小飼弾'.toBase64();         // 5bCP6aO85by+
    '小飼弾'.toBase64(true);     // 5bCP6aO85by-
    '小飼弾'.toBase64URI();      // 5bCP6aO85by-
    'ZGFua29nYWk='.fromBase64(); // dankogai
    '5bCP6aO85by+'.fromBase64(); // 小飼弾
    '5bCP6aO85by-'.fromBase64(); // 小飼弾
}
...
```

#### <a name="apidoc.element.js-base64.Base64.utob"></a>[function <span class="apidocSignatureSpan">js-base64.Base64.</span>utob (u)](#apidoc.element.js-base64.Base64.utob)
- description and source-code
```javascript
utob = function (u) {
    return u.replace(re_utob, cb_utob);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
