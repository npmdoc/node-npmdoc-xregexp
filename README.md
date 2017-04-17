# api documentation for  [xregexp (v3.2.0)](http://xregexp.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-xregexp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xregexp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xregexp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xregexp)
#### Extended regular expressions

[![NPM](https://nodei.co/npm/xregexp.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/xregexp)

- [https://npmdoc.github.io/node-npmdoc-xregexp/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-xregexp/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xregexp/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xregexp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xregexp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xregexp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Steven Levithan"
    },
    "bugs": {
        "url": "https://github.com/slevithan/xregexp/issues"
    },
    "dependencies": {},
    "description": "Extended regular expressions",
    "devDependencies": {
        "browserify": "^12.0.1",
        "jasmine": "^2.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "cb3601987bfe2695b584000c18f1c4a8c322878e",
        "tarball": "https://registry.npmjs.org/xregexp/-/xregexp-3.2.0.tgz"
    },
    "files": [
        "src",
        "xregexp-all.js",
        "LICENSE"
    ],
    "gitHead": "ddf24c536821faf2493625ed6bdc3cb5ce2c6fdd",
    "homepage": "http://xregexp.com/",
    "keywords": [
        "regex",
        "regexp",
        "regular expression",
        "unicode"
    ],
    "license": "MIT",
    "main": "xregexp-all.js",
    "maintainers": [
        {
            "name": "slevithan"
        }
    ],
    "name": "xregexp",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/slevithan/xregexp.git"
    },
    "scripts": {
        "build": "browserify src/index.js --standalone XRegExp > xregexp-all.js",
        "pretest": "npm run build",
        "test": "jasmine JASMINE_CONFIG_PATH=tests/jasmine.json"
    },
    "version": "3.2.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
