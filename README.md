# api documentation for  [xregexp (v3.1.1)](http://xregexp.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-xregexp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-xregexp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-xregexp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-xregexp)
#### Extended regular expressions

[![NPM](https://nodei.co/npm/xregexp.png?downloads=true)](https://www.npmjs.com/package/xregexp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-xregexp/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-xregexp_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-xregexp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-xregexp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-xregexp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Steven Levithan",
        "email": "steves_list@hotmail.com"
    },
    "bugs": {
        "url": "https://github.com/slevithan/xregexp/issues"
    },
    "dependencies": {},
    "description": "Extended regular expressions",
    "devDependencies": {
        "browserify": "^12.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "8ee18d75ef5c7cb3f9967f8d29414a6ca5b1a184",
        "tarball": "https://registry.npmjs.org/xregexp/-/xregexp-3.1.1.tgz"
    },
    "files": [
        "src"
    ],
    "gitHead": "37413619ea9f03638bfa92e038e4b4c15645d446",
    "homepage": "http://xregexp.com/",
    "keywords": [
        "regex",
        "regexp",
        "regular expression",
        "unicode"
    ],
    "license": "MIT",
    "main": "./src/index.js",
    "maintainers": [
        {
            "name": "slevithan",
            "email": "steves_list@hotmail.com"
        }
    ],
    "name": "xregexp",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/slevithan/xregexp.git"
    },
    "scripts": {
        "build": "browserify src/index.js --standalone XRegExp > xregexp-all.js"
    },
    "version": "3.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module xregexp](#apidoc.module.xregexp)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>_dec (hex)](#apidoc.element.xregexp._dec)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>_hasNativeFlag (flag)](#apidoc.element.xregexp._hasNativeFlag)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>_hex (dec)](#apidoc.element.xregexp._hex)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>_pad4 (str)](#apidoc.element.xregexp._pad4)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>addToken (regex, handler, options)](#apidoc.element.xregexp.addToken)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>addUnicodeData (data)](#apidoc.element.xregexp.addUnicodeData)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>build (pattern, subs, flags)](#apidoc.element.xregexp.build)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>cache (pattern, flags)](#apidoc.element.xregexp.cache)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>escape (str)](#apidoc.element.xregexp.escape)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>exec (str, regex, pos, sticky)](#apidoc.element.xregexp.exec)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>forEach (str, regex, callback)](#apidoc.element.xregexp.forEach)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>globalize (regex)](#apidoc.element.xregexp.globalize)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>install (options)](#apidoc.element.xregexp.install)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>isInstalled (feature)](#apidoc.element.xregexp.isInstalled)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>isRegExp (value)](#apidoc.element.xregexp.isRegExp)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>match (str, regex, scope)](#apidoc.element.xregexp.match)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>matchChain (str, chain)](#apidoc.element.xregexp.matchChain)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>matchRecursive (str, left, right, flags, options)](#apidoc.element.xregexp.matchRecursive)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>replace (str, search, replacement, scope)](#apidoc.element.xregexp.replace)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>replaceEach (str, replacements)](#apidoc.element.xregexp.replaceEach)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>split (str, separator, limit)](#apidoc.element.xregexp.split)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>test (str, regex, pos, sticky)](#apidoc.element.xregexp.test)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>uninstall (options)](#apidoc.element.xregexp.uninstall)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>union (patterns, flags)](#apidoc.element.xregexp.union)
1.  string <span class="apidocSignatureSpan">xregexp.</span>version

#### [module xregexp.cache](#apidoc.module.xregexp.cache)
1.  [function <span class="apidocSignatureSpan">xregexp.</span>cache (pattern, flags)](#apidoc.element.xregexp.cache.cache)
1.  [function <span class="apidocSignatureSpan">xregexp.cache.</span>flush (cacheName)](#apidoc.element.xregexp.cache.flush)



# <a name="apidoc.module.xregexp"></a>[module xregexp](#apidoc.module.xregexp)

#### <a name="apidoc.element.xregexp._dec"></a>[function <span class="apidocSignatureSpan">xregexp.</span>_dec (hex)](#apidoc.element.xregexp._dec)
- description and source-code
```javascript
function dec(hex) {
    return parseInt(hex, 16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp._hasNativeFlag"></a>[function <span class="apidocSignatureSpan">xregexp.</span>_hasNativeFlag (flag)](#apidoc.element.xregexp._hasNativeFlag)
- description and source-code
```javascript
function hasNativeFlag(flag) {
    // Can't check based on the presense of properties/getters since browsers might support such
    // properties even when they don't support the corresponding flag in regex construction (tested
    // in Chrome 48, where ''unicode' in /x/' is true but trying to construct a regex with flag 'u'
    // throws an error)
    var isSupported = true;
    try {
        // Can't use regex literals for testing even in a 'try' because regex literals with
        // unsupported flags cause a compilation error in IE
        new RegExp('', flag);
    } catch (exception) {
        isSupported = false;
    }
    if (isSupported && flag === 'y') {
        // Work around Safari 9.1.1 bug
        return new RegExp('aa|.', 'y').test('b');
    }
    return isSupported;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp._hex"></a>[function <span class="apidocSignatureSpan">xregexp.</span>_hex (dec)](#apidoc.element.xregexp._hex)
- description and source-code
```javascript
function hex(dec) {
    return parseInt(dec, 10).toString(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp._pad4"></a>[function <span class="apidocSignatureSpan">xregexp.</span>_pad4 (str)](#apidoc.element.xregexp._pad4)
- description and source-code
```javascript
function pad4(str) {
    while (str.length < 4) {
        str = '0' + str;
    }
    return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.addToken"></a>[function <span class="apidocSignatureSpan">xregexp.</span>addToken (regex, handler, options)](#apidoc.element.xregexp.addToken)
- description and source-code
```javascript
addToken = function (regex, handler, options) {
    options = options || {};
    var optionalFlags = options.optionalFlags, i;

    if (options.flag) {
        registerFlag(options.flag);
    }

    if (optionalFlags) {
        optionalFlags = nativ.split.call(optionalFlags, '');
        for (i = 0; i < optionalFlags.length; ++i) {
            registerFlag(optionalFlags[i]);
        }
    }

    // Add to the private list of syntax tokens
    tokens.push({
        regex: copyRegex(regex, {
            addG: true,
            addY: hasNativeY,
            isInternalOnly: true
        }),
        handler: handler,
        scope: options.scope || defaultScope,
        flag: options.flag,
        reparse: options.reparse,
        leadChar: options.leadChar
    });

    // Reset the pattern cache used by the 'XRegExp' constructor, since the same pattern and flags
    // might now produce different results
    XRegExp.cache.flush('patterns');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.addUnicodeData"></a>[function <span class="apidocSignatureSpan">xregexp.</span>addUnicodeData (data)](#apidoc.element.xregexp.addUnicodeData)
- description and source-code
```javascript
addUnicodeData = function (data) {
    var ERR_NO_NAME = 'Unicode token requires name',
        ERR_NO_DATA = 'Unicode token has no character data ',
        item,
        i;

    for (i = 0; i < data.length; ++i) {
        item = data[i];
        if (!item.name) {
            throw new Error(ERR_NO_NAME);
        }
        if (!(item.inverseOf || item.bmp || item.astral)) {
            throw new Error(ERR_NO_DATA + item.name);
        }
        unicode[normalize(item.name)] = item;
        if (item.alias) {
            unicode[normalize(item.alias)] = item;
        }
    }

    // Reset the pattern cache used by the 'XRegExp' constructor, since the same pattern and
    // flags might now produce different results
    XRegExp.cache.flush('patterns');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.build"></a>[function <span class="apidocSignatureSpan">xregexp.</span>build (pattern, subs, flags)](#apidoc.element.xregexp.build)
- description and source-code
```javascript
build = function (pattern, subs, flags) {
    var inlineFlags = /^\(\?([\w$]+)\)/.exec(pattern),
        data = {},
        numCaps = 0, // 'Caps' is short for captures
        numPriorCaps,
        numOuterCaps = 0,
        outerCapsMap = [0],
        outerCapNames,
        sub,
        p;

    // Add flags within a leading mode modifier to the overall pattern's flags
    if (inlineFlags) {
        flags = flags || '';
        inlineFlags[1].replace(/./g, function(flag) {
            // Don't add duplicates
            flags += (flags.indexOf(flag) > -1 ? '' : flag);
        });
    }

    for (p in subs) {
        if (subs.hasOwnProperty(p)) {
            // Passing to XRegExp enables extended syntax and ensures independent validity,
            // lest an unescaped '(', ')', '[', or trailing '\' breaks the '(?:)' wrapper. For
            // subpatterns provided as native regexes, it dies on octals and adds the property
            // used to hold extended regex instance data, for simplicity
            sub = asXRegExp(subs[p]);
            data[p] = {
                // Deanchoring allows embedding independently useful anchored regexes. If you
                // really need to keep your anchors, double them (i.e., '^^...$$')
                pattern: deanchor(sub.source),
                names: sub[REGEX_DATA].captureNames || []
            };
        }
    }

    // Passing to XRegExp dies on octals and ensures the outer pattern is independently valid;
    // helps keep this simple. Named captures will be put back
    pattern = asXRegExp(pattern);
    outerCapNames = pattern[REGEX_DATA].captureNames || [];
    pattern = pattern.source.replace(parts, function($0, $1, $2, $3, $4) {
        var subName = $1 || $2,
            capName,
            intro,
            localCapIndex;
        // Named subpattern
        if (subName) {
            if (!data.hasOwnProperty(subName)) {
                throw new ReferenceError('Undefined property ' + $0);
            }
            // Named subpattern was wrapped in a capturing group
            if ($1) {
                capName = outerCapNames[numOuterCaps];
                outerCapsMap[++numOuterCaps] = ++numCaps;
                // If it's a named group, preserve the name. Otherwise, use the subpattern name
                // as the capture name
                intro = '(?<' + (capName || subName) + '>';
            } else {
                intro = '(?:';
            }
            numPriorCaps = numCaps;
            return intro + data[subName].pattern.replace(subParts, function(match, paren, backref) {
                // Capturing group
                if (paren) {
                    capName = data[subName].names[numCaps - numPriorCaps];
                    ++numCaps;
                    // If the current capture has a name, preserve the name
                    if (capName) {
                        return '(?<' + capName + '>';
                    }
                // Backreference
                } else if (backref) {
                    localCapIndex = +backref - 1;
                    // Rewrite the backreference
                    return data[subName].names[localCapIndex] ?
                        // Need to preserve the backreference name in case using flag 'n'
                        '\\k<' + data[subName].names[localCapIndex] + '>' :
                        '\\' + (+backref + numPriorCaps);
                }
                return match;
            }) + ')';
        }
        // Capturing group
        if ($3) {
            capName = outerCapNames[numOuterCaps];
            outerCapsMap[++numOuterCaps] = ++numCaps;
            // If the current capture has a name, preserve the name
            if (capName) {
                return '(?<' + capName + '>';
            }
        // Backreference
        } else if ($4) {
            localCapIndex = +$4 - 1;
            // Rewrite the backreference
            return outerCapNames[localCapIndex] ?
                // Need to preserve the backreference name in case using flag 'n'
                '\\k<' + outerCapNames[localCapInde ...
```
- example usage
```shell
...
XRegExp uses Unicode 8.0.0.

### XRegExp.build

Build regular expressions using named subpatterns, for readability and pattern reuse:

'''js
var time = XRegExp.build('(?x)^ {{hours}} ({{minutes}}) $', {
    hours: XRegExp.build('{{h12}} : | {{h24}}', {
        h12: /1[0-2]|0?[1-9]/,
        h24: /2[0-3]|[01][0-9]/
    }),
    minutes: /^[0-5][0-9]$/
});
...
```

#### <a name="apidoc.element.xregexp.cache"></a>[function <span class="apidocSignatureSpan">xregexp.</span>cache (pattern, flags)](#apidoc.element.xregexp.cache)
- description and source-code
```javascript
cache = function (pattern, flags) {
    if (!regexCache[pattern]) {
        regexCache[pattern] = {};
    }
    return regexCache[pattern][flags] || (
        regexCache[pattern][flags] = XRegExp(pattern, flags)
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.escape"></a>[function <span class="apidocSignatureSpan">xregexp.</span>escape (str)](#apidoc.element.xregexp.escape)
- description and source-code
```javascript
escape = function (str) {
    return nativ.replace.call(toObject(str), /[-[\]{}()*+?.,\\^$|#\s]/g, '\\$&');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.exec"></a>[function <span class="apidocSignatureSpan">xregexp.</span>exec (str, regex, pos, sticky)](#apidoc.element.xregexp.exec)
- description and source-code
```javascript
exec = function (str, regex, pos, sticky) {
    var cacheKey = 'g',
        addY = false,
        match,
        r2;

    addY = hasNativeY && !!(sticky || (regex.sticky && sticky !== false));
    if (addY) {
        cacheKey += 'y';
    }

    regex[REGEX_DATA] = regex[REGEX_DATA] || {};

    // Shares cached copies with 'XRegExp.match'/'replace'
    r2 = regex[REGEX_DATA][cacheKey] || (
        regex[REGEX_DATA][cacheKey] = copyRegex(regex, {
            addG: true,
            addY: addY,
            removeY: sticky === false,
            isInternalOnly: true
        })
    );

    r2.lastIndex = pos = pos || 0;

    // Fixed 'exec' required for 'lastIndex' fix, named backreferences, etc.
    match = fixed.exec.call(r2, str);

    if (sticky && match && match.index !== pos) {
        match = null;
    }

    if (regex.global) {
        regex.lastIndex = match ? r2.lastIndex : 0;
    }

    return match;
}
```
- example usage
```shell
...
'''js
// Using named capture and flag x (free-spacing and line comments)
var date = XRegExp('(?<year>  [0-9]{4} ) -?  # year  \n\
                (?<month> [0-9]{2} ) -?  # month \n\
                (?<day>   [0-9]{2} )     # day   ', 'x');

// XRegExp.exec gives you named backreferences on the match result
var match = XRegExp.exec('2015-02-22', date);
match.year; // -> '2015'

// It also includes optional pos and sticky arguments
var pos = 3;
var result = [];
while (match = XRegExp.exec('<1><2><3><4>5<6>', /<(\d+)>/, pos, 'sticky')) {
result.push(match[1]);
...
```

#### <a name="apidoc.element.xregexp.forEach"></a>[function <span class="apidocSignatureSpan">xregexp.</span>forEach (str, regex, callback)](#apidoc.element.xregexp.forEach)
- description and source-code
```javascript
forEach = function (str, regex, callback) {
    var pos = 0,
        i = -1,
        match;

    while ((match = XRegExp.exec(str, regex, pos))) {
        // Because 'regex' is provided to 'callback', the function could use the deprecated/
        // nonstandard 'RegExp.prototype.compile' to mutate the regex. However, since 'XRegExp.exec'
        // doesn't use 'lastIndex' to set the search position, this can't lead to an infinite loop,
        // at least. Actually, because of the way 'XRegExp.exec' caches globalized versions of
        // regexes, mutating the regex will not have any effect on the iteration or matched strings,
        // which is a nice side effect that brings extra safety.
        callback(match, ++i, str, regex);

        pos = match.index + (match[0].length || 1);
    }
}
```
- example usage
```shell
...
// The only caveat is that named captures must be referenced using numbered
// backreferences if used with native methods
'2015-02-22'.replace(date, '$2/$3/$1');
// -> '02/22/2015'

// Extract every other digit from a string using XRegExp.forEach
var evens = [];
XRegExp.forEach('1a2345', /\d/, function(match, i) {
if (i % 2) evens.push(+match[0]);
});
// evens -> [2, 4]

// Get numbers within <b> tags using XRegExp.matchChain
XRegExp.matchChain('1 <b>2</b> 3 <b>4 a 56</b>', [
XRegExp('(?is)<b>.*?</b>'),
...
```

#### <a name="apidoc.element.xregexp.globalize"></a>[function <span class="apidocSignatureSpan">xregexp.</span>globalize (regex)](#apidoc.element.xregexp.globalize)
- description and source-code
```javascript
globalize = function (regex) {
    return copyRegex(regex, {addG: true});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.install"></a>[function <span class="apidocSignatureSpan">xregexp.</span>install (options)](#apidoc.element.xregexp.install)
- description and source-code
```javascript
install = function (options) {
    options = prepareOptions(options);

    if (!features.astral && options.astral) {
        setAstral(true);
    }

    if (!features.natives && options.natives) {
        setNatives(true);
    }
}
```
- example usage
```shell
...
unicodeWord.test('العربية'); // -> true

// Test some Unicode scripts
XRegExp('^\\p{Hiragana}+$').test('ひらがな'); // -> true
XRegExp('^[\\p{Latin}\\p{Common}]+$').test('Über Café.'); // -> true
'''

By default, '\p{…}' and '\P{…}' support the Basic Multilingual Plane (i.e. code points up to 'U+FFFF'). You can opt-in to full 21
-bit Unicode support (with code points up to 'U+10FFFF') on a per-regex basis by using flag 'A'. In XRegExp, this is called *astral
 mode*. You can automatically add flag 'A' for all new regexes by running 'XRegExp.install('astral')'. When in astral mode, '\p{…}' and '\P{…}' always match a full code point rather than a code unit, using surrogate pairs for code points above 'U+FFFF'.

'''js
// Using flag A to match astral code points
XRegExp('^\\pS$').test('💩'); // -> false
XRegExp('^\\pS$', 'A').test('💩'); // -> true
XRegExp('(?A)^\\pS$').test('💩'); // -> true
// Using surrogate pair U+D83D U+DCA9 to represent U+1F4A9 (pile of poo)
...
```

#### <a name="apidoc.element.xregexp.isInstalled"></a>[function <span class="apidocSignatureSpan">xregexp.</span>isInstalled (feature)](#apidoc.element.xregexp.isInstalled)
- description and source-code
```javascript
isInstalled = function (feature) {
    return !!(features[feature]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.isRegExp"></a>[function <span class="apidocSignatureSpan">xregexp.</span>isRegExp (value)](#apidoc.element.xregexp.isRegExp)
- description and source-code
```javascript
isRegExp = function (value) {
    return toString.call(value) === '[object RegExp]';
    //return isType(value, 'RegExp');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.match"></a>[function <span class="apidocSignatureSpan">xregexp.</span>match (str, regex, scope)](#apidoc.element.xregexp.match)
- description and source-code
```javascript
match = function (str, regex, scope) {
    var global = (regex.global && scope !== 'one') || scope === 'all',
        cacheKey = ((global ? 'g' : '') + (regex.sticky ? 'y' : '')) || 'noGY',
        result,
        r2;

    regex[REGEX_DATA] = regex[REGEX_DATA] || {};

    // Shares cached copies with 'XRegExp.exec'/'replace'
    r2 = regex[REGEX_DATA][cacheKey] || (
        regex[REGEX_DATA][cacheKey] = copyRegex(regex, {
            addG: !!global,
            removeG: scope === 'one',
            isInternalOnly: true
        })
    );

    result = nativ.match.call(toObject(str), r2);

    if (regex.global) {
        regex.lastIndex = (
            (scope === 'one' && result) ?
                // Can't use 'r2.lastIndex' since 'r2' is nonglobal in this case
                (result.index + result[0].length) : 0
        );
    }

    return global ? (result || []) : (result && result[0]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.matchChain"></a>[function <span class="apidocSignatureSpan">xregexp.</span>matchChain (str, chain)](#apidoc.element.xregexp.matchChain)
- description and source-code
```javascript
matchChain = function (str, chain) {
    return (function recurseChain(values, level) {
        var item = chain[level].regex ? chain[level] : {regex: chain[level]};
        var matches = [];

        function addMatch(match) {
            if (item.backref) {
                // Safari 4.0.5 (but not 5.0.5+) inappropriately uses sparse arrays to hold the
                // 'undefined's for backreferences to nonparticipating capturing groups. In such
                // cases, a 'hasOwnProperty' or 'in' check on its own would inappropriately throw
                // the exception, so also check if the backreference is a number that is within the
                // bounds of the array.
                if (!(match.hasOwnProperty(item.backref) || +item.backref < match.length)) {
                    throw new ReferenceError('Backreference to undefined group: ' + item.backref);
                }

                matches.push(match[item.backref] || '');
            } else {
                matches.push(match[0]);
            }
        }

        for (var i = 0; i < values.length; ++i) {
            XRegExp.forEach(values[i], item.regex, addMatch);
        }

        return ((level === chain.length - 1) || !matches.length) ?
            matches :
            recurseChain(matches, level + 1);
    }([str], 0));
}
```
- example usage
```shell
...
var evens = [];
XRegExp.forEach('1a2345', /\d/, function(match, i) {
    if (i % 2) evens.push(+match[0]);
});
// evens -> [2, 4]

// Get numbers within <b> tags using XRegExp.matchChain
XRegExp.matchChain('1 <b>2</b> 3 <b>4 a 56</b>', [
    XRegExp('(?is)<b>.*?</b>'),
    /\d+/
]);
// -> ['2', '4', '56']

// You can also pass forward and return specific backreferences
var html = '<a href="http://xregexp.com/">XRegExp</a>' +
...
```

#### <a name="apidoc.element.xregexp.matchRecursive"></a>[function <span class="apidocSignatureSpan">xregexp.</span>matchRecursive (str, left, right, flags, options)](#apidoc.element.xregexp.matchRecursive)
- description and source-code
```javascript
matchRecursive = function (str, left, right, flags, options) {
    flags = flags || '';
    options = options || {};
    var global = flags.indexOf('g') > -1,
        sticky = flags.indexOf('y') > -1,
        // Flag 'y' is controlled internally
        basicFlags = flags.replace(/y/g, ''),
        escapeChar = options.escapeChar,
        vN = options.valueNames,
        output = [],
        openTokens = 0,
        delimStart = 0,
        delimEnd = 0,
        lastOuterEnd = 0,
        outerStart,
        innerStart,
        leftMatch,
        rightMatch,
        esc;
    left = XRegExp(left, basicFlags);
    right = XRegExp(right, basicFlags);

    if (escapeChar) {
        if (escapeChar.length > 1) {
            throw new Error('Cannot use more than one escape character');
        }
        escapeChar = XRegExp.escape(escapeChar);
        // Using 'XRegExp.union' safely rewrites backreferences in 'left' and 'right'
        esc = new RegExp(
            '(?:' + escapeChar + '[\\S\\s]|(?:(?!' +
                XRegExp.union([left, right]).source +
                ')[^' + escapeChar + '])+)+',
            // Flags 'gy' not needed here
            flags.replace(/[^imu]+/g, '')
        );
    }

    while (true) {
        // If using an escape character, advance to the delimiter's next starting position,
        // skipping any escaped characters in between
        if (escapeChar) {
            delimEnd += (XRegExp.exec(str, esc, delimEnd, 'sticky') || [''])[0].length;
        }
        leftMatch = XRegExp.exec(str, left, delimEnd);
        rightMatch = XRegExp.exec(str, right, delimEnd);
        // Keep the leftmost match only
        if (leftMatch && rightMatch) {
            if (leftMatch.index <= rightMatch.index) {
                rightMatch = null;
            } else {
                leftMatch = null;
            }
        }
        // Paths (LM: leftMatch, RM: rightMatch, OT: openTokens):
        // LM | RM | OT | Result
        // 1  | 0  | 1  | loop
        // 1  | 0  | 0  | loop
        // 0  | 1  | 1  | loop
        // 0  | 1  | 0  | throw
        // 0  | 0  | 1  | throw
        // 0  | 0  | 0  | break
        // The paths above don't include the sticky mode special case. The loop ends after the
        // first completed match if not 'global'.
        if (leftMatch || rightMatch) {
            delimStart = (leftMatch || rightMatch).index;
            delimEnd = delimStart + (leftMatch || rightMatch)[0].length;
        } else if (!openTokens) {
            break;
        }
        if (sticky && !openTokens && delimStart > lastOuterEnd) {
            break;
        }
        if (leftMatch) {
            if (!openTokens) {
                outerStart = delimStart;
                innerStart = delimEnd;
            }
            ++openTokens;
        } else if (rightMatch && openTokens) {
            if (!--openTokens) {
                if (vN) {
                    if (vN[0] && outerStart > lastOuterEnd) {
                        output.push(row(vN[0], str.slice(lastOuterEnd, outerStart), lastOuterEnd, outerStart));
                    }
                    if (vN[1]) {
                        output.push(row(vN[1], str.slice(outerStart, innerStart), outerStart, innerStart));
                    }
                    if (vN[2]) {
                        output.push(row(vN[2], str.slice(innerStart, delimStart), innerStart, delimStart));
                    }
                    if (vN[3]) {
                        output.push(row(vN[3], str.slice(delimStart, delimEnd), delimStart, delimEnd));
                    }
                } else {
                    output.push(str.slice(innerStart, delimStart));
                }
                lastOuterEnd = delimEnd;
                if (!global) {
                    break;
                }
            }
        } else {
            throw new Error('Unbalanced delimiter found in string');
        }
        // If the delimiter matched an empty string, avoid an infinite loop
        if (delimStart === delimEnd) {
            ++delimEnd;
        }
    }

    if (global && !sticky && vN & ...
```
- example usage
```shell
...

### XRegExp.matchRecursive

Match recursive constructs using XRegExp pattern strings as left and right delimiters:

'''js
var str = '(t((e))s)t()(ing)';
XRegExp.matchRecursive(str, '\\(', '\\)', 'g');
// -> ['t((e))s', '', 'ing']

// Extended information mode with valueNames
str = 'Here is <div> <div>an</div></div> example';
XRegExp.matchRecursive(str, '<div\\s*>', '</div>', 'gi', {
    valueNames: ['between', 'left', 'match', 'right']
});
...
```

#### <a name="apidoc.element.xregexp.replace"></a>[function <span class="apidocSignatureSpan">xregexp.</span>replace (str, search, replacement, scope)](#apidoc.element.xregexp.replace)
- description and source-code
```javascript
replace = function (str, search, replacement, scope) {
    var isRegex = XRegExp.isRegExp(search),
        global = (search.global && scope !== 'one') || scope === 'all',
        cacheKey = ((global ? 'g' : '') + (search.sticky ? 'y' : '')) || 'noGY',
        s2 = search,
        result;

    if (isRegex) {
        search[REGEX_DATA] = search[REGEX_DATA] || {};

        // Shares cached copies with 'XRegExp.exec'/'match'. Since a copy is used, 'search''s
        // 'lastIndex' isn't updated *during* replacement iterations
        s2 = search[REGEX_DATA][cacheKey] || (
            search[REGEX_DATA][cacheKey] = copyRegex(search, {
                addG: !!global,
                removeG: scope === 'one',
                isInternalOnly: true
            })
        );
    } else if (global) {
        s2 = new RegExp(XRegExp.escape(String(search)), 'g');
    }

    // Fixed 'replace' required for named backreferences, etc.
    result = fixed.replace.call(toObject(str), s2, replacement);

    if (isRegex && search.global) {
        // Fixes IE, Safari bug (last tested IE 9, Safari 5.1)
        search.lastIndex = 0;
    }

    return result;
}
```
- example usage
```shell
...
while (match = XRegExp.exec('<1><2><3><4>5<6>', /<(\d+)>/, pos, 'sticky')) {
    result.push(match[1]);
    pos = match.index + match[0].length;
}
// result -> ['2', '3', '4']

// XRegExp.replace allows named backreferences in replacements
XRegExp.replace('2015-02-22', date, '${month}/${day}/${year}');
// -> '02/22/2015'
XRegExp.replace('2015-02-22', date, function(match) {
    return match.month + '/' + match.day + '/' + match.year;
});
// -> '02/22/2015'

// In fact, XRegExps compile to RegExps and work perfectly with native methods
...
```

#### <a name="apidoc.element.xregexp.replaceEach"></a>[function <span class="apidocSignatureSpan">xregexp.</span>replaceEach (str, replacements)](#apidoc.element.xregexp.replaceEach)
- description and source-code
```javascript
replaceEach = function (str, replacements) {
    var i, r;

    for (i = 0; i < replacements.length; ++i) {
        r = replacements[i];
        str = XRegExp.replace(str, r[0], r[1], r[2]);
    }

    return str;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.split"></a>[function <span class="apidocSignatureSpan">xregexp.</span>split (str, separator, limit)](#apidoc.element.xregexp.split)
- description and source-code
```javascript
split = function (str, separator, limit) {
    return fixed.split.call(toObject(str), separator, limit);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.test"></a>[function <span class="apidocSignatureSpan">xregexp.</span>test (str, regex, pos, sticky)](#apidoc.element.xregexp.test)
- description and source-code
```javascript
test = function (str, regex, pos, sticky) {
    // Do this the easy way :-)
    return !!XRegExp.exec(str, regex, pos, sticky);
}
```
- example usage
```shell
...
// -> '02/22/2015'
XRegExp.replace('2015-02-22', date, function(match) {
    return match.month + '/' + match.day + '/' + match.year;
});
// -> '02/22/2015'

// In fact, XRegExps compile to RegExps and work perfectly with native methods
date.test('2015-02-22');
// -> true

// The only caveat is that named captures must be referenced using numbered
// backreferences if used with native methods
'2015-02-22'.replace(date, '$2/$3/$1');
// -> '02/22/2015'
...
```

#### <a name="apidoc.element.xregexp.uninstall"></a>[function <span class="apidocSignatureSpan">xregexp.</span>uninstall (options)](#apidoc.element.xregexp.uninstall)
- description and source-code
```javascript
uninstall = function (options) {
    options = prepareOptions(options);

    if (features.astral && options.astral) {
        setAstral(false);
    }

    if (features.natives && options.natives) {
        setNatives(false);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.union"></a>[function <span class="apidocSignatureSpan">xregexp.</span>union (patterns, flags)](#apidoc.element.xregexp.union)
- description and source-code
```javascript
union = function (patterns, flags) {
    var numCaptures = 0;
    var numPriorCaptures;
    var captureNames;

    function rewrite(match, paren, backref) {
        var name = captureNames[numCaptures - numPriorCaptures];

        // Capturing group
        if (paren) {
            ++numCaptures;
            // If the current capture has a name, preserve the name
            if (name) {
                return '(?<' + name + '>';
            }
        // Backreference
        } else if (backref) {
            // Rewrite the backreference
            return '\\' + (+backref + numPriorCaptures);
        }

        return match;
    }

    if (!(isType(patterns, 'Array') && patterns.length)) {
        throw new TypeError('Must provide a nonempty array of patterns to merge');
    }

    var parts = /(\()(?!\?)|\\([1-9]\d*)|\\[\s\S]|\[(?:[^\\\]]|\\[\s\S])*]/g;
    var output = [];
    var pattern;
    for (var i = 0; i < patterns.length; ++i) {
        pattern = patterns[i];

        if (XRegExp.isRegExp(pattern)) {
            numPriorCaptures = numCaptures;
            captureNames = (pattern[REGEX_DATA] && pattern[REGEX_DATA].captureNames) || [];

            // Rewrite backreferences. Passing to XRegExp dies on octals and ensures patterns are
            // independently valid; helps keep this simple. Named captures are put back
            output.push(nativ.replace.call(XRegExp(pattern.source).source, parts, rewrite));
        } else {
            output.push(XRegExp.escape(pattern));
        }
    }

    return XRegExp(output.join('|'), flags);
}
```
- example usage
```shell
...
XRegExp.matchChain(html, [
    {regex: /<a href="([^"]+)">/i, backref: 1},
    {regex: XRegExp('(?i)^https?://(?<domain>[^/?#]+)'), backref: 'domain'}
]);
// -> ['xregexp.com', 'www.google.com']

// Merge strings and regexes into a single pattern with updated backreferences
XRegExp.union(['a+b*c', /(dog)\1/, /(cat)\1/], 'i');
// -> /a\+b\*c|(dog)\1|(cat)\2/i
'''

These examples give the flavor of what's possible, but XRegExp has more syntax, flags, methods, options, and browser fixes that
aren't shown here. You can even augment XRegExp's regular expression syntax with addons (see below) or write your own. See [xregexp
.com](http://xregexp.com/) for details.

## Addons
...
```



# <a name="apidoc.module.xregexp.cache"></a>[module xregexp.cache](#apidoc.module.xregexp.cache)

#### <a name="apidoc.element.xregexp.cache.cache"></a>[function <span class="apidocSignatureSpan">xregexp.</span>cache (pattern, flags)](#apidoc.element.xregexp.cache.cache)
- description and source-code
```javascript
cache = function (pattern, flags) {
    if (!regexCache[pattern]) {
        regexCache[pattern] = {};
    }
    return regexCache[pattern][flags] || (
        regexCache[pattern][flags] = XRegExp(pattern, flags)
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.xregexp.cache.flush"></a>[function <span class="apidocSignatureSpan">xregexp.cache.</span>flush (cacheName)](#apidoc.element.xregexp.cache.flush)
- description and source-code
```javascript
flush = function (cacheName) {
    if (cacheName === 'patterns') {
        // Flush the pattern cache used by the 'XRegExp' constructor
        patternCache = {};
    } else {
        // Flush the regex cache populated by 'XRegExp.cache'
        regexCache = {};
    }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
