# api documentation for  [cash (v0.8.0)](https://github.com/dthree/cash#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cash.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cash) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cash.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cash)
#### Cross-platform Linux commands in pure ES6.

[![NPM](https://nodei.co/npm/cash.png?downloads=true)](https://www.npmjs.com/package/cash)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cash/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-cash%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cash/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cash/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cash/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "dthree"
    },
    "bin": {
        "$": "./bin/cash.js",
        "cash": "./bin/cash.js"
    },
    "bugs": {
        "url": "https://github.com/dthree/cash/issues"
    },
    "dependencies": {
        "array-shuffle": "^1.0.0",
        "chalk": "^1.1.0",
        "filesize": "^3.1.3",
        "fkill": "^3.1.0",
        "fs-extra": "^0.23.1",
        "glob": "^6.0.4",
        "lodash": "^4.0.0",
        "minimist": "^1.2.0",
        "user-home": "^2.0.0",
        "username": "^1.0.1",
        "vorpal": "^1.10.8",
        "vorpal-autocomplete-fs": "0.0.3",
        "vorpal-grep": "^0.1.2",
        "vorpal-less": "0.0.13"
    },
    "description": "Cross-platform Linux commands in pure ES6.",
    "devDependencies": {
        "babel-core": "^6.5.2",
        "babel-preset-es2015": "^6.5.0",
        "coveralls": "^2.11.6",
        "gulp": "^3.9.0",
        "gulp-babel": "^6.1.2",
        "gulp-changed": "^1.3.0",
        "gulp-eslint": "^2.0.0",
        "istanbul": "^0.4.2",
        "mocha": "^2.2.5",
        "shelljs": "^0.6.0",
        "should": "^7.0.3",
        "webpack": "^1.12.13",
        "xo": "^0.12.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0a0b289e87abccb30c504b006b6f975b8955c16b",
        "tarball": "https://registry.npmjs.org/cash/-/cash-0.8.0.tgz"
    },
    "engines": {
        "iojs": ">= 1.0.0",
        "node": ">= 4"
    },
    "files": [
        "commands.json",
        "dist",
        "bin"
    ],
    "gitHead": "e0e21e1a193adef6cb8a9cd6965d94d0fd34f939",
    "homepage": "https://github.com/dthree/cash#readme",
    "keywords": [
        "terminal",
        "emulator",
        "cygwin",
        "cli",
        "windows",
        "linux",
        "unix",
        "posix",
        "shell",
        "shelljs",
        "bash",
        "cash",
        "$",
        "tty",
        "util",
        "vorpal",
        "vorpal.js"
    ],
    "license": "MIT",
    "main": "./dist/index.js",
    "maintainers": [
        {
            "name": "aseemk",
            "email": "aseem.kishore@gmail.com"
        },
        {
            "name": "dthree",
            "email": "threedeecee@gmail.com"
        }
    ],
    "name": "cash",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dthree/cash.git"
    },
    "scripts": {
        "lint": "xo ./src/*.js ./src/**/*.js ./test/*.js",
        "test": "gulp builder; ./node_modules/istanbul/lib/cli.js cover --root './dist' -x './dist/lib/sugar.js' _mocha -- -R spec && npm run lint",
        "test-win": "mocha"
    },
    "version": "0.8.0",
    "xo": {
        "envs": [
            "node",
            "mocha"
        ],
        "space": true,
        "esnext": true,
        "rules": {
            "prefer-arrow-callback": 0,
            "no-loop-func": 0,
            "no-nested-ternary": 0,
            "no-constant-condition": 0,
            "no-use-extend-native/no-use-extend-native": 0,
            "no-negated-condition": 0,
            "no-inner-declarations": 0,
            "prefer-reflect": 0,
            "wrap-iife": 0,
            "no-unused-expressions": 0,
            "global-require": 0
        }
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cash](#apidoc.module.cash)
1.  [function <span class="apidocSignatureSpan">cash.</span>alias (args, options, callback)](#apidoc.element.cash.alias)
1.  [function <span class="apidocSignatureSpan">cash.</span>cat (args, options, callback)](#apidoc.element.cash.cat)
1.  [function <span class="apidocSignatureSpan">cash.</span>cd (args, options, callback)](#apidoc.element.cash.cd)
1.  [function <span class="apidocSignatureSpan">cash.</span>clear (args, options, callback)](#apidoc.element.cash.clear)
1.  [function <span class="apidocSignatureSpan">cash.</span>cp (args, options, callback)](#apidoc.element.cash.cp)
1.  [function <span class="apidocSignatureSpan">cash.</span>echo (args, options, callback)](#apidoc.element.cash.echo)
1.  [function <span class="apidocSignatureSpan">cash.</span>export (args, options, callback)](#apidoc.element.cash.export)
1.  [function <span class="apidocSignatureSpan">cash.</span>false (args, options, callback)](#apidoc.element.cash.false)
1.  [function <span class="apidocSignatureSpan">cash.</span>grep (args, options, callback)](#apidoc.element.cash.grep)
1.  [function <span class="apidocSignatureSpan">cash.</span>head (args, options, callback)](#apidoc.element.cash.head)
1.  [function <span class="apidocSignatureSpan">cash.</span>kill (args, options, callback)](#apidoc.element.cash.kill)
1.  [function <span class="apidocSignatureSpan">cash.</span>less (args, options, callback)](#apidoc.element.cash.less)
1.  [function <span class="apidocSignatureSpan">cash.</span>ls (args, options, callback)](#apidoc.element.cash.ls)
1.  [function <span class="apidocSignatureSpan">cash.</span>mkdir (args, options, callback)](#apidoc.element.cash.mkdir)
1.  [function <span class="apidocSignatureSpan">cash.</span>mv (args, options, callback)](#apidoc.element.cash.mv)
1.  [function <span class="apidocSignatureSpan">cash.</span>pwd (args, options, callback)](#apidoc.element.cash.pwd)
1.  [function <span class="apidocSignatureSpan">cash.</span>rm (args, options, callback)](#apidoc.element.cash.rm)
1.  [function <span class="apidocSignatureSpan">cash.</span>show ()](#apidoc.element.cash.show)
1.  [function <span class="apidocSignatureSpan">cash.</span>sort (args, options, callback)](#apidoc.element.cash.sort)
1.  [function <span class="apidocSignatureSpan">cash.</span>source (args, options, callback)](#apidoc.element.cash.source)
1.  [function <span class="apidocSignatureSpan">cash.</span>tail (args, options, callback)](#apidoc.element.cash.tail)
1.  [function <span class="apidocSignatureSpan">cash.</span>touch (args, options, callback)](#apidoc.element.cash.touch)
1.  [function <span class="apidocSignatureSpan">cash.</span>true (args, options, callback)](#apidoc.element.cash.true)
1.  [function <span class="apidocSignatureSpan">cash.</span>unalias (args, options, callback)](#apidoc.element.cash.unalias)
1.  [function <span class="apidocSignatureSpan">cash.</span>vorpal.Session (options)](#apidoc.element.cash.vorpal.Session)
1.  function <span class="apidocSignatureSpan">cash.</span>vorpal.lodash
1.  object <span class="apidocSignatureSpan">cash.</span>vorpal
1.  object <span class="apidocSignatureSpan">cash.</span>vorpal.Session.prototype
1.  object <span class="apidocSignatureSpan">cash.</span>vorpal.chalk
1.  object <span class="apidocSignatureSpan">cash.</span>vorpal.lodash.prototype
1.  object <span class="apidocSignatureSpan">cash.</span>vorpal.ui
1.  object <span class="apidocSignatureSpan">cash.</span>vorpal.util

#### [module cash.vorpal](#apidoc.module.cash.vorpal)
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.</span>_hooked
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.</span>_useDeprecatedAutocompletion
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.</span>executables
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.</span>isCommandArgKeyPairNormalized
1.  [function <span class="apidocSignatureSpan">cash.vorpal.</span>Session (options)](#apidoc.element.cash.vorpal.Session)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.</span>_help ()](#apidoc.element.cash.vorpal._help)
1.  function <span class="apidocSignatureSpan">cash.vorpal.</span>lodash
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>_aliases
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>_queue
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>api
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>chalk
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>cmdHistory
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>commands
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>server
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>session
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>ui
1.  object <span class="apidocSignatureSpan">cash.vorpal.</span>util
1.  string <span class="apidocSignatureSpan">cash.vorpal.</span>_delimiter
1.  string <span class="apidocSignatureSpan">cash.vorpal.</span>_version

#### [module cash.vorpal.Session](#apidoc.module.cash.vorpal.Session)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.</span>Session (options)](#apidoc.element.cash.vorpal.Session.Session)

#### [module cash.vorpal.Session.prototype](#apidoc.module.cash.vorpal.Session.prototype)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>_autocomplete (str, arr)](#apidoc.element.cash.vorpal.Session.prototype._autocomplete)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>_guid ()](#apidoc.element.cash.vorpal.Session.prototype._guid)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>_log ()](#apidoc.element.cash.vorpal.Session.prototype._log)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>completeCommand ()](#apidoc.element.cash.vorpal.Session.prototype.completeCommand)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>delimiter (str)](#apidoc.element.cash.vorpal.Session.prototype.delimiter)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>execCommandSet (wrapper, callback)](#apidoc.element.cash.vorpal.Session.prototype.execCommandSet)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>fullDelimiter ()](#apidoc.element.cash.vorpal.Session.prototype.fullDelimiter)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getAutocomplete (str, cb)](#apidoc.element.cash.vorpal.Session.prototype.getAutocomplete)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getAutocompleteDeprecated (str, cb)](#apidoc.element.cash.vorpal.Session.prototype.getAutocompleteDeprecated)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getHistory (direction)](#apidoc.element.cash.vorpal.Session.prototype.getHistory)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getKeypressResult (key, value, cb)](#apidoc.element.cash.vorpal.Session.prototype.getKeypressResult)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>help (command)](#apidoc.element.cash.vorpal.Session.prototype.help)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>history (str)](#apidoc.element.cash.vorpal.Session.prototype.history)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>isLocal ()](#apidoc.element.cash.vorpal.Session.prototype.isLocal)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>log ()](#apidoc.element.cash.vorpal.Session.prototype.log)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>match (str, arr)](#apidoc.element.cash.vorpal.Session.prototype.match)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>modeDelimiter (str)](#apidoc.element.cash.vorpal.Session.prototype.modeDelimiter)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>prompt (options, cb)](#apidoc.element.cash.vorpal.Session.prototype.prompt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>registerCommand ()](#apidoc.element.cash.vorpal.Session.prototype.registerCommand)

#### [module cash.vorpal.chalk](#apidoc.module.cash.vorpal.chalk)
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>enabled
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>supportsColor
1.  [function <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>hasColor ()](#apidoc.element.cash.vorpal.chalk.hasColor)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>stripColor (str)](#apidoc.element.cash.vorpal.chalk.stripColor)
1.  object <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>styles

#### [module cash.vorpal.lodash](#apidoc.module.cash.vorpal.lodash)
1.  function <span class="apidocSignatureSpan">cash.vorpal.</span>lodash
1.  function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>_
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>add (value, other)](#apidoc.element.cash.vorpal.lodash.add)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>after (n, func)](#apidoc.element.cash.vorpal.lodash.after)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>ary (func, n, guard)](#apidoc.element.cash.vorpal.lodash.ary)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assign (object, sources)](#apidoc.element.cash.vorpal.lodash.assign)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assignIn (object, sources)](#apidoc.element.cash.vorpal.lodash.assignIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assignInWith (object, sources)](#apidoc.element.cash.vorpal.lodash.assignInWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assignWith (object, sources)](#apidoc.element.cash.vorpal.lodash.assignWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>at (object, paths)](#apidoc.element.cash.vorpal.lodash.at)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>attempt (func, args)](#apidoc.element.cash.vorpal.lodash.attempt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>before (n, func)](#apidoc.element.cash.vorpal.lodash.before)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>bind (func, thisArg, partials)](#apidoc.element.cash.vorpal.lodash.bind)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>bindAll (object, methodNames)](#apidoc.element.cash.vorpal.lodash.bindAll)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>bindKey (object, key, partials)](#apidoc.element.cash.vorpal.lodash.bindKey)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>camelCase (string)](#apidoc.element.cash.vorpal.lodash.camelCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>capitalize (string)](#apidoc.element.cash.vorpal.lodash.capitalize)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>castArray ()](#apidoc.element.cash.vorpal.lodash.castArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>ceil (number, precision)](#apidoc.element.cash.vorpal.lodash.ceil)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>chain (value)](#apidoc.element.cash.vorpal.lodash.chain)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>chunk (array, size, guard)](#apidoc.element.cash.vorpal.lodash.chunk)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>clamp (number, lower, upper)](#apidoc.element.cash.vorpal.lodash.clamp)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>clone (value)](#apidoc.element.cash.vorpal.lodash.clone)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cloneDeep (value)](#apidoc.element.cash.vorpal.lodash.cloneDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cloneDeepWith (value, customizer)](#apidoc.element.cash.vorpal.lodash.cloneDeepWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cloneWith (value, customizer)](#apidoc.element.cash.vorpal.lodash.cloneWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>compact (array)](#apidoc.element.cash.vorpal.lodash.compact)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>concat ()](#apidoc.element.cash.vorpal.lodash.concat)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cond (pairs)](#apidoc.element.cash.vorpal.lodash.cond)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>conforms (source)](#apidoc.element.cash.vorpal.lodash.conforms)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>conformsTo (object, source)](#apidoc.element.cash.vorpal.lodash.conformsTo)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>constant (value)](#apidoc.element.cash.vorpal.lodash.constant)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>countBy (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.countBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>create (prototype, properties)](#apidoc.element.cash.vorpal.lodash.create)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>curry (func, arity, guard)](#apidoc.element.cash.vorpal.lodash.curry)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>curryRight (func, arity, guard)](#apidoc.element.cash.vorpal.lodash.curryRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>debounce (func, wait, options)](#apidoc.element.cash.vorpal.lodash.debounce)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>deburr (string)](#apidoc.element.cash.vorpal.lodash.deburr)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defaultTo (value, defaultValue)](#apidoc.element.cash.vorpal.lodash.defaultTo)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defaults (args)](#apidoc.element.cash.vorpal.lodash.defaults)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defaultsDeep (args)](#apidoc.element.cash.vorpal.lodash.defaultsDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defer (func, args)](#apidoc.element.cash.vorpal.lodash.defer)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>delay (func, wait, args)](#apidoc.element.cash.vorpal.lodash.delay)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>difference (array, values)](#apidoc.element.cash.vorpal.lodash.difference)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>differenceBy (array, values)](#apidoc.element.cash.vorpal.lodash.differenceBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>differenceWith (array, values)](#apidoc.element.cash.vorpal.lodash.differenceWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>divide (value, other)](#apidoc.element.cash.vorpal.lodash.divide)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>drop (array, n, guard)](#apidoc.element.cash.vorpal.lodash.drop)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>dropRight (array, n, guard)](#apidoc.element.cash.vorpal.lodash.dropRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>dropRightWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.dropRightWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>dropWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.dropWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>each (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.each)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>eachRight (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.eachRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>endsWith (string, target, position)](#apidoc.element.cash.vorpal.lodash.endsWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>entries (object)](#apidoc.element.cash.vorpal.lodash.entries)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>entriesIn (object)](#apidoc.element.cash.vorpal.lodash.entriesIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>eq (value, other)](#apidoc.element.cash.vorpal.lodash.eq)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>escape (string)](#apidoc.element.cash.vorpal.lodash.escape)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>escapeRegExp (string)](#apidoc.element.cash.vorpal.lodash.escapeRegExp)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>every (collection, predicate, guard)](#apidoc.element.cash.vorpal.lodash.every)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>extend (object, sources)](#apidoc.element.cash.vorpal.lodash.extend)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>extendWith (object, sources)](#apidoc.element.cash.vorpal.lodash.extendWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>fill (array, value, start, end)](#apidoc.element.cash.vorpal.lodash.fill)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>filter (collection, predicate)](#apidoc.element.cash.vorpal.lodash.filter)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>find (collection, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.find)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findIndex (array, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.findIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findKey (object, predicate)](#apidoc.element.cash.vorpal.lodash.findKey)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findLast (collection, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.findLast)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findLastIndex (array, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.findLastIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findLastKey (object, predicate)](#apidoc.element.cash.vorpal.lodash.findLastKey)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>first (array)](#apidoc.element.cash.vorpal.lodash.first)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatMap (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.flatMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatMapDeep (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.flatMapDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatMapDepth (collection, iteratee, depth)](#apidoc.element.cash.vorpal.lodash.flatMapDepth)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatten (array)](#apidoc.element.cash.vorpal.lodash.flatten)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flattenDeep (array)](#apidoc.element.cash.vorpal.lodash.flattenDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flattenDepth (array, depth)](#apidoc.element.cash.vorpal.lodash.flattenDepth)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flip (func)](#apidoc.element.cash.vorpal.lodash.flip)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>floor (number, precision)](#apidoc.element.cash.vorpal.lodash.floor)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flow (funcs)](#apidoc.element.cash.vorpal.lodash.flow)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flowRight (funcs)](#apidoc.element.cash.vorpal.lodash.flowRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forEach (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.forEach)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forEachRight (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.forEachRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forIn (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forInRight (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forInRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forOwn (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forOwn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forOwnRight (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forOwnRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>fromPairs (pairs)](#apidoc.element.cash.vorpal.lodash.fromPairs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>functions (object)](#apidoc.element.cash.vorpal.lodash.functions)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>functionsIn (object)](#apidoc.element.cash.vorpal.lodash.functionsIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>get (object, path, defaultValue)](#apidoc.element.cash.vorpal.lodash.get)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>groupBy (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.groupBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>gt (value, other)](#apidoc.element.cash.vorpal.lodash.gt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>gte (value, other)](#apidoc.element.cash.vorpal.lodash.gte)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>has (object, path)](#apidoc.element.cash.vorpal.lodash.has)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>hasIn (object, path)](#apidoc.element.cash.vorpal.lodash.hasIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>head (array)](#apidoc.element.cash.vorpal.lodash.head)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>identity (value)](#apidoc.element.cash.vorpal.lodash.identity)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>inRange (number, start, end)](#apidoc.element.cash.vorpal.lodash.inRange)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>includes (collection, value, fromIndex, guard)](#apidoc.element.cash.vorpal.lodash.includes)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>indexOf (array, value, fromIndex)](#apidoc.element.cash.vorpal.lodash.indexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>initial (array)](#apidoc.element.cash.vorpal.lodash.initial)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>intersection (arrays)](#apidoc.element.cash.vorpal.lodash.intersection)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>intersectionBy (arrays)](#apidoc.element.cash.vorpal.lodash.intersectionBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>intersectionWith (arrays)](#apidoc.element.cash.vorpal.lodash.intersectionWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invert (object, iteratee)](#apidoc.element.cash.vorpal.lodash.invert)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invertBy (object, iteratee)](#apidoc.element.cash.vorpal.lodash.invertBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invoke (object, path, args)](#apidoc.element.cash.vorpal.lodash.invoke)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invokeMap (collection, path, args)](#apidoc.element.cash.vorpal.lodash.invokeMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArguments (value)](#apidoc.element.cash.vorpal.lodash.isArguments)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArray ()](#apidoc.element.cash.vorpal.lodash.isArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArrayBuffer (value)](#apidoc.element.cash.vorpal.lodash.isArrayBuffer)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArrayLike (value)](#apidoc.element.cash.vorpal.lodash.isArrayLike)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArrayLikeObject (value)](#apidoc.element.cash.vorpal.lodash.isArrayLikeObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isBoolean (value)](#apidoc.element.cash.vorpal.lodash.isBoolean)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isBuffer (b)](#apidoc.element.cash.vorpal.lodash.isBuffer)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isDate (value)](#apidoc.element.cash.vorpal.lodash.isDate)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isElement (value)](#apidoc.element.cash.vorpal.lodash.isElement)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isEmpty (value)](#apidoc.element.cash.vorpal.lodash.isEmpty)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isEqual (value, other)](#apidoc.element.cash.vorpal.lodash.isEqual)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isEqualWith (value, other, customizer)](#apidoc.element.cash.vorpal.lodash.isEqualWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isError (value)](#apidoc.element.cash.vorpal.lodash.isError)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isFinite (value)](#apidoc.element.cash.vorpal.lodash.isFinite)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isFunction (value)](#apidoc.element.cash.vorpal.lodash.isFunction)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isInteger (value)](#apidoc.element.cash.vorpal.lodash.isInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isLength (value)](#apidoc.element.cash.vorpal.lodash.isLength)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isMap (value)](#apidoc.element.cash.vorpal.lodash.isMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isMatch (object, source)](#apidoc.element.cash.vorpal.lodash.isMatch)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isMatchWith (object, source, customizer)](#apidoc.element.cash.vorpal.lodash.isMatchWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNaN (value)](#apidoc.element.cash.vorpal.lodash.isNaN)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNative (value)](#apidoc.element.cash.vorpal.lodash.isNative)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNil (value)](#apidoc.element.cash.vorpal.lodash.isNil)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNull (value)](#apidoc.element.cash.vorpal.lodash.isNull)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNumber (value)](#apidoc.element.cash.vorpal.lodash.isNumber)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isObject (value)](#apidoc.element.cash.vorpal.lodash.isObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isObjectLike (value)](#apidoc.element.cash.vorpal.lodash.isObjectLike)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isPlainObject (value)](#apidoc.element.cash.vorpal.lodash.isPlainObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isRegExp (value)](#apidoc.element.cash.vorpal.lodash.isRegExp)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isSafeInteger (value)](#apidoc.element.cash.vorpal.lodash.isSafeInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isSet (value)](#apidoc.element.cash.vorpal.lodash.isSet)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isString (value)](#apidoc.element.cash.vorpal.lodash.isString)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isSymbol (value)](#apidoc.element.cash.vorpal.lodash.isSymbol)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isTypedArray (value)](#apidoc.element.cash.vorpal.lodash.isTypedArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isUndefined (value)](#apidoc.element.cash.vorpal.lodash.isUndefined)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isWeakMap (value)](#apidoc.element.cash.vorpal.lodash.isWeakMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isWeakSet (value)](#apidoc.element.cash.vorpal.lodash.isWeakSet)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>iteratee (func)](#apidoc.element.cash.vorpal.lodash.iteratee)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>join (array, separator)](#apidoc.element.cash.vorpal.lodash.join)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>kebabCase (string)](#apidoc.element.cash.vorpal.lodash.kebabCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>keyBy (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.keyBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>keys (object)](#apidoc.element.cash.vorpal.lodash.keys)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>keysIn (object)](#apidoc.element.cash.vorpal.lodash.keysIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>last (array)](#apidoc.element.cash.vorpal.lodash.last)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lastIndexOf (array, value, fromIndex)](#apidoc.element.cash.vorpal.lodash.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lowerCase (string)](#apidoc.element.cash.vorpal.lodash.lowerCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lowerFirst (string)](#apidoc.element.cash.vorpal.lodash.lowerFirst)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lt (value, other)](#apidoc.element.cash.vorpal.lodash.lt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lte (value, other)](#apidoc.element.cash.vorpal.lodash.lte)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>map (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.map)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mapKeys (object, iteratee)](#apidoc.element.cash.vorpal.lodash.mapKeys)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mapValues (object, iteratee)](#apidoc.element.cash.vorpal.lodash.mapValues)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>matches (source)](#apidoc.element.cash.vorpal.lodash.matches)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>matchesProperty (path, srcValue)](#apidoc.element.cash.vorpal.lodash.matchesProperty)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>max (array)](#apidoc.element.cash.vorpal.lodash.max)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>maxBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.maxBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mean (array)](#apidoc.element.cash.vorpal.lodash.mean)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>meanBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.meanBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>memoize (func, resolver)](#apidoc.element.cash.vorpal.lodash.memoize)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>merge (object, sources)](#apidoc.element.cash.vorpal.lodash.merge)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mergeWith (object, sources)](#apidoc.element.cash.vorpal.lodash.mergeWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>method (path, args)](#apidoc.element.cash.vorpal.lodash.method)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>methodOf (object, args)](#apidoc.element.cash.vorpal.lodash.methodOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>min (array)](#apidoc.element.cash.vorpal.lodash.min)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>minBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.minBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mixin (object, source, options)](#apidoc.element.cash.vorpal.lodash.mixin)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>multiply (value, other)](#apidoc.element.cash.vorpal.lodash.multiply)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>negate (predicate)](#apidoc.element.cash.vorpal.lodash.negate)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>noConflict ()](#apidoc.element.cash.vorpal.lodash.noConflict)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>noop ()](#apidoc.element.cash.vorpal.lodash.noop)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>now ()](#apidoc.element.cash.vorpal.lodash.now)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>nth (array, n)](#apidoc.element.cash.vorpal.lodash.nth)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>nthArg (n)](#apidoc.element.cash.vorpal.lodash.nthArg)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>omit (object, paths)](#apidoc.element.cash.vorpal.lodash.omit)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>omitBy (object, predicate)](#apidoc.element.cash.vorpal.lodash.omitBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>once (func)](#apidoc.element.cash.vorpal.lodash.once)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>orderBy (collection, iteratees, orders, guard)](#apidoc.element.cash.vorpal.lodash.orderBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>over (iteratees)](#apidoc.element.cash.vorpal.lodash.over)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>overArgs (func, transforms)](#apidoc.element.cash.vorpal.lodash.overArgs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>overEvery (iteratees)](#apidoc.element.cash.vorpal.lodash.overEvery)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>overSome (iteratees)](#apidoc.element.cash.vorpal.lodash.overSome)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pad (string, length, chars)](#apidoc.element.cash.vorpal.lodash.pad)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>padEnd (string, length, chars)](#apidoc.element.cash.vorpal.lodash.padEnd)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>padStart (string, length, chars)](#apidoc.element.cash.vorpal.lodash.padStart)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>parseInt (string, radix, guard)](#apidoc.element.cash.vorpal.lodash.parseInt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>partial (func, partials)](#apidoc.element.cash.vorpal.lodash.partial)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>partialRight (func, partials)](#apidoc.element.cash.vorpal.lodash.partialRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>partition (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.partition)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pick (object, paths)](#apidoc.element.cash.vorpal.lodash.pick)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pickBy (object, predicate)](#apidoc.element.cash.vorpal.lodash.pickBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>property (path)](#apidoc.element.cash.vorpal.lodash.property)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>propertyOf (object)](#apidoc.element.cash.vorpal.lodash.propertyOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pull (array, values)](#apidoc.element.cash.vorpal.lodash.pull)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAll (array, values)](#apidoc.element.cash.vorpal.lodash.pullAll)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAllBy (array, values, iteratee)](#apidoc.element.cash.vorpal.lodash.pullAllBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAllWith (array, values, comparator)](#apidoc.element.cash.vorpal.lodash.pullAllWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAt (array, indexes)](#apidoc.element.cash.vorpal.lodash.pullAt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>random (lower, upper, floating)](#apidoc.element.cash.vorpal.lodash.random)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>range (start, end, step)](#apidoc.element.cash.vorpal.lodash.range)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>rangeRight (start, end, step)](#apidoc.element.cash.vorpal.lodash.rangeRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>rearg (func, indexes)](#apidoc.element.cash.vorpal.lodash.rearg)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reduce (collection, iteratee, accumulator)](#apidoc.element.cash.vorpal.lodash.reduce)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reduceRight (collection, iteratee, accumulator)](#apidoc.element.cash.vorpal.lodash.reduceRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reject (collection, predicate)](#apidoc.element.cash.vorpal.lodash.reject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>remove (array, predicate)](#apidoc.element.cash.vorpal.lodash.remove)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>repeat (string, n, guard)](#apidoc.element.cash.vorpal.lodash.repeat)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>replace ()](#apidoc.element.cash.vorpal.lodash.replace)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>rest (func, start)](#apidoc.element.cash.vorpal.lodash.rest)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>result (object, path, defaultValue)](#apidoc.element.cash.vorpal.lodash.result)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reverse (array)](#apidoc.element.cash.vorpal.lodash.reverse)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>round (number, precision)](#apidoc.element.cash.vorpal.lodash.round)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>runInContext (context)](#apidoc.element.cash.vorpal.lodash.runInContext)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sample (collection)](#apidoc.element.cash.vorpal.lodash.sample)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sampleSize (collection, n, guard)](#apidoc.element.cash.vorpal.lodash.sampleSize)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>set (object, path, value)](#apidoc.element.cash.vorpal.lodash.set)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>setWith (object, path, value, customizer)](#apidoc.element.cash.vorpal.lodash.setWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>shuffle (collection)](#apidoc.element.cash.vorpal.lodash.shuffle)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>size (collection)](#apidoc.element.cash.vorpal.lodash.size)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>slice (array, start, end)](#apidoc.element.cash.vorpal.lodash.slice)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>snakeCase (string)](#apidoc.element.cash.vorpal.lodash.snakeCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>some (collection, predicate, guard)](#apidoc.element.cash.vorpal.lodash.some)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortBy (collection, iteratees)](#apidoc.element.cash.vorpal.lodash.sortBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedIndex (array, value)](#apidoc.element.cash.vorpal.lodash.sortedIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedIndexBy (array, value, iteratee)](#apidoc.element.cash.vorpal.lodash.sortedIndexBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedIndexOf (array, value)](#apidoc.element.cash.vorpal.lodash.sortedIndexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedLastIndex (array, value)](#apidoc.element.cash.vorpal.lodash.sortedLastIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedLastIndexBy (array, value, iteratee)](#apidoc.element.cash.vorpal.lodash.sortedLastIndexBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedLastIndexOf (array, value)](#apidoc.element.cash.vorpal.lodash.sortedLastIndexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedUniq (array)](#apidoc.element.cash.vorpal.lodash.sortedUniq)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedUniqBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.sortedUniqBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>split (string, separator, limit)](#apidoc.element.cash.vorpal.lodash.split)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>spread (func, start)](#apidoc.element.cash.vorpal.lodash.spread)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>startCase (string)](#apidoc.element.cash.vorpal.lodash.startCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>startsWith (string, target, position)](#apidoc.element.cash.vorpal.lodash.startsWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubArray ()](#apidoc.element.cash.vorpal.lodash.stubArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubFalse ()](#apidoc.element.cash.vorpal.lodash.stubFalse)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubObject ()](#apidoc.element.cash.vorpal.lodash.stubObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubString ()](#apidoc.element.cash.vorpal.lodash.stubString)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubTrue ()](#apidoc.element.cash.vorpal.lodash.stubTrue)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>subtract (value, other)](#apidoc.element.cash.vorpal.lodash.subtract)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sum (array)](#apidoc.element.cash.vorpal.lodash.sum)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sumBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.sumBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>tail (array)](#apidoc.element.cash.vorpal.lodash.tail)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>take (array, n, guard)](#apidoc.element.cash.vorpal.lodash.take)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>takeRight (array, n, guard)](#apidoc.element.cash.vorpal.lodash.takeRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>takeRightWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.takeRightWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>takeWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.takeWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>tap (value, interceptor)](#apidoc.element.cash.vorpal.lodash.tap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>template (string, options, guard)](#apidoc.element.cash.vorpal.lodash.template)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>throttle (func, wait, options)](#apidoc.element.cash.vorpal.lodash.throttle)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>thru (value, interceptor)](#apidoc.element.cash.vorpal.lodash.thru)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>times (n, iteratee)](#apidoc.element.cash.vorpal.lodash.times)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toArray (value)](#apidoc.element.cash.vorpal.lodash.toArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toFinite (value)](#apidoc.element.cash.vorpal.lodash.toFinite)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toInteger (value)](#apidoc.element.cash.vorpal.lodash.toInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toLength (value)](#apidoc.element.cash.vorpal.lodash.toLength)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toLower (value)](#apidoc.element.cash.vorpal.lodash.toLower)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toNumber (value)](#apidoc.element.cash.vorpal.lodash.toNumber)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPairs (object)](#apidoc.element.cash.vorpal.lodash.toPairs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPairsIn (object)](#apidoc.element.cash.vorpal.lodash.toPairsIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPath (value)](#apidoc.element.cash.vorpal.lodash.toPath)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPlainObject (value)](#apidoc.element.cash.vorpal.lodash.toPlainObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toSafeInteger (value)](#apidoc.element.cash.vorpal.lodash.toSafeInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toString (value)](#apidoc.element.cash.vorpal.lodash.toString)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toUpper (value)](#apidoc.element.cash.vorpal.lodash.toUpper)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>transform (object, iteratee, accumulator)](#apidoc.element.cash.vorpal.lodash.transform)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>trim (string, chars, guard)](#apidoc.element.cash.vorpal.lodash.trim)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>trimEnd (string, chars, guard)](#apidoc.element.cash.vorpal.lodash.trimEnd)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>trimStart (string, chars, guard)](#apidoc.element.cash.vorpal.lodash.trimStart)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>truncate (string, options)](#apidoc.element.cash.vorpal.lodash.truncate)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unary (func)](#apidoc.element.cash.vorpal.lodash.unary)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unescape (string)](#apidoc.element.cash.vorpal.lodash.unescape)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>union (arrays)](#apidoc.element.cash.vorpal.lodash.union)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unionBy (arrays)](#apidoc.element.cash.vorpal.lodash.unionBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unionWith (arrays)](#apidoc.element.cash.vorpal.lodash.unionWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniq (array)](#apidoc.element.cash.vorpal.lodash.uniq)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniqBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.uniqBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniqWith (array, comparator)](#apidoc.element.cash.vorpal.lodash.uniqWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniqueId (prefix)](#apidoc.element.cash.vorpal.lodash.uniqueId)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unset (object, path)](#apidoc.element.cash.vorpal.lodash.unset)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unzip (array)](#apidoc.element.cash.vorpal.lodash.unzip)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unzipWith (array, iteratee)](#apidoc.element.cash.vorpal.lodash.unzipWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>update (object, path, updater)](#apidoc.element.cash.vorpal.lodash.update)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>updateWith (object, path, updater, customizer)](#apidoc.element.cash.vorpal.lodash.updateWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>upperCase (string)](#apidoc.element.cash.vorpal.lodash.upperCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>upperFirst (string)](#apidoc.element.cash.vorpal.lodash.upperFirst)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>values (object)](#apidoc.element.cash.vorpal.lodash.values)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>valuesIn (object)](#apidoc.element.cash.vorpal.lodash.valuesIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>without (array, values)](#apidoc.element.cash.vorpal.lodash.without)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>words (string, pattern, guard)](#apidoc.element.cash.vorpal.lodash.words)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>wrap (value, wrapper)](#apidoc.element.cash.vorpal.lodash.wrap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>xor (arrays)](#apidoc.element.cash.vorpal.lodash.xor)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>xorBy (arrays)](#apidoc.element.cash.vorpal.lodash.xorBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>xorWith (arrays)](#apidoc.element.cash.vorpal.lodash.xorWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zip (array)](#apidoc.element.cash.vorpal.lodash.zip)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zipObject (props, values)](#apidoc.element.cash.vorpal.lodash.zipObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zipObjectDeep (props, values)](#apidoc.element.cash.vorpal.lodash.zipObjectDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zipWith (arrays)](#apidoc.element.cash.vorpal.lodash.zipWith)
1.  object <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>templateSettings
1.  string <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>VERSION

#### [module cash.vorpal.lodash.prototype](#apidoc.module.cash.vorpal.lodash.prototype)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>add ()](#apidoc.element.cash.vorpal.lodash.prototype.add)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>after ()](#apidoc.element.cash.vorpal.lodash.prototype.after)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>ary ()](#apidoc.element.cash.vorpal.lodash.prototype.ary)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assign ()](#apidoc.element.cash.vorpal.lodash.prototype.assign)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assignIn ()](#apidoc.element.cash.vorpal.lodash.prototype.assignIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assignInWith ()](#apidoc.element.cash.vorpal.lodash.prototype.assignInWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assignWith ()](#apidoc.element.cash.vorpal.lodash.prototype.assignWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>at (paths)](#apidoc.element.cash.vorpal.lodash.prototype.at)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>attempt ()](#apidoc.element.cash.vorpal.lodash.prototype.attempt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>before ()](#apidoc.element.cash.vorpal.lodash.prototype.before)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>bind ()](#apidoc.element.cash.vorpal.lodash.prototype.bind)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>bindAll ()](#apidoc.element.cash.vorpal.lodash.prototype.bindAll)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>bindKey ()](#apidoc.element.cash.vorpal.lodash.prototype.bindKey)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>camelCase ()](#apidoc.element.cash.vorpal.lodash.prototype.camelCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>capitalize ()](#apidoc.element.cash.vorpal.lodash.prototype.capitalize)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>castArray ()](#apidoc.element.cash.vorpal.lodash.prototype.castArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>ceil ()](#apidoc.element.cash.vorpal.lodash.prototype.ceil)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>chain ()](#apidoc.element.cash.vorpal.lodash.prototype.chain)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>chunk ()](#apidoc.element.cash.vorpal.lodash.prototype.chunk)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>clamp ()](#apidoc.element.cash.vorpal.lodash.prototype.clamp)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>clone ()](#apidoc.element.cash.vorpal.lodash.prototype.clone)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cloneDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.cloneDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cloneDeepWith ()](#apidoc.element.cash.vorpal.lodash.prototype.cloneDeepWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cloneWith ()](#apidoc.element.cash.vorpal.lodash.prototype.cloneWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>commit ()](#apidoc.element.cash.vorpal.lodash.prototype.commit)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>compact ()](#apidoc.element.cash.vorpal.lodash.prototype.compact)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>concat ()](#apidoc.element.cash.vorpal.lodash.prototype.concat)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cond ()](#apidoc.element.cash.vorpal.lodash.prototype.cond)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>conforms ()](#apidoc.element.cash.vorpal.lodash.prototype.conforms)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>conformsTo ()](#apidoc.element.cash.vorpal.lodash.prototype.conformsTo)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>constant ()](#apidoc.element.cash.vorpal.lodash.prototype.constant)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>countBy ()](#apidoc.element.cash.vorpal.lodash.prototype.countBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>create ()](#apidoc.element.cash.vorpal.lodash.prototype.create)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>curry ()](#apidoc.element.cash.vorpal.lodash.prototype.curry)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>curryRight ()](#apidoc.element.cash.vorpal.lodash.prototype.curryRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>debounce ()](#apidoc.element.cash.vorpal.lodash.prototype.debounce)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>deburr ()](#apidoc.element.cash.vorpal.lodash.prototype.deburr)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defaultTo ()](#apidoc.element.cash.vorpal.lodash.prototype.defaultTo)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defaults ()](#apidoc.element.cash.vorpal.lodash.prototype.defaults)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defaultsDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.defaultsDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defer ()](#apidoc.element.cash.vorpal.lodash.prototype.defer)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>delay ()](#apidoc.element.cash.vorpal.lodash.prototype.delay)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>difference ()](#apidoc.element.cash.vorpal.lodash.prototype.difference)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>differenceBy ()](#apidoc.element.cash.vorpal.lodash.prototype.differenceBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>differenceWith ()](#apidoc.element.cash.vorpal.lodash.prototype.differenceWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>divide ()](#apidoc.element.cash.vorpal.lodash.prototype.divide)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>drop ()](#apidoc.element.cash.vorpal.lodash.prototype.drop)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>dropRight ()](#apidoc.element.cash.vorpal.lodash.prototype.dropRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>dropRightWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.dropRightWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>dropWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.dropWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>each ()](#apidoc.element.cash.vorpal.lodash.prototype.each)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>eachRight ()](#apidoc.element.cash.vorpal.lodash.prototype.eachRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>endsWith ()](#apidoc.element.cash.vorpal.lodash.prototype.endsWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>entries ()](#apidoc.element.cash.vorpal.lodash.prototype.entries)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>entriesIn ()](#apidoc.element.cash.vorpal.lodash.prototype.entriesIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>eq ()](#apidoc.element.cash.vorpal.lodash.prototype.eq)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>escape ()](#apidoc.element.cash.vorpal.lodash.prototype.escape)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>escapeRegExp ()](#apidoc.element.cash.vorpal.lodash.prototype.escapeRegExp)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>every ()](#apidoc.element.cash.vorpal.lodash.prototype.every)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>extend ()](#apidoc.element.cash.vorpal.lodash.prototype.extend)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>extendWith ()](#apidoc.element.cash.vorpal.lodash.prototype.extendWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>fill ()](#apidoc.element.cash.vorpal.lodash.prototype.fill)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>filter ()](#apidoc.element.cash.vorpal.lodash.prototype.filter)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>find ()](#apidoc.element.cash.vorpal.lodash.prototype.find)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.findIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findKey ()](#apidoc.element.cash.vorpal.lodash.prototype.findKey)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findLast ()](#apidoc.element.cash.vorpal.lodash.prototype.findLast)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findLastIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.findLastIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findLastKey ()](#apidoc.element.cash.vorpal.lodash.prototype.findLastKey)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>first ()](#apidoc.element.cash.vorpal.lodash.prototype.first)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatMap ()](#apidoc.element.cash.vorpal.lodash.prototype.flatMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatMapDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.flatMapDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatMapDepth ()](#apidoc.element.cash.vorpal.lodash.prototype.flatMapDepth)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatten ()](#apidoc.element.cash.vorpal.lodash.prototype.flatten)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flattenDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.flattenDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flattenDepth ()](#apidoc.element.cash.vorpal.lodash.prototype.flattenDepth)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flip ()](#apidoc.element.cash.vorpal.lodash.prototype.flip)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>floor ()](#apidoc.element.cash.vorpal.lodash.prototype.floor)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flow ()](#apidoc.element.cash.vorpal.lodash.prototype.flow)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flowRight ()](#apidoc.element.cash.vorpal.lodash.prototype.flowRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forEach ()](#apidoc.element.cash.vorpal.lodash.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forEachRight ()](#apidoc.element.cash.vorpal.lodash.prototype.forEachRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forIn ()](#apidoc.element.cash.vorpal.lodash.prototype.forIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forInRight ()](#apidoc.element.cash.vorpal.lodash.prototype.forInRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forOwn ()](#apidoc.element.cash.vorpal.lodash.prototype.forOwn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forOwnRight ()](#apidoc.element.cash.vorpal.lodash.prototype.forOwnRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>fromPairs ()](#apidoc.element.cash.vorpal.lodash.prototype.fromPairs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>functions ()](#apidoc.element.cash.vorpal.lodash.prototype.functions)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>functionsIn ()](#apidoc.element.cash.vorpal.lodash.prototype.functionsIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>get ()](#apidoc.element.cash.vorpal.lodash.prototype.get)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>groupBy ()](#apidoc.element.cash.vorpal.lodash.prototype.groupBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>gt ()](#apidoc.element.cash.vorpal.lodash.prototype.gt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>gte ()](#apidoc.element.cash.vorpal.lodash.prototype.gte)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>has ()](#apidoc.element.cash.vorpal.lodash.prototype.has)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>hasIn ()](#apidoc.element.cash.vorpal.lodash.prototype.hasIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>head ()](#apidoc.element.cash.vorpal.lodash.prototype.head)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>identity ()](#apidoc.element.cash.vorpal.lodash.prototype.identity)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>inRange ()](#apidoc.element.cash.vorpal.lodash.prototype.inRange)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>includes ()](#apidoc.element.cash.vorpal.lodash.prototype.includes)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>indexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>initial ()](#apidoc.element.cash.vorpal.lodash.prototype.initial)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>intersection ()](#apidoc.element.cash.vorpal.lodash.prototype.intersection)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>intersectionBy ()](#apidoc.element.cash.vorpal.lodash.prototype.intersectionBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>intersectionWith ()](#apidoc.element.cash.vorpal.lodash.prototype.intersectionWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invert ()](#apidoc.element.cash.vorpal.lodash.prototype.invert)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invertBy ()](#apidoc.element.cash.vorpal.lodash.prototype.invertBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invoke ()](#apidoc.element.cash.vorpal.lodash.prototype.invoke)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invokeMap ()](#apidoc.element.cash.vorpal.lodash.prototype.invokeMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArguments ()](#apidoc.element.cash.vorpal.lodash.prototype.isArguments)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArray ()](#apidoc.element.cash.vorpal.lodash.prototype.isArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArrayBuffer ()](#apidoc.element.cash.vorpal.lodash.prototype.isArrayBuffer)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArrayLike ()](#apidoc.element.cash.vorpal.lodash.prototype.isArrayLike)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArrayLikeObject ()](#apidoc.element.cash.vorpal.lodash.prototype.isArrayLikeObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isBoolean ()](#apidoc.element.cash.vorpal.lodash.prototype.isBoolean)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isBuffer ()](#apidoc.element.cash.vorpal.lodash.prototype.isBuffer)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isDate ()](#apidoc.element.cash.vorpal.lodash.prototype.isDate)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isElement ()](#apidoc.element.cash.vorpal.lodash.prototype.isElement)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isEmpty ()](#apidoc.element.cash.vorpal.lodash.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isEqual ()](#apidoc.element.cash.vorpal.lodash.prototype.isEqual)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isEqualWith ()](#apidoc.element.cash.vorpal.lodash.prototype.isEqualWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isError ()](#apidoc.element.cash.vorpal.lodash.prototype.isError)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isFinite ()](#apidoc.element.cash.vorpal.lodash.prototype.isFinite)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isFunction ()](#apidoc.element.cash.vorpal.lodash.prototype.isFunction)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.isInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isLength ()](#apidoc.element.cash.vorpal.lodash.prototype.isLength)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isMap ()](#apidoc.element.cash.vorpal.lodash.prototype.isMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isMatch ()](#apidoc.element.cash.vorpal.lodash.prototype.isMatch)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isMatchWith ()](#apidoc.element.cash.vorpal.lodash.prototype.isMatchWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNaN ()](#apidoc.element.cash.vorpal.lodash.prototype.isNaN)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNative ()](#apidoc.element.cash.vorpal.lodash.prototype.isNative)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNil ()](#apidoc.element.cash.vorpal.lodash.prototype.isNil)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNull ()](#apidoc.element.cash.vorpal.lodash.prototype.isNull)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNumber ()](#apidoc.element.cash.vorpal.lodash.prototype.isNumber)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isObject ()](#apidoc.element.cash.vorpal.lodash.prototype.isObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isObjectLike ()](#apidoc.element.cash.vorpal.lodash.prototype.isObjectLike)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isPlainObject ()](#apidoc.element.cash.vorpal.lodash.prototype.isPlainObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isRegExp ()](#apidoc.element.cash.vorpal.lodash.prototype.isRegExp)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isSafeInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.isSafeInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isSet ()](#apidoc.element.cash.vorpal.lodash.prototype.isSet)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isString ()](#apidoc.element.cash.vorpal.lodash.prototype.isString)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isSymbol ()](#apidoc.element.cash.vorpal.lodash.prototype.isSymbol)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isTypedArray ()](#apidoc.element.cash.vorpal.lodash.prototype.isTypedArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isUndefined ()](#apidoc.element.cash.vorpal.lodash.prototype.isUndefined)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isWeakMap ()](#apidoc.element.cash.vorpal.lodash.prototype.isWeakMap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isWeakSet ()](#apidoc.element.cash.vorpal.lodash.prototype.isWeakSet)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>iteratee ()](#apidoc.element.cash.vorpal.lodash.prototype.iteratee)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>join ()](#apidoc.element.cash.vorpal.lodash.prototype.join)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>kebabCase ()](#apidoc.element.cash.vorpal.lodash.prototype.kebabCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>keyBy ()](#apidoc.element.cash.vorpal.lodash.prototype.keyBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>keys ()](#apidoc.element.cash.vorpal.lodash.prototype.keys)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>keysIn ()](#apidoc.element.cash.vorpal.lodash.prototype.keysIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>last ()](#apidoc.element.cash.vorpal.lodash.prototype.last)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lastIndexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lowerCase ()](#apidoc.element.cash.vorpal.lodash.prototype.lowerCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lowerFirst ()](#apidoc.element.cash.vorpal.lodash.prototype.lowerFirst)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lt ()](#apidoc.element.cash.vorpal.lodash.prototype.lt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lte ()](#apidoc.element.cash.vorpal.lodash.prototype.lte)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>map ()](#apidoc.element.cash.vorpal.lodash.prototype.map)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mapKeys ()](#apidoc.element.cash.vorpal.lodash.prototype.mapKeys)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mapValues ()](#apidoc.element.cash.vorpal.lodash.prototype.mapValues)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>matches ()](#apidoc.element.cash.vorpal.lodash.prototype.matches)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>matchesProperty ()](#apidoc.element.cash.vorpal.lodash.prototype.matchesProperty)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>max ()](#apidoc.element.cash.vorpal.lodash.prototype.max)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>maxBy ()](#apidoc.element.cash.vorpal.lodash.prototype.maxBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mean ()](#apidoc.element.cash.vorpal.lodash.prototype.mean)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>meanBy ()](#apidoc.element.cash.vorpal.lodash.prototype.meanBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>memoize ()](#apidoc.element.cash.vorpal.lodash.prototype.memoize)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>merge ()](#apidoc.element.cash.vorpal.lodash.prototype.merge)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mergeWith ()](#apidoc.element.cash.vorpal.lodash.prototype.mergeWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>method ()](#apidoc.element.cash.vorpal.lodash.prototype.method)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>methodOf ()](#apidoc.element.cash.vorpal.lodash.prototype.methodOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>min ()](#apidoc.element.cash.vorpal.lodash.prototype.min)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>minBy ()](#apidoc.element.cash.vorpal.lodash.prototype.minBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mixin ()](#apidoc.element.cash.vorpal.lodash.prototype.mixin)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>multiply ()](#apidoc.element.cash.vorpal.lodash.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>negate ()](#apidoc.element.cash.vorpal.lodash.prototype.negate)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>next ()](#apidoc.element.cash.vorpal.lodash.prototype.next)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>noConflict ()](#apidoc.element.cash.vorpal.lodash.prototype.noConflict)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>noop ()](#apidoc.element.cash.vorpal.lodash.prototype.noop)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>now ()](#apidoc.element.cash.vorpal.lodash.prototype.now)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>nth ()](#apidoc.element.cash.vorpal.lodash.prototype.nth)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>nthArg ()](#apidoc.element.cash.vorpal.lodash.prototype.nthArg)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>omit ()](#apidoc.element.cash.vorpal.lodash.prototype.omit)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>omitBy ()](#apidoc.element.cash.vorpal.lodash.prototype.omitBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>once ()](#apidoc.element.cash.vorpal.lodash.prototype.once)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>orderBy ()](#apidoc.element.cash.vorpal.lodash.prototype.orderBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>over ()](#apidoc.element.cash.vorpal.lodash.prototype.over)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>overArgs ()](#apidoc.element.cash.vorpal.lodash.prototype.overArgs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>overEvery ()](#apidoc.element.cash.vorpal.lodash.prototype.overEvery)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>overSome ()](#apidoc.element.cash.vorpal.lodash.prototype.overSome)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pad ()](#apidoc.element.cash.vorpal.lodash.prototype.pad)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>padEnd ()](#apidoc.element.cash.vorpal.lodash.prototype.padEnd)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>padStart ()](#apidoc.element.cash.vorpal.lodash.prototype.padStart)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>parseInt ()](#apidoc.element.cash.vorpal.lodash.prototype.parseInt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>partial ()](#apidoc.element.cash.vorpal.lodash.prototype.partial)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>partialRight ()](#apidoc.element.cash.vorpal.lodash.prototype.partialRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>partition ()](#apidoc.element.cash.vorpal.lodash.prototype.partition)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pick ()](#apidoc.element.cash.vorpal.lodash.prototype.pick)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pickBy ()](#apidoc.element.cash.vorpal.lodash.prototype.pickBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>plant (value)](#apidoc.element.cash.vorpal.lodash.prototype.plant)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pop ()](#apidoc.element.cash.vorpal.lodash.prototype.pop)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>property ()](#apidoc.element.cash.vorpal.lodash.prototype.property)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>propertyOf ()](#apidoc.element.cash.vorpal.lodash.prototype.propertyOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pull ()](#apidoc.element.cash.vorpal.lodash.prototype.pull)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAll ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAll)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAllBy ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAllBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAllWith ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAllWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAt ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAt)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>push ()](#apidoc.element.cash.vorpal.lodash.prototype.push)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>random ()](#apidoc.element.cash.vorpal.lodash.prototype.random)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>range ()](#apidoc.element.cash.vorpal.lodash.prototype.range)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>rangeRight ()](#apidoc.element.cash.vorpal.lodash.prototype.rangeRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>rearg ()](#apidoc.element.cash.vorpal.lodash.prototype.rearg)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reduce ()](#apidoc.element.cash.vorpal.lodash.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reduceRight ()](#apidoc.element.cash.vorpal.lodash.prototype.reduceRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reject ()](#apidoc.element.cash.vorpal.lodash.prototype.reject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>remove ()](#apidoc.element.cash.vorpal.lodash.prototype.remove)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>repeat ()](#apidoc.element.cash.vorpal.lodash.prototype.repeat)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>replace ()](#apidoc.element.cash.vorpal.lodash.prototype.replace)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>rest ()](#apidoc.element.cash.vorpal.lodash.prototype.rest)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>result ()](#apidoc.element.cash.vorpal.lodash.prototype.result)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reverse ()](#apidoc.element.cash.vorpal.lodash.prototype.reverse)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>round ()](#apidoc.element.cash.vorpal.lodash.prototype.round)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>runInContext ()](#apidoc.element.cash.vorpal.lodash.prototype.runInContext)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sample ()](#apidoc.element.cash.vorpal.lodash.prototype.sample)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sampleSize ()](#apidoc.element.cash.vorpal.lodash.prototype.sampleSize)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>set ()](#apidoc.element.cash.vorpal.lodash.prototype.set)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>setWith ()](#apidoc.element.cash.vorpal.lodash.prototype.setWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>shift ()](#apidoc.element.cash.vorpal.lodash.prototype.shift)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>shuffle ()](#apidoc.element.cash.vorpal.lodash.prototype.shuffle)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>size ()](#apidoc.element.cash.vorpal.lodash.prototype.size)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>slice ()](#apidoc.element.cash.vorpal.lodash.prototype.slice)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>snakeCase ()](#apidoc.element.cash.vorpal.lodash.prototype.snakeCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>some ()](#apidoc.element.cash.vorpal.lodash.prototype.some)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sort ()](#apidoc.element.cash.vorpal.lodash.prototype.sort)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedIndexBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedIndexBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedIndexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedIndexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedLastIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndex)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedLastIndexBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndexBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedLastIndexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndexOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedUniq ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedUniq)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedUniqBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedUniqBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>splice ()](#apidoc.element.cash.vorpal.lodash.prototype.splice)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>split ()](#apidoc.element.cash.vorpal.lodash.prototype.split)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>spread ()](#apidoc.element.cash.vorpal.lodash.prototype.spread)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>startCase ()](#apidoc.element.cash.vorpal.lodash.prototype.startCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>startsWith ()](#apidoc.element.cash.vorpal.lodash.prototype.startsWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubArray ()](#apidoc.element.cash.vorpal.lodash.prototype.stubArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubFalse ()](#apidoc.element.cash.vorpal.lodash.prototype.stubFalse)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubObject ()](#apidoc.element.cash.vorpal.lodash.prototype.stubObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubString ()](#apidoc.element.cash.vorpal.lodash.prototype.stubString)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubTrue ()](#apidoc.element.cash.vorpal.lodash.prototype.stubTrue)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>subtract ()](#apidoc.element.cash.vorpal.lodash.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sum ()](#apidoc.element.cash.vorpal.lodash.prototype.sum)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sumBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sumBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>tail ()](#apidoc.element.cash.vorpal.lodash.prototype.tail)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>take ()](#apidoc.element.cash.vorpal.lodash.prototype.take)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>takeRight ()](#apidoc.element.cash.vorpal.lodash.prototype.takeRight)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>takeRightWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.takeRightWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>takeWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.takeWhile)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>tap ()](#apidoc.element.cash.vorpal.lodash.prototype.tap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>template ()](#apidoc.element.cash.vorpal.lodash.prototype.template)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>throttle ()](#apidoc.element.cash.vorpal.lodash.prototype.throttle)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>thru ()](#apidoc.element.cash.vorpal.lodash.prototype.thru)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>times ()](#apidoc.element.cash.vorpal.lodash.prototype.times)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toArray ()](#apidoc.element.cash.vorpal.lodash.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toFinite ()](#apidoc.element.cash.vorpal.lodash.prototype.toFinite)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.toInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toJSON ()](#apidoc.element.cash.vorpal.lodash.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toLength ()](#apidoc.element.cash.vorpal.lodash.prototype.toLength)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toLower ()](#apidoc.element.cash.vorpal.lodash.prototype.toLower)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toNumber ()](#apidoc.element.cash.vorpal.lodash.prototype.toNumber)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPairs ()](#apidoc.element.cash.vorpal.lodash.prototype.toPairs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPairsIn ()](#apidoc.element.cash.vorpal.lodash.prototype.toPairsIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPath ()](#apidoc.element.cash.vorpal.lodash.prototype.toPath)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPlainObject ()](#apidoc.element.cash.vorpal.lodash.prototype.toPlainObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toSafeInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.toSafeInteger)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toString ()](#apidoc.element.cash.vorpal.lodash.prototype.toString)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toUpper ()](#apidoc.element.cash.vorpal.lodash.prototype.toUpper)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>transform ()](#apidoc.element.cash.vorpal.lodash.prototype.transform)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>trim ()](#apidoc.element.cash.vorpal.lodash.prototype.trim)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>trimEnd ()](#apidoc.element.cash.vorpal.lodash.prototype.trimEnd)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>trimStart ()](#apidoc.element.cash.vorpal.lodash.prototype.trimStart)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>truncate ()](#apidoc.element.cash.vorpal.lodash.prototype.truncate)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unary ()](#apidoc.element.cash.vorpal.lodash.prototype.unary)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unescape ()](#apidoc.element.cash.vorpal.lodash.prototype.unescape)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>union ()](#apidoc.element.cash.vorpal.lodash.prototype.union)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unionBy ()](#apidoc.element.cash.vorpal.lodash.prototype.unionBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unionWith ()](#apidoc.element.cash.vorpal.lodash.prototype.unionWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniq ()](#apidoc.element.cash.vorpal.lodash.prototype.uniq)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniqBy ()](#apidoc.element.cash.vorpal.lodash.prototype.uniqBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniqWith ()](#apidoc.element.cash.vorpal.lodash.prototype.uniqWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniqueId ()](#apidoc.element.cash.vorpal.lodash.prototype.uniqueId)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unset ()](#apidoc.element.cash.vorpal.lodash.prototype.unset)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unshift ()](#apidoc.element.cash.vorpal.lodash.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unzip ()](#apidoc.element.cash.vorpal.lodash.prototype.unzip)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unzipWith ()](#apidoc.element.cash.vorpal.lodash.prototype.unzipWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>update ()](#apidoc.element.cash.vorpal.lodash.prototype.update)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>updateWith ()](#apidoc.element.cash.vorpal.lodash.prototype.updateWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>upperCase ()](#apidoc.element.cash.vorpal.lodash.prototype.upperCase)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>upperFirst ()](#apidoc.element.cash.vorpal.lodash.prototype.upperFirst)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>value ()](#apidoc.element.cash.vorpal.lodash.prototype.value)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>valueOf ()](#apidoc.element.cash.vorpal.lodash.prototype.valueOf)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>values ()](#apidoc.element.cash.vorpal.lodash.prototype.values)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>valuesIn ()](#apidoc.element.cash.vorpal.lodash.prototype.valuesIn)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>without ()](#apidoc.element.cash.vorpal.lodash.prototype.without)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>words ()](#apidoc.element.cash.vorpal.lodash.prototype.words)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>wrap ()](#apidoc.element.cash.vorpal.lodash.prototype.wrap)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>xor ()](#apidoc.element.cash.vorpal.lodash.prototype.xor)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>xorBy ()](#apidoc.element.cash.vorpal.lodash.prototype.xorBy)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>xorWith ()](#apidoc.element.cash.vorpal.lodash.prototype.xorWith)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zip ()](#apidoc.element.cash.vorpal.lodash.prototype.zip)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zipObject ()](#apidoc.element.cash.vorpal.lodash.prototype.zipObject)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zipObjectDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.zipObjectDeep)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zipWith ()](#apidoc.element.cash.vorpal.lodash.prototype.zipWith)

#### [module cash.vorpal.ui](#apidoc.module.cash.vorpal.ui)
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_cancelled
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_midPrompt
1.  boolean <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_sigintCalled
1.  [function <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_sigint ()](#apidoc.element.cash.vorpal.ui._sigint)
1.  number <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_eventsCount
1.  number <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_sigintCount
1.  object <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_events
1.  object <span class="apidocSignatureSpan">cash.vorpal.ui.</span>domain
1.  object <span class="apidocSignatureSpan">cash.vorpal.ui.</span>inquirer
1.  object <span class="apidocSignatureSpan">cash.vorpal.ui.</span>inquirerStdout

#### [module cash.vorpal.util](#apidoc.module.cash.vorpal.util)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>buildCommandArgs (passedArgs, cmd, execCommand, isCommandArgKeyPairNormalized)](#apidoc.element.cash.vorpal.util.buildCommandArgs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>fixArgsForApply (obj)](#apidoc.element.cash.vorpal.util.fixArgsForApply)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>humanReadableArgName (arg)](#apidoc.element.cash.vorpal.util.humanReadableArgName)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>matchCommand (cmd, cmds)](#apidoc.element.cash.vorpal.util.matchCommand)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>pad (str, width, delimiter)](#apidoc.element.cash.vorpal.util.pad)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>parseArgs (str, opts)](#apidoc.element.cash.vorpal.util.parseArgs)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>parseCommand (command, commands)](#apidoc.element.cash.vorpal.util.parseCommand)
1.  [function <span class="apidocSignatureSpan">cash.vorpal.util.</span>prettifyArray (arr)](#apidoc.element.cash.vorpal.util.prettifyArray)



# <a name="apidoc.module.cash"></a>[module cash](#apidoc.module.cash)

#### <a name="apidoc.element.cash.alias"></a>[function <span class="apidocSignatureSpan">cash.</span>alias (args, options, callback)](#apidoc.element.cash.alias)
- description and source-code
```javascript
alias = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.cat"></a>[function <span class="apidocSignatureSpan">cash.</span>cat (args, options, callback)](#apidoc.element.cash.cat)
- description and source-code
```javascript
cat = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.cd"></a>[function <span class="apidocSignatureSpan">cash.</span>cd (args, options, callback)](#apidoc.element.cash.cd)
- description and source-code
```javascript
cd = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.clear"></a>[function <span class="apidocSignatureSpan">cash.</span>clear (args, options, callback)](#apidoc.element.cash.clear)
- description and source-code
```javascript
clear = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.cp"></a>[function <span class="apidocSignatureSpan">cash.</span>cp (args, options, callback)](#apidoc.element.cash.cp)
- description and source-code
```javascript
cp = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.echo"></a>[function <span class="apidocSignatureSpan">cash.</span>echo (args, options, callback)](#apidoc.element.cash.echo)
- description and source-code
```javascript
echo = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.export"></a>[function <span class="apidocSignatureSpan">cash.</span>export (args, options, callback)](#apidoc.element.cash.export)
- description and source-code
```javascript
export = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.false"></a>[function <span class="apidocSignatureSpan">cash.</span>false (args, options, callback)](#apidoc.element.cash.false)
- description and source-code
```javascript
false = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.grep"></a>[function <span class="apidocSignatureSpan">cash.</span>grep (args, options, callback)](#apidoc.element.cash.grep)
- description and source-code
```javascript
grep = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.head"></a>[function <span class="apidocSignatureSpan">cash.</span>head (args, options, callback)](#apidoc.element.cash.head)
- description and source-code
```javascript
head = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.kill"></a>[function <span class="apidocSignatureSpan">cash.</span>kill (args, options, callback)](#apidoc.element.cash.kill)
- description and source-code
```javascript
kill = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.less"></a>[function <span class="apidocSignatureSpan">cash.</span>less (args, options, callback)](#apidoc.element.cash.less)
- description and source-code
```javascript
less = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.ls"></a>[function <span class="apidocSignatureSpan">cash.</span>ls (args, options, callback)](#apidoc.element.cash.ls)
- description and source-code
```javascript
ls = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
...

### Wow. But I want this programmatically!

Again, you're in business:

'''js
const $ = require('cash');
const out = $.ls('.', {l: true});
'''

Not terse enough? How about this:

'''js
const out = $('ls -lah');
'''
...
```

#### <a name="apidoc.element.cash.mkdir"></a>[function <span class="apidocSignatureSpan">cash.</span>mkdir (args, options, callback)](#apidoc.element.cash.mkdir)
- description and source-code
```javascript
mkdir = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.mv"></a>[function <span class="apidocSignatureSpan">cash.</span>mv (args, options, callback)](#apidoc.element.cash.mv)
- description and source-code
```javascript
mv = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.pwd"></a>[function <span class="apidocSignatureSpan">cash.</span>pwd (args, options, callback)](#apidoc.element.cash.pwd)
- description and source-code
```javascript
pwd = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.rm"></a>[function <span class="apidocSignatureSpan">cash.</span>rm (args, options, callback)](#apidoc.element.cash.rm)
- description and source-code
```javascript
rm = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.show"></a>[function <span class="apidocSignatureSpan">cash.</span>show ()](#apidoc.element.cash.show)
- description and source-code
```javascript
function show() {
<span class="apidocCodeCommentSpan">  /* istanbul ignore next */
</span>  app.vorpal.show();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.sort"></a>[function <span class="apidocSignatureSpan">cash.</span>sort (args, options, callback)](#apidoc.element.cash.sort)
- description and source-code
```javascript
sort = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.source"></a>[function <span class="apidocSignatureSpan">cash.</span>source (args, options, callback)](#apidoc.element.cash.source)
- description and source-code
```javascript
source = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.tail"></a>[function <span class="apidocSignatureSpan">cash.</span>tail (args, options, callback)](#apidoc.element.cash.tail)
- description and source-code
```javascript
tail = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.touch"></a>[function <span class="apidocSignatureSpan">cash.</span>touch (args, options, callback)](#apidoc.element.cash.touch)
- description and source-code
```javascript
touch = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.true"></a>[function <span class="apidocSignatureSpan">cash.</span>true (args, options, callback)](#apidoc.element.cash.true)
- description and source-code
```javascript
true = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.unalias"></a>[function <span class="apidocSignatureSpan">cash.</span>unalias (args, options, callback)](#apidoc.element.cash.unalias)
- description and source-code
```javascript
unalias = function (args, options, callback) {
  callback = callback || function () {};
  options = options || {};
  options.vorpal = app.vorpal;
  return interfacer.call(this, {
    command: app.vorpal.api[cmd],
    args: args,
    options: options,
    callback: callback,
    async: app.vorpal.api[cmd].async || false,
    silent: true
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session"></a>[function <span class="apidocSignatureSpan">cash.</span>vorpal.Session (options)](#apidoc.element.cash.vorpal.Session)
- description and source-code
```javascript
function Session(options) {
  options = options || {};
  this.id = options.id || this._guid();
  this.parent = options.parent || undefined;
  this.authenticating = options.authenticating || false;
  this.authenticated = options.authenticated || undefined;
  this.user = options.user || 'guest';
  this.host = options.host;
  this.address = options.address || undefined;
  this._isLocal = options.local || undefined;
  this._delimiter = options.delimiter || String(os.hostname()).split('.')[0] + '~$';
  this._modeDelimiter = undefined;

  // Keeps history of how many times in a row 'tab' was
  // pressed on the keyboard.
  this._tabCtr = 0;

  this.cmdHistory = this.parent.cmdHistory;

  // Special command mode vorpal is in at the moment,
  // such as REPL. See mode documentation.
  this._mode = undefined;

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal"></a>[module cash.vorpal](#apidoc.module.cash.vorpal)

#### <a name="apidoc.element.cash.vorpal.Session"></a>[function <span class="apidocSignatureSpan">cash.vorpal.</span>Session (options)](#apidoc.element.cash.vorpal.Session)
- description and source-code
```javascript
function Session(options) {
  options = options || {};
  this.id = options.id || this._guid();
  this.parent = options.parent || undefined;
  this.authenticating = options.authenticating || false;
  this.authenticated = options.authenticated || undefined;
  this.user = options.user || 'guest';
  this.host = options.host;
  this.address = options.address || undefined;
  this._isLocal = options.local || undefined;
  this._delimiter = options.delimiter || String(os.hostname()).split('.')[0] + '~$';
  this._modeDelimiter = undefined;

  // Keeps history of how many times in a row 'tab' was
  // pressed on the keyboard.
  this._tabCtr = 0;

  this.cmdHistory = this.parent.cmdHistory;

  // Special command mode vorpal is in at the moment,
  // such as REPL. See mode documentation.
  this._mode = undefined;

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal._help"></a>[function <span class="apidocSignatureSpan">cash.vorpal.</span>_help ()](#apidoc.element.cash.vorpal._help)
- description and source-code
```javascript
_help = function () {
  var version = require('./../package.json').version;
  var result = '';

  result += 'Cash, version ' + version + '\n';
  result += 'These shell commands are defined internally.  Type 'help\' to see this list.\n';
  result += 'Type 'help name\' to find out more about the function 'name\'.\n';
  result += 'Use 'info cash\' to find out more about the shell in general.\n';
  result += '\n';

  var half = Math.floor(commands.length / 2);
  var width = Math.floor((process.stdout.columns - 3) / 2);
  var lhalf = Math.ceil(commands.length / 2);
  var padding = commands.length % 2 === 1 ? 1 : 0;
  for (var i = 0; i < lhalf; ++i) {
    var colA = pad(chop(commands[i], width), width);
    var colB = pad(chop(commands[half + i + padding] || '', width), width);
    var line = i === lhalf - 1 ? '' : '\n';
    result += ' ' + colA + ' ' + colB + line;
  }

  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.Session"></a>[module cash.vorpal.Session](#apidoc.module.cash.vorpal.Session)

#### <a name="apidoc.element.cash.vorpal.Session.Session"></a>[function <span class="apidocSignatureSpan">cash.vorpal.</span>Session (options)](#apidoc.element.cash.vorpal.Session.Session)
- description and source-code
```javascript
function Session(options) {
  options = options || {};
  this.id = options.id || this._guid();
  this.parent = options.parent || undefined;
  this.authenticating = options.authenticating || false;
  this.authenticated = options.authenticated || undefined;
  this.user = options.user || 'guest';
  this.host = options.host;
  this.address = options.address || undefined;
  this._isLocal = options.local || undefined;
  this._delimiter = options.delimiter || String(os.hostname()).split('.')[0] + '~$';
  this._modeDelimiter = undefined;

  // Keeps history of how many times in a row 'tab' was
  // pressed on the keyboard.
  this._tabCtr = 0;

  this.cmdHistory = this.parent.cmdHistory;

  // Special command mode vorpal is in at the moment,
  // such as REPL. See mode documentation.
  this._mode = undefined;

  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.Session.prototype"></a>[module cash.vorpal.Session.prototype](#apidoc.module.cash.vorpal.Session.prototype)

#### <a name="apidoc.element.cash.vorpal.Session.prototype._autocomplete"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>_autocomplete (str, arr)](#apidoc.element.cash.vorpal.Session.prototype._autocomplete)
- description and source-code
```javascript
_autocomplete = function (str, arr) {
  return autocomplete.match.call(this, str, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype._guid"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>_guid ()](#apidoc.element.cash.vorpal.Session.prototype._guid)
- description and source-code
```javascript
_guid = function () {
  function s4() {
    return Math.floor((1 + Math.random()) * 0x10000).toString(16).substring(1);
  }
  return s4() + s4() + '-' + s4() + '-' + s4() + '-' + s4() + '-' + s4() + s4() + s4();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype._log"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>_log ()](#apidoc.element.cash.vorpal.Session.prototype._log)
- description and source-code
```javascript
_log = function () {
  var self = this;
  if (this.isLocal()) {
    this.parent.ui.log.apply(this.parent.ui, arguments);
  } else {
    // If it's an error, expose the stack. Otherwise
    // we get a helpful '{}'.
    var args = [];
    for (var i = 0; i < arguments.length; ++i) {
      var str = arguments[i];
      str = str && str.stack ? 'Error: ' + str.message : str;
      args.push(str);
    }
    self.parent._send('vantage-ssn-stdout-downstream', 'downstream', { sessionId: self.id, value: args });
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.completeCommand"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>completeCommand ()](#apidoc.element.cash.vorpal.Session.prototype.completeCommand)
- description and source-code
```javascript
completeCommand = function () {
  this._completedCommands++;
  if (this._registeredCommands <= this._completedCommands) {
    this._registeredCommands = 0;
    this._completedCommands = 0;
    if (this._commandSetCallback) {
      this._commandSetCallback();
    }
    this._commandSetCallback = undefined;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.delimiter"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>delimiter (str)](#apidoc.element.cash.vorpal.Session.prototype.delimiter)
- description and source-code
```javascript
delimiter = function (str) {
  if (str === undefined) {
    return this._delimiter;
  }
  this._delimiter = String(str).trim() + ' ';
  if (this.isLocal()) {
    this.parent.ui.refresh();
  } else {
    this.parent._send('vantage-delimiter-downstream', 'downstream', { value: str, sessionId: this.id });
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.execCommandSet"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>execCommandSet (wrapper, callback)](#apidoc.element.cash.vorpal.Session.prototype.execCommandSet)
- description and source-code
```javascript
execCommandSet = function (wrapper, callback) {
  var self = this;
  var response = {};
  var res;
  var cbk = callback;
  this._registeredCommands = 1;
  this._completedCommands = 0;

  // Create the command instance for the first
  // command and hook it up to the pipe chain.
  var commandInstance = new CommandInstance({
    downstream: wrapper.pipes[0],
    commandObject: wrapper.commandObject,
    commandWrapper: wrapper
  });

  wrapper.commandInstance = commandInstance;

  function sendDones(itm) {
    if (itm.commandObject && itm.commandObject._done) {
      itm.commandObject._done.call(itm);
    }
    if (itm.downstream) {
      sendDones(itm.downstream);
    }
  }

  // Called when command is cancelled
  this.cancelCommands = function () {
    var callCancel = function callCancel(commandInstance) {
      if (_.isFunction(commandInstance.commandObject._cancel)) {
        commandInstance.commandObject._cancel.call(commandInstance);
      }

      if (commandInstance.downstream) {
        callCancel(commandInstance.downstream);
      }
    };

    callCancel(wrapper.commandInstance);

    // Check if there is a cancel method on the promise
    if (res && _.isFunction(res.cancel)) {
      res.cancel(wrapper.commandInstance);
    }

    self.removeListener('vorpal_command_cancel', self.cancelCommands);
    self.cancelCommands = undefined;
    self._commandSetCallback = undefined;
    self._registeredCommands = 0;
    self._completedCommands = 0;
    self.parent.emit('client_command_cancelled', { command: wrapper.command });

    cbk(wrapper);
  };

  this.on('vorpal_command_cancel', self.cancelCommands);

  // Gracefully handles all instances of the command completing.
  this._commandSetCallback = function () {
    var err = response.error;
    var data = response.data;
    var argus = response.args;
    if (self.isLocal() && err) {
      var stack;
      if (data && data.stack) {
        stack = data.stack;
      } else if (err && err.stack) {
        stack = err.stack;
      } else {
        stack = err;
      }
      self.log(stack);
      self.parent.emit('client_command_error', { command: wrapper.command, error: err });
    } else if (self.isLocal()) {
      self.parent.emit('client_command_executed', { command: wrapper.command });
    }

    self.removeListener('vorpal_command_cancel', self.cancelCommands);
    self.cancelCommands = undefined;
    cbk(wrapper, err, data, argus);
    sendDones(commandInstance);
  };

  function onCompletion(wrapper, err, data, argus) {
    response = {
      error: err,
      data: data,
      args: argus
    };
    self.completeCommand();
  }

  var valid;
  if (_.isFunction(wrapper.validate)) {
    try {
      valid = wrapper.validate.call(commandInstance, wrapper.args);
    } catch (e) {
      // Complete with error on validation error
      onCompletion(wrapper, e);
      return this;
    }
  }

  if (valid !== true && valid !== undefined) {
    onCompletion(wrapper, valid || null);
    return this;
  }

  // Call the root command.
  res = wrapper.fn.call(commandInstance, wrapper.args, function () {
    var argus = util.fixArgsForApply(arguments);
    onCompletion(wrapper, argus[0], argus[1], argus);
  });

  // If the command as declared by the user
  // returns a promise, handle accordingly.
  if (res && _.isFunction(res.then)) {
    res.then(function (data) {
      onCompletion(wrapper, undefined, data);
    }).catch(function (err) {
      onCompletion(wrapper, true, err);
    });
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.fullDelimiter"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>fullDelimiter ()](#apidoc.element.cash.vorpal.Session.prototype.fullDelimiter)
- description and source-code
```javascript
fullDelimiter = function () {
  var result = this._delimiter + (this._modeDelimiter !== undefined ? this._modeDelimiter : '');
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.getAutocomplete"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getAutocomplete (str, cb)](#apidoc.element.cash.vorpal.Session.prototype.getAutocomplete)
- description and source-code
```javascript
getAutocomplete = function (str, cb) {
  return autocomplete.exec.call(this, str, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.getAutocompleteDeprecated"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getAutocompleteDeprecated (str, cb)](#apidoc.element.cash.vorpal.Session.prototype.getAutocompleteDeprecated)
- description and source-code
```javascript
getAutocompleteDeprecated = function (str, cb) {
  cb = cb || function () {};

  // Entire command string
  var cursor = this.parent.ui._activePrompt.screen.rl.cursor;
  var trimmed = String(str).trim();
  var cut = String(trimmed).slice(0, cursor);
  var remainder = String(trimmed).slice(cursor, trimmed.length).replace(/ +$/, '');
  trimmed = cut;

  // Set "trimmed" to command string after pipe
  // Set "pre" to command string, pipe, and a space
  var pre = '';
  var lastPipeIndex = trimmed.lastIndexOf('|');
  if (lastPipeIndex !== -1) {
    pre = trimmed.substr(0, lastPipeIndex + 1) + ' ';
    trimmed = trimmed.substr(lastPipeIndex + 1).trim();
  }

  // Complete command
  var names = _.map(this.parent.commands, '_name');
  names = names.concat.apply(names, _.map(this.parent.commands, '_aliases'));
  var result = this._autocomplete(trimmed, names);
  if (result && trimmed.length < String(result).trim().length) {
    cb(undefined, pre + result + remainder);
    return;
  }

  // Find custom autocompletion
  var match;
  var extra;

  names.forEach(function (name) {
    if (trimmed.substr(0, name.length) === name && String(name).trim() !== '') {
      match = name;
      extra = trimmed.substr(name.length).trim();
    }
  });

  var command = match ? _.find(this.parent.commands, { _name: match }) : undefined;

  if (!command) {
    command = _.find(this.parent.commands, { _catch: true });
    if (command) {
      extra = trimmed;
    }
  }

  if (command && _.isFunction(command._autocompletion)) {
    this._tabCtr++;
    command._autocompletion.call(this, extra, this._tabCtr, function (err, autocomplete) {
      if (err) {
        return cb(err);
      }
      if (_.isArray(autocomplete)) {
        return cb(undefined, autocomplete);
      } else if (autocomplete === undefined) {
        return cb(undefined, undefined);
      }
      return cb(undefined, pre + autocomplete + remainder);
    });
  } else {
    cb(undefined, undefined);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.getHistory"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getHistory (direction)](#apidoc.element.cash.vorpal.Session.prototype.getHistory)
- description and source-code
```javascript
getHistory = function (direction) {
  var history;
  if (direction === 'up') {
    history = this.cmdHistory.getPreviousHistory();
  } else if (direction === 'down') {
    history = this.cmdHistory.getNextHistory();
  }
  return history;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.getKeypressResult"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>getKeypressResult (key, value, cb)](#apidoc.element.cash.vorpal.Session.prototype.getKeypressResult)
- description and source-code
```javascript
getKeypressResult = function (key, value, cb) {
  cb = cb || function () {};
  var keyMatch = ['up', 'down', 'tab'].indexOf(key) > -1;
  if (key !== 'tab') {
    this._tabCtr = 0;
  }
  if (keyMatch) {
    if (['up', 'down'].indexOf(key) > -1) {
      cb(undefined, this.getHistory(key));
    } else if (key === 'tab') {
      // If the Vorpal user has any commands that use
      // command.autocompletion, defer to the deprecated
      // version of autocompletion. Otherwise, default
      // to the new version.
      var fn = this.parent._useDeprecatedAutocompletion ? 'getAutocompleteDeprecated' : 'getAutocomplete';
      this[fn](value, function (err, data) {
        cb(err, data);
      });
    }
  } else {
    this._histCtr = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.help"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>help (command)](#apidoc.element.cash.vorpal.Session.prototype.help)
- description and source-code
```javascript
help = function (command) {
  this.log(this.parent._commandHelp(command || ''));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.history"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>history (str)](#apidoc.element.cash.vorpal.Session.prototype.history)
- description and source-code
```javascript
history = function (str) {
  var exceptions = [];
  if (str && exceptions.indexOf(String(str).toLowerCase()) === -1) {
    this.cmdHistory.newCommand(str);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.isLocal"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>isLocal ()](#apidoc.element.cash.vorpal.Session.prototype.isLocal)
- description and source-code
```javascript
isLocal = function () {
  return this._isLocal;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.log"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>log ()](#apidoc.element.cash.vorpal.Session.prototype.log)
- description and source-code
```javascript
log = function () {
  var args = util.fixArgsForApply(arguments);
  return this._log.apply(this, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.match"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>match (str, arr)](#apidoc.element.cash.vorpal.Session.prototype.match)
- description and source-code
```javascript
match = function (str, arr) {
  return this._autocomplete(str, arr);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.modeDelimiter"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>modeDelimiter (str)](#apidoc.element.cash.vorpal.Session.prototype.modeDelimiter)
- description and source-code
```javascript
modeDelimiter = function (str) {
  var self = this;
  if (str === undefined) {
    return this._modeDelimiter;
  }
  if (!this.isLocal()) {
    self.parent._send('vantage-mode-delimiter-downstream', 'downstream', { value: str, sessionId: self.id });
  } else {
    if (str === false || str === 'false') {
      this._modeDelimiter = undefined;
    } else {
      this._modeDelimiter = String(str).trim() + ' ';
    }
    this.parent.ui.refresh();
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.prompt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>prompt (options, cb)](#apidoc.element.cash.vorpal.Session.prototype.prompt)
- description and source-code
```javascript
prompt = function (options, cb) {
  options = options || {};
  options.sessionId = this.id;
  return this.parent.prompt(options, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.Session.prototype.registerCommand"></a>[function <span class="apidocSignatureSpan">cash.vorpal.Session.prototype.</span>registerCommand ()](#apidoc.element.cash.vorpal.Session.prototype.registerCommand)
- description and source-code
```javascript
registerCommand = function () {
  this._registeredCommands = this._registeredCommands || 0;
  this._registeredCommands++;
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.chalk"></a>[module cash.vorpal.chalk](#apidoc.module.cash.vorpal.chalk)

#### <a name="apidoc.element.cash.vorpal.chalk.hasColor"></a>[function <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>hasColor ()](#apidoc.element.cash.vorpal.chalk.hasColor)
- description and source-code
```javascript
hasColor = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.chalk.stripColor"></a>[function <span class="apidocSignatureSpan">cash.vorpal.chalk.</span>stripColor (str)](#apidoc.element.cash.vorpal.chalk.stripColor)
- description and source-code
```javascript
stripColor = function (str) {
	return typeof str === 'string' ? str.replace(ansiRegex, '') : str;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.lodash"></a>[module cash.vorpal.lodash](#apidoc.module.cash.vorpal.lodash)

#### <a name="apidoc.element.cash.vorpal.lodash.add"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>add (value, other)](#apidoc.element.cash.vorpal.lodash.add)
- description and source-code
```javascript
add = function (value, other) {
  var result;
  if (value === undefined && other === undefined) {
    return defaultValue;
  }
  if (value !== undefined) {
    result = value;
  }
  if (other !== undefined) {
    if (result === undefined) {
      return other;
    }
    if (typeof value == 'string' || typeof other == 'string') {
      value = baseToString(value);
      other = baseToString(other);
    } else {
      value = baseToNumber(value);
      other = baseToNumber(other);
    }
    result = operator(value, other);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.after"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>after (n, func)](#apidoc.element.cash.vorpal.lodash.after)
- description and source-code
```javascript
function after(n, func) {
  if (typeof func != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  n = toInteger(n);
  return function() {
    if (--n < 1) {
      return func.apply(this, arguments);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.ary"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>ary (func, n, guard)](#apidoc.element.cash.vorpal.lodash.ary)
- description and source-code
```javascript
function ary(func, n, guard) {
  n = guard ? undefined : n;
  n = (func && n == null) ? func.length : n;
  return createWrap(func, WRAP_ARY_FLAG, undefined, undefined, undefined, undefined, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.assign"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assign (object, sources)](#apidoc.element.cash.vorpal.lodash.assign)
- description and source-code
```javascript
assign = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.assignIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assignIn (object, sources)](#apidoc.element.cash.vorpal.lodash.assignIn)
- description and source-code
```javascript
assignIn = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.assignInWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assignInWith (object, sources)](#apidoc.element.cash.vorpal.lodash.assignInWith)
- description and source-code
```javascript
assignInWith = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.assignWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>assignWith (object, sources)](#apidoc.element.cash.vorpal.lodash.assignWith)
- description and source-code
```javascript
assignWith = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.at"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>at (object, paths)](#apidoc.element.cash.vorpal.lodash.at)
- description and source-code
```javascript
function baseAt(object, paths) {
  var index = -1,
      length = paths.length,
      result = Array(length),
      skip = object == null;

  while (++index < length) {
    result[index] = skip ? undefined : get(object, paths[index]);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.attempt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>attempt (func, args)](#apidoc.element.cash.vorpal.lodash.attempt)
- description and source-code
```javascript
attempt = function (func, args) {
  try {
    return apply(func, undefined, args);
  } catch (e) {
    return isError(e) ? e : new Error(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.before"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>before (n, func)](#apidoc.element.cash.vorpal.lodash.before)
- description and source-code
```javascript
function before(n, func) {
  var result;
  if (typeof func != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  n = toInteger(n);
  return function() {
    if (--n > 0) {
      result = func.apply(this, arguments);
    }
    if (n <= 1) {
      func = undefined;
    }
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.bind"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>bind (func, thisArg, partials)](#apidoc.element.cash.vorpal.lodash.bind)
- description and source-code
```javascript
bind = function (func, thisArg, partials) {
  var bitmask = WRAP_BIND_FLAG;
  if (partials.length) {
    var holders = replaceHolders(partials, getHolder(bind));
    bitmask |= WRAP_PARTIAL_FLAG;
  }
  return createWrap(func, bitmask, thisArg, partials, holders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.bindAll"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>bindAll (object, methodNames)](#apidoc.element.cash.vorpal.lodash.bindAll)
- description and source-code
```javascript
bindAll = function (object, methodNames) {
  arrayEach(methodNames, function(key) {
    key = toKey(key);
    baseAssignValue(object, key, bind(object[key], object));
  });
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.bindKey"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>bindKey (object, key, partials)](#apidoc.element.cash.vorpal.lodash.bindKey)
- description and source-code
```javascript
bindKey = function (object, key, partials) {
  var bitmask = WRAP_BIND_FLAG | WRAP_BIND_KEY_FLAG;
  if (partials.length) {
    var holders = replaceHolders(partials, getHolder(bindKey));
    bitmask |= WRAP_PARTIAL_FLAG;
  }
  return createWrap(key, bitmask, object, partials, holders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.camelCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>camelCase (string)](#apidoc.element.cash.vorpal.lodash.camelCase)
- description and source-code
```javascript
camelCase = function (string) {
  return arrayReduce(words(deburr(string).replace(reApos, '')), callback, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.capitalize"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>capitalize (string)](#apidoc.element.cash.vorpal.lodash.capitalize)
- description and source-code
```javascript
function capitalize(string) {
  return upperFirst(toString(string).toLowerCase());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.castArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>castArray ()](#apidoc.element.cash.vorpal.lodash.castArray)
- description and source-code
```javascript
function castArray() {
  if (!arguments.length) {
    return [];
  }
  var value = arguments[0];
  return isArray(value) ? value : [value];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.ceil"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>ceil (number, precision)](#apidoc.element.cash.vorpal.lodash.ceil)
- description and source-code
```javascript
ceil = function (number, precision) {
  number = toNumber(number);
  precision = precision == null ? 0 : nativeMin(toInteger(precision), 292);
  if (precision) {
    // Shift with exponential notation to avoid floating-point issues.
    // See [MDN](https://mdn.io/round#Examples) for more details.
    var pair = (toString(number) + 'e').split('e'),
        value = func(pair[0] + 'e' + (+pair[1] + precision));

    pair = (toString(value) + 'e').split('e');
    return +(pair[0] + 'e' + (+pair[1] - precision));
  }
  return func(number);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.chain"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>chain (value)](#apidoc.element.cash.vorpal.lodash.chain)
- description and source-code
```javascript
function chain(value) {
  var result = lodash(value);
  result.__chain__ = true;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.chunk"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>chunk (array, size, guard)](#apidoc.element.cash.vorpal.lodash.chunk)
- description and source-code
```javascript
function chunk(array, size, guard) {
  if ((guard ? isIterateeCall(array, size, guard) : size === undefined)) {
    size = 1;
  } else {
    size = nativeMax(toInteger(size), 0);
  }
  var length = array == null ? 0 : array.length;
  if (!length || size < 1) {
    return [];
  }
  var index = 0,
      resIndex = 0,
      result = Array(nativeCeil(length / size));

  while (index < length) {
    result[resIndex++] = baseSlice(array, index, (index += size));
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.clamp"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>clamp (number, lower, upper)](#apidoc.element.cash.vorpal.lodash.clamp)
- description and source-code
```javascript
function clamp(number, lower, upper) {
  if (upper === undefined) {
    upper = lower;
    lower = undefined;
  }
  if (upper !== undefined) {
    upper = toNumber(upper);
    upper = upper === upper ? upper : 0;
  }
  if (lower !== undefined) {
    lower = toNumber(lower);
    lower = lower === lower ? lower : 0;
  }
  return baseClamp(toNumber(number), lower, upper);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.clone"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>clone (value)](#apidoc.element.cash.vorpal.lodash.clone)
- description and source-code
```javascript
function clone(value) {
  return baseClone(value, CLONE_SYMBOLS_FLAG);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.cloneDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cloneDeep (value)](#apidoc.element.cash.vorpal.lodash.cloneDeep)
- description and source-code
```javascript
function cloneDeep(value) {
  return baseClone(value, CLONE_DEEP_FLAG | CLONE_SYMBOLS_FLAG);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.cloneDeepWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cloneDeepWith (value, customizer)](#apidoc.element.cash.vorpal.lodash.cloneDeepWith)
- description and source-code
```javascript
function cloneDeepWith(value, customizer) {
  customizer = typeof customizer == 'function' ? customizer : undefined;
  return baseClone(value, CLONE_DEEP_FLAG | CLONE_SYMBOLS_FLAG, customizer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.cloneWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cloneWith (value, customizer)](#apidoc.element.cash.vorpal.lodash.cloneWith)
- description and source-code
```javascript
function cloneWith(value, customizer) {
  customizer = typeof customizer == 'function' ? customizer : undefined;
  return baseClone(value, CLONE_SYMBOLS_FLAG, customizer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.compact"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>compact (array)](#apidoc.element.cash.vorpal.lodash.compact)
- description and source-code
```javascript
function compact(array) {
  var index = -1,
      length = array == null ? 0 : array.length,
      resIndex = 0,
      result = [];

  while (++index < length) {
    var value = array[index];
    if (value) {
      result[resIndex++] = value;
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.concat"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>concat ()](#apidoc.element.cash.vorpal.lodash.concat)
- description and source-code
```javascript
function concat() {
  var length = arguments.length;
  if (!length) {
    return [];
  }
  var args = Array(length - 1),
      array = arguments[0],
      index = length;

  while (index--) {
    args[index - 1] = arguments[index];
  }
  return arrayPush(isArray(array) ? copyArray(array) : [array], baseFlatten(args, 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.cond"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>cond (pairs)](#apidoc.element.cash.vorpal.lodash.cond)
- description and source-code
```javascript
function cond(pairs) {
  var length = pairs == null ? 0 : pairs.length,
      toIteratee = getIteratee();

  pairs = !length ? [] : arrayMap(pairs, function(pair) {
    if (typeof pair[1] != 'function') {
      throw new TypeError(FUNC_ERROR_TEXT);
    }
    return [toIteratee(pair[0]), pair[1]];
  });

  return baseRest(function(args) {
    var index = -1;
    while (++index < length) {
      var pair = pairs[index];
      if (apply(pair[0], this, args)) {
        return apply(pair[1], this, args);
      }
    }
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.conforms"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>conforms (source)](#apidoc.element.cash.vorpal.lodash.conforms)
- description and source-code
```javascript
function conforms(source) {
  return baseConforms(baseClone(source, CLONE_DEEP_FLAG));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.conformsTo"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>conformsTo (object, source)](#apidoc.element.cash.vorpal.lodash.conformsTo)
- description and source-code
```javascript
function conformsTo(object, source) {
  return source == null || baseConformsTo(object, source, keys(source));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.constant"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>constant (value)](#apidoc.element.cash.vorpal.lodash.constant)
- description and source-code
```javascript
function constant(value) {
  return function() {
    return value;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.countBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>countBy (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.countBy)
- description and source-code
```javascript
countBy = function (collection, iteratee) {
  var func = isArray(collection) ? arrayAggregator : baseAggregator,
      accumulator = initializer ? initializer() : {};

  return func(collection, setter, getIteratee(iteratee, 2), accumulator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.create"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>create (prototype, properties)](#apidoc.element.cash.vorpal.lodash.create)
- description and source-code
```javascript
function create(prototype, properties) {
  var result = baseCreate(prototype);
  return properties == null ? result : baseAssign(result, properties);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.curry"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>curry (func, arity, guard)](#apidoc.element.cash.vorpal.lodash.curry)
- description and source-code
```javascript
function curry(func, arity, guard) {
  arity = guard ? undefined : arity;
  var result = createWrap(func, WRAP_CURRY_FLAG, undefined, undefined, undefined, undefined, undefined, arity);
  result.placeholder = curry.placeholder;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.curryRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>curryRight (func, arity, guard)](#apidoc.element.cash.vorpal.lodash.curryRight)
- description and source-code
```javascript
function curryRight(func, arity, guard) {
  arity = guard ? undefined : arity;
  var result = createWrap(func, WRAP_CURRY_RIGHT_FLAG, undefined, undefined, undefined, undefined, undefined, arity);
  result.placeholder = curryRight.placeholder;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.debounce"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>debounce (func, wait, options)](#apidoc.element.cash.vorpal.lodash.debounce)
- description and source-code
```javascript
function debounce(func, wait, options) {
  var lastArgs,
      lastThis,
      maxWait,
      result,
      timerId,
      lastCallTime,
      lastInvokeTime = 0,
      leading = false,
      maxing = false,
      trailing = true;

  if (typeof func != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  wait = toNumber(wait) || 0;
  if (isObject(options)) {
    leading = !!options.leading;
    maxing = 'maxWait' in options;
    maxWait = maxing ? nativeMax(toNumber(options.maxWait) || 0, wait) : maxWait;
    trailing = 'trailing' in options ? !!options.trailing : trailing;
  }

  function invokeFunc(time) {
    var args = lastArgs,
        thisArg = lastThis;

    lastArgs = lastThis = undefined;
    lastInvokeTime = time;
    result = func.apply(thisArg, args);
    return result;
  }

  function leadingEdge(time) {
    // Reset any 'maxWait' timer.
    lastInvokeTime = time;
    // Start the timer for the trailing edge.
    timerId = setTimeout(timerExpired, wait);
    // Invoke the leading edge.
    return leading ? invokeFunc(time) : result;
  }

  function remainingWait(time) {
    var timeSinceLastCall = time - lastCallTime,
        timeSinceLastInvoke = time - lastInvokeTime,
        result = wait - timeSinceLastCall;

    return maxing ? nativeMin(result, maxWait - timeSinceLastInvoke) : result;
  }

  function shouldInvoke(time) {
    var timeSinceLastCall = time - lastCallTime,
        timeSinceLastInvoke = time - lastInvokeTime;

    // Either this is the first call, activity has stopped and we're at the
    // trailing edge, the system time has gone backwards and we're treating
    // it as the trailing edge, or we've hit the 'maxWait' limit.
    return (lastCallTime === undefined || (timeSinceLastCall >= wait) ||
      (timeSinceLastCall < 0) || (maxing && timeSinceLastInvoke >= maxWait));
  }

  function timerExpired() {
    var time = now();
    if (shouldInvoke(time)) {
      return trailingEdge(time);
    }
    // Restart the timer.
    timerId = setTimeout(timerExpired, remainingWait(time));
  }

  function trailingEdge(time) {
    timerId = undefined;

    // Only invoke if we have 'lastArgs' which means 'func' has been
    // debounced at least once.
    if (trailing && lastArgs) {
      return invokeFunc(time);
    }
    lastArgs = lastThis = undefined;
    return result;
  }

  function cancel() {
    if (timerId !== undefined) {
      clearTimeout(timerId);
    }
    lastInvokeTime = 0;
    lastArgs = lastCallTime = lastThis = timerId = undefined;
  }

  function flush() {
    return timerId === undefined ? result : trailingEdge(now());
  }

  function debounced() {
    var time = now(),
        isInvoking = shouldInvoke(time);

    lastArgs = arguments;
    lastThis = this;
    lastCallTime = time;

    if (isInvoking) {
      if (timerId === undefined) {
        return leadingEdge(lastCallTime);
      }
      if (maxing) {
        // Handle invocations in a tight loop.
        timerId = setTimeout(timerExpired, wait);
        return invokeFunc(lastCallTime);
      }
    }
    if (timerId === undefined) {
      timerId = setTimeout(timerExpired, wait);
    }
    return result;
  }
  debounced.cancel = cancel;
  debounced.flush = flush;
  return debounced;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.deburr"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>deburr (string)](#apidoc.element.cash.vorpal.lodash.deburr)
- description and source-code
```javascript
function deburr(string) {
  string = toString(string);
  return string && string.replace(reLatin, deburrLetter).replace(reComboMark, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.defaultTo"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defaultTo (value, defaultValue)](#apidoc.element.cash.vorpal.lodash.defaultTo)
- description and source-code
```javascript
function defaultTo(value, defaultValue) {
  return (value == null || value !== value) ? defaultValue : value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.defaults"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defaults (args)](#apidoc.element.cash.vorpal.lodash.defaults)
- description and source-code
```javascript
defaults = function (args) {
  args.push(undefined, customDefaultsAssignIn);
  return apply(assignInWith, undefined, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.defaultsDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defaultsDeep (args)](#apidoc.element.cash.vorpal.lodash.defaultsDeep)
- description and source-code
```javascript
defaultsDeep = function (args) {
  args.push(undefined, customDefaultsMerge);
  return apply(mergeWith, undefined, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.defer"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>defer (func, args)](#apidoc.element.cash.vorpal.lodash.defer)
- description and source-code
```javascript
defer = function (func, args) {
  return baseDelay(func, 1, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.delay"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>delay (func, wait, args)](#apidoc.element.cash.vorpal.lodash.delay)
- description and source-code
```javascript
delay = function (func, wait, args) {
  return baseDelay(func, toNumber(wait) || 0, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.difference"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>difference (array, values)](#apidoc.element.cash.vorpal.lodash.difference)
- description and source-code
```javascript
difference = function (array, values) {
  return isArrayLikeObject(array)
    ? baseDifference(array, baseFlatten(values, 1, isArrayLikeObject, true))
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.differenceBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>differenceBy (array, values)](#apidoc.element.cash.vorpal.lodash.differenceBy)
- description and source-code
```javascript
differenceBy = function (array, values) {
  var iteratee = last(values);
  if (isArrayLikeObject(iteratee)) {
    iteratee = undefined;
  }
  return isArrayLikeObject(array)
    ? baseDifference(array, baseFlatten(values, 1, isArrayLikeObject, true), getIteratee(iteratee, 2))
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.differenceWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>differenceWith (array, values)](#apidoc.element.cash.vorpal.lodash.differenceWith)
- description and source-code
```javascript
differenceWith = function (array, values) {
  var comparator = last(values);
  if (isArrayLikeObject(comparator)) {
    comparator = undefined;
  }
  return isArrayLikeObject(array)
    ? baseDifference(array, baseFlatten(values, 1, isArrayLikeObject, true), undefined, comparator)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.divide"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>divide (value, other)](#apidoc.element.cash.vorpal.lodash.divide)
- description and source-code
```javascript
divide = function (value, other) {
  var result;
  if (value === undefined && other === undefined) {
    return defaultValue;
  }
  if (value !== undefined) {
    result = value;
  }
  if (other !== undefined) {
    if (result === undefined) {
      return other;
    }
    if (typeof value == 'string' || typeof other == 'string') {
      value = baseToString(value);
      other = baseToString(other);
    } else {
      value = baseToNumber(value);
      other = baseToNumber(other);
    }
    result = operator(value, other);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.drop"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>drop (array, n, guard)](#apidoc.element.cash.vorpal.lodash.drop)
- description and source-code
```javascript
function drop(array, n, guard) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return [];
  }
  n = (guard || n === undefined) ? 1 : toInteger(n);
  return baseSlice(array, n < 0 ? 0 : n, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.dropRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>dropRight (array, n, guard)](#apidoc.element.cash.vorpal.lodash.dropRight)
- description and source-code
```javascript
function dropRight(array, n, guard) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return [];
  }
  n = (guard || n === undefined) ? 1 : toInteger(n);
  n = length - n;
  return baseSlice(array, 0, n < 0 ? 0 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.dropRightWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>dropRightWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.dropRightWhile)
- description and source-code
```javascript
function dropRightWhile(array, predicate) {
  return (array && array.length)
    ? baseWhile(array, getIteratee(predicate, 3), true, true)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.dropWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>dropWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.dropWhile)
- description and source-code
```javascript
function dropWhile(array, predicate) {
  return (array && array.length)
    ? baseWhile(array, getIteratee(predicate, 3), true)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.each"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>each (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.each)
- description and source-code
```javascript
function forEach(collection, iteratee) {
  var func = isArray(collection) ? arrayEach : baseEach;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.eachRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>eachRight (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.eachRight)
- description and source-code
```javascript
function forEachRight(collection, iteratee) {
  var func = isArray(collection) ? arrayEachRight : baseEachRight;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.endsWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>endsWith (string, target, position)](#apidoc.element.cash.vorpal.lodash.endsWith)
- description and source-code
```javascript
function endsWith(string, target, position) {
  string = toString(string);
  target = baseToString(target);

  var length = string.length;
  position = position === undefined
    ? length
    : baseClamp(toInteger(position), 0, length);

  var end = position;
  position -= target.length;
  return position >= 0 && string.slice(position, end) == target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.entries"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>entries (object)](#apidoc.element.cash.vorpal.lodash.entries)
- description and source-code
```javascript
entries = function (object) {
  var tag = getTag(object);
  if (tag == mapTag) {
    return mapToArray(object);
  }
  if (tag == setTag) {
    return setToPairs(object);
  }
  return baseToPairs(object, keysFunc(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.entriesIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>entriesIn (object)](#apidoc.element.cash.vorpal.lodash.entriesIn)
- description and source-code
```javascript
entriesIn = function (object) {
  var tag = getTag(object);
  if (tag == mapTag) {
    return mapToArray(object);
  }
  if (tag == setTag) {
    return setToPairs(object);
  }
  return baseToPairs(object, keysFunc(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.eq"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>eq (value, other)](#apidoc.element.cash.vorpal.lodash.eq)
- description and source-code
```javascript
function eq(value, other) {
  return value === other || (value !== value && other !== other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.escape"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>escape (string)](#apidoc.element.cash.vorpal.lodash.escape)
- description and source-code
```javascript
function escape(string) {
  string = toString(string);
  return (string && reHasUnescapedHtml.test(string))
    ? string.replace(reUnescapedHtml, escapeHtmlChar)
    : string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.escapeRegExp"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>escapeRegExp (string)](#apidoc.element.cash.vorpal.lodash.escapeRegExp)
- description and source-code
```javascript
function escapeRegExp(string) {
  string = toString(string);
  return (string && reHasRegExpChar.test(string))
    ? string.replace(reRegExpChar, '\\$&')
    : string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.every"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>every (collection, predicate, guard)](#apidoc.element.cash.vorpal.lodash.every)
- description and source-code
```javascript
function every(collection, predicate, guard) {
  var func = isArray(collection) ? arrayEvery : baseEvery;
  if (guard && isIterateeCall(collection, predicate, guard)) {
    predicate = undefined;
  }
  return func(collection, getIteratee(predicate, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.extend"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>extend (object, sources)](#apidoc.element.cash.vorpal.lodash.extend)
- description and source-code
```javascript
extend = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.extendWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>extendWith (object, sources)](#apidoc.element.cash.vorpal.lodash.extendWith)
- description and source-code
```javascript
extendWith = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.fill"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>fill (array, value, start, end)](#apidoc.element.cash.vorpal.lodash.fill)
- description and source-code
```javascript
function fill(array, value, start, end) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return [];
  }
  if (start && typeof start != 'number' && isIterateeCall(array, value, start)) {
    start = 0;
    end = length;
  }
  return baseFill(array, value, start, end);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.filter"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>filter (collection, predicate)](#apidoc.element.cash.vorpal.lodash.filter)
- description and source-code
```javascript
function filter(collection, predicate) {
  var func = isArray(collection) ? arrayFilter : baseFilter;
  return func(collection, getIteratee(predicate, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.find"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>find (collection, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.find)
- description and source-code
```javascript
find = function (collection, predicate, fromIndex) {
  var iterable = Object(collection);
  if (!isArrayLike(collection)) {
    var iteratee = getIteratee(predicate, 3);
    collection = keys(collection);
    predicate = function(key) { return iteratee(iterable[key], key, iterable); };
  }
  var index = findIndexFunc(collection, predicate, fromIndex);
  return index > -1 ? iterable[iteratee ? collection[index] : index] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.findIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findIndex (array, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.findIndex)
- description and source-code
```javascript
function findIndex(array, predicate, fromIndex) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return -1;
  }
  var index = fromIndex == null ? 0 : toInteger(fromIndex);
  if (index < 0) {
    index = nativeMax(length + index, 0);
  }
  return baseFindIndex(array, getIteratee(predicate, 3), index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.findKey"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findKey (object, predicate)](#apidoc.element.cash.vorpal.lodash.findKey)
- description and source-code
```javascript
function findKey(object, predicate) {
  return baseFindKey(object, getIteratee(predicate, 3), baseForOwn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.findLast"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findLast (collection, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.findLast)
- description and source-code
```javascript
findLast = function (collection, predicate, fromIndex) {
  var iterable = Object(collection);
  if (!isArrayLike(collection)) {
    var iteratee = getIteratee(predicate, 3);
    collection = keys(collection);
    predicate = function(key) { return iteratee(iterable[key], key, iterable); };
  }
  var index = findIndexFunc(collection, predicate, fromIndex);
  return index > -1 ? iterable[iteratee ? collection[index] : index] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.findLastIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findLastIndex (array, predicate, fromIndex)](#apidoc.element.cash.vorpal.lodash.findLastIndex)
- description and source-code
```javascript
function findLastIndex(array, predicate, fromIndex) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return -1;
  }
  var index = length - 1;
  if (fromIndex !== undefined) {
    index = toInteger(fromIndex);
    index = fromIndex < 0
      ? nativeMax(length + index, 0)
      : nativeMin(index, length - 1);
  }
  return baseFindIndex(array, getIteratee(predicate, 3), index, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.findLastKey"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>findLastKey (object, predicate)](#apidoc.element.cash.vorpal.lodash.findLastKey)
- description and source-code
```javascript
function findLastKey(object, predicate) {
  return baseFindKey(object, getIteratee(predicate, 3), baseForOwnRight);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.first"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>first (array)](#apidoc.element.cash.vorpal.lodash.first)
- description and source-code
```javascript
function head(array) {
  return (array && array.length) ? array[0] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flatMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatMap (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.flatMap)
- description and source-code
```javascript
function flatMap(collection, iteratee) {
  return baseFlatten(map(collection, iteratee), 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flatMapDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatMapDeep (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.flatMapDeep)
- description and source-code
```javascript
function flatMapDeep(collection, iteratee) {
  return baseFlatten(map(collection, iteratee), INFINITY);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flatMapDepth"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatMapDepth (collection, iteratee, depth)](#apidoc.element.cash.vorpal.lodash.flatMapDepth)
- description and source-code
```javascript
function flatMapDepth(collection, iteratee, depth) {
  depth = depth === undefined ? 1 : toInteger(depth);
  return baseFlatten(map(collection, iteratee), depth);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flatten"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flatten (array)](#apidoc.element.cash.vorpal.lodash.flatten)
- description and source-code
```javascript
function flatten(array) {
  var length = array == null ? 0 : array.length;
  return length ? baseFlatten(array, 1) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flattenDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flattenDeep (array)](#apidoc.element.cash.vorpal.lodash.flattenDeep)
- description and source-code
```javascript
function flattenDeep(array) {
  var length = array == null ? 0 : array.length;
  return length ? baseFlatten(array, INFINITY) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flattenDepth"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flattenDepth (array, depth)](#apidoc.element.cash.vorpal.lodash.flattenDepth)
- description and source-code
```javascript
function flattenDepth(array, depth) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return [];
  }
  depth = depth === undefined ? 1 : toInteger(depth);
  return baseFlatten(array, depth);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flip"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flip (func)](#apidoc.element.cash.vorpal.lodash.flip)
- description and source-code
```javascript
function flip(func) {
  return createWrap(func, WRAP_FLIP_FLAG);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.floor"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>floor (number, precision)](#apidoc.element.cash.vorpal.lodash.floor)
- description and source-code
```javascript
floor = function (number, precision) {
  number = toNumber(number);
  precision = precision == null ? 0 : nativeMin(toInteger(precision), 292);
  if (precision) {
    // Shift with exponential notation to avoid floating-point issues.
    // See [MDN](https://mdn.io/round#Examples) for more details.
    var pair = (toString(number) + 'e').split('e'),
        value = func(pair[0] + 'e' + (+pair[1] + precision));

    pair = (toString(value) + 'e').split('e');
    return +(pair[0] + 'e' + (+pair[1] - precision));
  }
  return func(number);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flow"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flow (funcs)](#apidoc.element.cash.vorpal.lodash.flow)
- description and source-code
```javascript
flow = function (funcs) {
  var length = funcs.length,
      index = length,
      prereq = LodashWrapper.prototype.thru;

  if (fromRight) {
    funcs.reverse();
  }
  while (index--) {
    var func = funcs[index];
    if (typeof func != 'function') {
      throw new TypeError(FUNC_ERROR_TEXT);
    }
    if (prereq && !wrapper && getFuncName(func) == 'wrapper') {
      var wrapper = new LodashWrapper([], true);
    }
  }
  index = wrapper ? index : length;
  while (++index < length) {
    func = funcs[index];

    var funcName = getFuncName(func),
        data = funcName == 'wrapper' ? getData(func) : undefined;

    if (data && isLaziable(data[0]) &&
          data[1] == (WRAP_ARY_FLAG | WRAP_CURRY_FLAG | WRAP_PARTIAL_FLAG | WRAP_REARG_FLAG) &&
          !data[4].length && data[9] == 1
        ) {
      wrapper = wrapper[getFuncName(data[0])].apply(wrapper, data[3]);
    } else {
      wrapper = (func.length == 1 && isLaziable(func))
        ? wrapper[funcName]()
        : wrapper.thru(func);
    }
  }
  return function() {
    var args = arguments,
        value = args[0];

    if (wrapper && args.length == 1 && isArray(value)) {
      return wrapper.plant(value).value();
    }
    var index = 0,
        result = length ? funcs[index].apply(this, args) : value;

    while (++index < length) {
      result = funcs[index].call(this, result);
    }
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.flowRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>flowRight (funcs)](#apidoc.element.cash.vorpal.lodash.flowRight)
- description and source-code
```javascript
flowRight = function (funcs) {
  var length = funcs.length,
      index = length,
      prereq = LodashWrapper.prototype.thru;

  if (fromRight) {
    funcs.reverse();
  }
  while (index--) {
    var func = funcs[index];
    if (typeof func != 'function') {
      throw new TypeError(FUNC_ERROR_TEXT);
    }
    if (prereq && !wrapper && getFuncName(func) == 'wrapper') {
      var wrapper = new LodashWrapper([], true);
    }
  }
  index = wrapper ? index : length;
  while (++index < length) {
    func = funcs[index];

    var funcName = getFuncName(func),
        data = funcName == 'wrapper' ? getData(func) : undefined;

    if (data && isLaziable(data[0]) &&
          data[1] == (WRAP_ARY_FLAG | WRAP_CURRY_FLAG | WRAP_PARTIAL_FLAG | WRAP_REARG_FLAG) &&
          !data[4].length && data[9] == 1
        ) {
      wrapper = wrapper[getFuncName(data[0])].apply(wrapper, data[3]);
    } else {
      wrapper = (func.length == 1 && isLaziable(func))
        ? wrapper[funcName]()
        : wrapper.thru(func);
    }
  }
  return function() {
    var args = arguments,
        value = args[0];

    if (wrapper && args.length == 1 && isArray(value)) {
      return wrapper.plant(value).value();
    }
    var index = 0,
        result = length ? funcs[index].apply(this, args) : value;

    while (++index < length) {
      result = funcs[index].call(this, result);
    }
    return result;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.forEach"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forEach (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.forEach)
- description and source-code
```javascript
function forEach(collection, iteratee) {
  var func = isArray(collection) ? arrayEach : baseEach;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.forEachRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forEachRight (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.forEachRight)
- description and source-code
```javascript
function forEachRight(collection, iteratee) {
  var func = isArray(collection) ? arrayEachRight : baseEachRight;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.forIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forIn (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forIn)
- description and source-code
```javascript
function forIn(object, iteratee) {
  return object == null
    ? object
    : baseFor(object, getIteratee(iteratee, 3), keysIn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.forInRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forInRight (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forInRight)
- description and source-code
```javascript
function forInRight(object, iteratee) {
  return object == null
    ? object
    : baseForRight(object, getIteratee(iteratee, 3), keysIn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.forOwn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forOwn (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forOwn)
- description and source-code
```javascript
function forOwn(object, iteratee) {
  return object && baseForOwn(object, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.forOwnRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>forOwnRight (object, iteratee)](#apidoc.element.cash.vorpal.lodash.forOwnRight)
- description and source-code
```javascript
function forOwnRight(object, iteratee) {
  return object && baseForOwnRight(object, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.fromPairs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>fromPairs (pairs)](#apidoc.element.cash.vorpal.lodash.fromPairs)
- description and source-code
```javascript
function fromPairs(pairs) {
  var index = -1,
      length = pairs == null ? 0 : pairs.length,
      result = {};

  while (++index < length) {
    var pair = pairs[index];
    result[pair[0]] = pair[1];
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.functions"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>functions (object)](#apidoc.element.cash.vorpal.lodash.functions)
- description and source-code
```javascript
function functions(object) {
  return object == null ? [] : baseFunctions(object, keys(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.functionsIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>functionsIn (object)](#apidoc.element.cash.vorpal.lodash.functionsIn)
- description and source-code
```javascript
function functionsIn(object) {
  return object == null ? [] : baseFunctions(object, keysIn(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.get"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>get (object, path, defaultValue)](#apidoc.element.cash.vorpal.lodash.get)
- description and source-code
```javascript
function get(object, path, defaultValue) {
  var result = object == null ? undefined : baseGet(object, path);
  return result === undefined ? defaultValue : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.groupBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>groupBy (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.groupBy)
- description and source-code
```javascript
groupBy = function (collection, iteratee) {
  var func = isArray(collection) ? arrayAggregator : baseAggregator,
      accumulator = initializer ? initializer() : {};

  return func(collection, setter, getIteratee(iteratee, 2), accumulator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.gt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>gt (value, other)](#apidoc.element.cash.vorpal.lodash.gt)
- description and source-code
```javascript
gt = function (value, other) {
  if (!(typeof value == 'string' && typeof other == 'string')) {
    value = toNumber(value);
    other = toNumber(other);
  }
  return operator(value, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.gte"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>gte (value, other)](#apidoc.element.cash.vorpal.lodash.gte)
- description and source-code
```javascript
gte = function (value, other) {
  if (!(typeof value == 'string' && typeof other == 'string')) {
    value = toNumber(value);
    other = toNumber(other);
  }
  return operator(value, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.has"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>has (object, path)](#apidoc.element.cash.vorpal.lodash.has)
- description and source-code
```javascript
function has(object, path) {
  return object != null && hasPath(object, path, baseHas);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.hasIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>hasIn (object, path)](#apidoc.element.cash.vorpal.lodash.hasIn)
- description and source-code
```javascript
function hasIn(object, path) {
  return object != null && hasPath(object, path, baseHasIn);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.head"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>head (array)](#apidoc.element.cash.vorpal.lodash.head)
- description and source-code
```javascript
function head(array) {
  return (array && array.length) ? array[0] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.identity"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>identity (value)](#apidoc.element.cash.vorpal.lodash.identity)
- description and source-code
```javascript
function identity(value) {
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.inRange"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>inRange (number, start, end)](#apidoc.element.cash.vorpal.lodash.inRange)
- description and source-code
```javascript
function inRange(number, start, end) {
  start = toFinite(start);
  if (end === undefined) {
    end = start;
    start = 0;
  } else {
    end = toFinite(end);
  }
  number = toNumber(number);
  return baseInRange(number, start, end);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.includes"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>includes (collection, value, fromIndex, guard)](#apidoc.element.cash.vorpal.lodash.includes)
- description and source-code
```javascript
function includes(collection, value, fromIndex, guard) {
  collection = isArrayLike(collection) ? collection : values(collection);
  fromIndex = (fromIndex && !guard) ? toInteger(fromIndex) : 0;

  var length = collection.length;
  if (fromIndex < 0) {
    fromIndex = nativeMax(length + fromIndex, 0);
  }
  return isString(collection)
    ? (fromIndex <= length && collection.indexOf(value, fromIndex) > -1)
    : (!!length && baseIndexOf(collection, value, fromIndex) > -1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.indexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>indexOf (array, value, fromIndex)](#apidoc.element.cash.vorpal.lodash.indexOf)
- description and source-code
```javascript
function indexOf(array, value, fromIndex) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return -1;
  }
  var index = fromIndex == null ? 0 : toInteger(fromIndex);
  if (index < 0) {
    index = nativeMax(length + index, 0);
  }
  return baseIndexOf(array, value, index);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.initial"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>initial (array)](#apidoc.element.cash.vorpal.lodash.initial)
- description and source-code
```javascript
function initial(array) {
  var length = array == null ? 0 : array.length;
  return length ? baseSlice(array, 0, -1) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.intersection"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>intersection (arrays)](#apidoc.element.cash.vorpal.lodash.intersection)
- description and source-code
```javascript
intersection = function (arrays) {
  var mapped = arrayMap(arrays, castArrayLikeObject);
  return (mapped.length && mapped[0] === arrays[0])
    ? baseIntersection(mapped)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.intersectionBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>intersectionBy (arrays)](#apidoc.element.cash.vorpal.lodash.intersectionBy)
- description and source-code
```javascript
intersectionBy = function (arrays) {
  var iteratee = last(arrays),
      mapped = arrayMap(arrays, castArrayLikeObject);

  if (iteratee === last(mapped)) {
    iteratee = undefined;
  } else {
    mapped.pop();
  }
  return (mapped.length && mapped[0] === arrays[0])
    ? baseIntersection(mapped, getIteratee(iteratee, 2))
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.intersectionWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>intersectionWith (arrays)](#apidoc.element.cash.vorpal.lodash.intersectionWith)
- description and source-code
```javascript
intersectionWith = function (arrays) {
  var comparator = last(arrays),
      mapped = arrayMap(arrays, castArrayLikeObject);

  comparator = typeof comparator == 'function' ? comparator : undefined;
  if (comparator) {
    mapped.pop();
  }
  return (mapped.length && mapped[0] === arrays[0])
    ? baseIntersection(mapped, undefined, comparator)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.invert"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invert (object, iteratee)](#apidoc.element.cash.vorpal.lodash.invert)
- description and source-code
```javascript
invert = function (object, iteratee) {
  return baseInverter(object, setter, toIteratee(iteratee), {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.invertBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invertBy (object, iteratee)](#apidoc.element.cash.vorpal.lodash.invertBy)
- description and source-code
```javascript
invertBy = function (object, iteratee) {
  return baseInverter(object, setter, toIteratee(iteratee), {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.invoke"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invoke (object, path, args)](#apidoc.element.cash.vorpal.lodash.invoke)
- description and source-code
```javascript
function baseInvoke(object, path, args) {
  path = castPath(path, object);
  object = parent(object, path);
  var func = object == null ? object : object[toKey(last(path))];
  return func == null ? undefined : apply(func, object, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.invokeMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>invokeMap (collection, path, args)](#apidoc.element.cash.vorpal.lodash.invokeMap)
- description and source-code
```javascript
invokeMap = function (collection, path, args) {
  var index = -1,
      isFunc = typeof path == 'function',
      result = isArrayLike(collection) ? Array(collection.length) : [];

  baseEach(collection, function(value) {
    result[++index] = isFunc ? apply(path, value, args) : baseInvoke(value, path, args);
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isArguments"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArguments (value)](#apidoc.element.cash.vorpal.lodash.isArguments)
- description and source-code
```javascript
function baseIsArguments(value) {
  return isObjectLike(value) && baseGetTag(value) == argsTag;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArray ()](#apidoc.element.cash.vorpal.lodash.isArray)
- description and source-code
```javascript
function isArray() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isArrayBuffer"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArrayBuffer (value)](#apidoc.element.cash.vorpal.lodash.isArrayBuffer)
- description and source-code
```javascript
isArrayBuffer = function (value) {
  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isArrayLike"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArrayLike (value)](#apidoc.element.cash.vorpal.lodash.isArrayLike)
- description and source-code
```javascript
function isArrayLike(value) {
  return value != null && isLength(value.length) && !isFunction(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isArrayLikeObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isArrayLikeObject (value)](#apidoc.element.cash.vorpal.lodash.isArrayLikeObject)
- description and source-code
```javascript
function isArrayLikeObject(value) {
  return isObjectLike(value) && isArrayLike(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isBoolean"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isBoolean (value)](#apidoc.element.cash.vorpal.lodash.isBoolean)
- description and source-code
```javascript
function isBoolean(value) {
  return value === true || value === false ||
    (isObjectLike(value) && baseGetTag(value) == boolTag);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isBuffer"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isBuffer (b)](#apidoc.element.cash.vorpal.lodash.isBuffer)
- description and source-code
```javascript
function isBuffer(b) {
  return b instanceof Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isDate"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isDate (value)](#apidoc.element.cash.vorpal.lodash.isDate)
- description and source-code
```javascript
isDate = function (value) {
  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isElement"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isElement (value)](#apidoc.element.cash.vorpal.lodash.isElement)
- description and source-code
```javascript
function isElement(value) {
  return isObjectLike(value) && value.nodeType === 1 && !isPlainObject(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isEmpty"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isEmpty (value)](#apidoc.element.cash.vorpal.lodash.isEmpty)
- description and source-code
```javascript
function isEmpty(value) {
  if (value == null) {
    return true;
  }
  if (isArrayLike(value) &&
      (isArray(value) || typeof value == 'string' || typeof value.splice == 'function' ||
        isBuffer(value) || isTypedArray(value) || isArguments(value))) {
    return !value.length;
  }
  var tag = getTag(value);
  if (tag == mapTag || tag == setTag) {
    return !value.size;
  }
  if (isPrototype(value)) {
    return !baseKeys(value).length;
  }
  for (var key in value) {
    if (hasOwnProperty.call(value, key)) {
      return false;
    }
  }
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isEqual"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isEqual (value, other)](#apidoc.element.cash.vorpal.lodash.isEqual)
- description and source-code
```javascript
function isEqual(value, other) {
  return baseIsEqual(value, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isEqualWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isEqualWith (value, other, customizer)](#apidoc.element.cash.vorpal.lodash.isEqualWith)
- description and source-code
```javascript
function isEqualWith(value, other, customizer) {
  customizer = typeof customizer == 'function' ? customizer : undefined;
  var result = customizer ? customizer(value, other) : undefined;
  return result === undefined ? baseIsEqual(value, other, undefined, customizer) : !!result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isError"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isError (value)](#apidoc.element.cash.vorpal.lodash.isError)
- description and source-code
```javascript
function isError(value) {
  if (!isObjectLike(value)) {
    return false;
  }
  var tag = baseGetTag(value);
  return tag == errorTag || tag == domExcTag ||
    (typeof value.message == 'string' && typeof value.name == 'string' && !isPlainObject(value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isFinite"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isFinite (value)](#apidoc.element.cash.vorpal.lodash.isFinite)
- description and source-code
```javascript
function isFinite(value) {
  return typeof value == 'number' && nativeIsFinite(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isFunction"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isFunction (value)](#apidoc.element.cash.vorpal.lodash.isFunction)
- description and source-code
```javascript
function isFunction(value) {
  if (!isObject(value)) {
    return false;
  }
  // The use of 'Object#toString' avoids issues with the 'typeof' operator
  // in Safari 9 which returns 'object' for typed arrays and other constructors.
  var tag = baseGetTag(value);
  return tag == funcTag || tag == genTag || tag == asyncTag || tag == proxyTag;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isInteger (value)](#apidoc.element.cash.vorpal.lodash.isInteger)
- description and source-code
```javascript
function isInteger(value) {
  return typeof value == 'number' && value == toInteger(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isLength"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isLength (value)](#apidoc.element.cash.vorpal.lodash.isLength)
- description and source-code
```javascript
function isLength(value) {
  return typeof value == 'number' &&
    value > -1 && value % 1 == 0 && value <= MAX_SAFE_INTEGER;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isMap (value)](#apidoc.element.cash.vorpal.lodash.isMap)
- description and source-code
```javascript
isMap = function (value) {
  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isMatch"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isMatch (object, source)](#apidoc.element.cash.vorpal.lodash.isMatch)
- description and source-code
```javascript
function isMatch(object, source) {
  return object === source || baseIsMatch(object, source, getMatchData(source));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isMatchWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isMatchWith (object, source, customizer)](#apidoc.element.cash.vorpal.lodash.isMatchWith)
- description and source-code
```javascript
function isMatchWith(object, source, customizer) {
  customizer = typeof customizer == 'function' ? customizer : undefined;
  return baseIsMatch(object, source, getMatchData(source), customizer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isNaN"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNaN (value)](#apidoc.element.cash.vorpal.lodash.isNaN)
- description and source-code
```javascript
function isNaN(value) {
  // An 'NaN' primitive is the only value that is not equal to itself.
  // Perform the 'toStringTag' check first to avoid errors with some
  // ActiveX objects in IE.
  return isNumber(value) && value != +value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isNative"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNative (value)](#apidoc.element.cash.vorpal.lodash.isNative)
- description and source-code
```javascript
function isNative(value) {
  if (isMaskable(value)) {
    throw new Error(CORE_ERROR_TEXT);
  }
  return baseIsNative(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isNil"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNil (value)](#apidoc.element.cash.vorpal.lodash.isNil)
- description and source-code
```javascript
function isNil(value) {
  return value == null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isNull"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNull (value)](#apidoc.element.cash.vorpal.lodash.isNull)
- description and source-code
```javascript
function isNull(value) {
  return value === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isNumber"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isNumber (value)](#apidoc.element.cash.vorpal.lodash.isNumber)
- description and source-code
```javascript
function isNumber(value) {
  return typeof value == 'number' ||
    (isObjectLike(value) && baseGetTag(value) == numberTag);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isObject (value)](#apidoc.element.cash.vorpal.lodash.isObject)
- description and source-code
```javascript
function isObject(value) {
  var type = typeof value;
  return value != null && (type == 'object' || type == 'function');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isObjectLike"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isObjectLike (value)](#apidoc.element.cash.vorpal.lodash.isObjectLike)
- description and source-code
```javascript
function isObjectLike(value) {
  return value != null && typeof value == 'object';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isPlainObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isPlainObject (value)](#apidoc.element.cash.vorpal.lodash.isPlainObject)
- description and source-code
```javascript
function isPlainObject(value) {
  if (!isObjectLike(value) || baseGetTag(value) != objectTag) {
    return false;
  }
  var proto = getPrototype(value);
  if (proto === null) {
    return true;
  }
  var Ctor = hasOwnProperty.call(proto, 'constructor') && proto.constructor;
  return typeof Ctor == 'function' && Ctor instanceof Ctor &&
    funcToString.call(Ctor) == objectCtorString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isRegExp"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isRegExp (value)](#apidoc.element.cash.vorpal.lodash.isRegExp)
- description and source-code
```javascript
isRegExp = function (value) {
  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isSafeInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isSafeInteger (value)](#apidoc.element.cash.vorpal.lodash.isSafeInteger)
- description and source-code
```javascript
function isSafeInteger(value) {
  return isInteger(value) && value >= -MAX_SAFE_INTEGER && value <= MAX_SAFE_INTEGER;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isSet"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isSet (value)](#apidoc.element.cash.vorpal.lodash.isSet)
- description and source-code
```javascript
isSet = function (value) {
  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isString"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isString (value)](#apidoc.element.cash.vorpal.lodash.isString)
- description and source-code
```javascript
function isString(value) {
  return typeof value == 'string' ||
    (!isArray(value) && isObjectLike(value) && baseGetTag(value) == stringTag);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isSymbol"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isSymbol (value)](#apidoc.element.cash.vorpal.lodash.isSymbol)
- description and source-code
```javascript
function isSymbol(value) {
  return typeof value == 'symbol' ||
    (isObjectLike(value) && baseGetTag(value) == symbolTag);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isTypedArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isTypedArray (value)](#apidoc.element.cash.vorpal.lodash.isTypedArray)
- description and source-code
```javascript
isTypedArray = function (value) {
  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isUndefined"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isUndefined (value)](#apidoc.element.cash.vorpal.lodash.isUndefined)
- description and source-code
```javascript
function isUndefined(value) {
  return value === undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isWeakMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isWeakMap (value)](#apidoc.element.cash.vorpal.lodash.isWeakMap)
- description and source-code
```javascript
function isWeakMap(value) {
  return isObjectLike(value) && getTag(value) == weakMapTag;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.isWeakSet"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>isWeakSet (value)](#apidoc.element.cash.vorpal.lodash.isWeakSet)
- description and source-code
```javascript
function isWeakSet(value) {
  return isObjectLike(value) && baseGetTag(value) == weakSetTag;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.iteratee"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>iteratee (func)](#apidoc.element.cash.vorpal.lodash.iteratee)
- description and source-code
```javascript
function iteratee(func) {
  return baseIteratee(typeof func == 'function' ? func : baseClone(func, CLONE_DEEP_FLAG));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.join"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>join (array, separator)](#apidoc.element.cash.vorpal.lodash.join)
- description and source-code
```javascript
function join(array, separator) {
  return array == null ? '' : nativeJoin.call(array, separator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.kebabCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>kebabCase (string)](#apidoc.element.cash.vorpal.lodash.kebabCase)
- description and source-code
```javascript
kebabCase = function (string) {
  return arrayReduce(words(deburr(string).replace(reApos, '')), callback, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.keyBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>keyBy (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.keyBy)
- description and source-code
```javascript
keyBy = function (collection, iteratee) {
  var func = isArray(collection) ? arrayAggregator : baseAggregator,
      accumulator = initializer ? initializer() : {};

  return func(collection, setter, getIteratee(iteratee, 2), accumulator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.keys"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>keys (object)](#apidoc.element.cash.vorpal.lodash.keys)
- description and source-code
```javascript
function keys(object) {
  return isArrayLike(object) ? arrayLikeKeys(object) : baseKeys(object);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.keysIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>keysIn (object)](#apidoc.element.cash.vorpal.lodash.keysIn)
- description and source-code
```javascript
function keysIn(object) {
  return isArrayLike(object) ? arrayLikeKeys(object, true) : baseKeysIn(object);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.last"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>last (array)](#apidoc.element.cash.vorpal.lodash.last)
- description and source-code
```javascript
function last(array) {
  var length = array == null ? 0 : array.length;
  return length ? array[length - 1] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.lastIndexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lastIndexOf (array, value, fromIndex)](#apidoc.element.cash.vorpal.lodash.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(array, value, fromIndex) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return -1;
  }
  var index = length;
  if (fromIndex !== undefined) {
    index = toInteger(fromIndex);
    index = index < 0 ? nativeMax(length + index, 0) : nativeMin(index, length - 1);
  }
  return value === value
    ? strictLastIndexOf(array, value, index)
    : baseFindIndex(array, baseIsNaN, index, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.lowerCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lowerCase (string)](#apidoc.element.cash.vorpal.lodash.lowerCase)
- description and source-code
```javascript
lowerCase = function (string) {
  return arrayReduce(words(deburr(string).replace(reApos, '')), callback, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.lowerFirst"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lowerFirst (string)](#apidoc.element.cash.vorpal.lodash.lowerFirst)
- description and source-code
```javascript
lowerFirst = function (string) {
  string = toString(string);

  var strSymbols = hasUnicode(string)
    ? stringToArray(string)
    : undefined;

  var chr = strSymbols
    ? strSymbols[0]
    : string.charAt(0);

  var trailing = strSymbols
    ? castSlice(strSymbols, 1).join('')
    : string.slice(1);

  return chr[methodName]() + trailing;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.lt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lt (value, other)](#apidoc.element.cash.vorpal.lodash.lt)
- description and source-code
```javascript
lt = function (value, other) {
  if (!(typeof value == 'string' && typeof other == 'string')) {
    value = toNumber(value);
    other = toNumber(other);
  }
  return operator(value, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.lte"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>lte (value, other)](#apidoc.element.cash.vorpal.lodash.lte)
- description and source-code
```javascript
lte = function (value, other) {
  if (!(typeof value == 'string' && typeof other == 'string')) {
    value = toNumber(value);
    other = toNumber(other);
  }
  return operator(value, other);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.map"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>map (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.map)
- description and source-code
```javascript
function map(collection, iteratee) {
  var func = isArray(collection) ? arrayMap : baseMap;
  return func(collection, getIteratee(iteratee, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.mapKeys"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mapKeys (object, iteratee)](#apidoc.element.cash.vorpal.lodash.mapKeys)
- description and source-code
```javascript
function mapKeys(object, iteratee) {
  var result = {};
  iteratee = getIteratee(iteratee, 3);

  baseForOwn(object, function(value, key, object) {
    baseAssignValue(result, iteratee(value, key, object), value);
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.mapValues"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mapValues (object, iteratee)](#apidoc.element.cash.vorpal.lodash.mapValues)
- description and source-code
```javascript
function mapValues(object, iteratee) {
  var result = {};
  iteratee = getIteratee(iteratee, 3);

  baseForOwn(object, function(value, key, object) {
    baseAssignValue(result, key, iteratee(value, key, object));
  });
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.matches"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>matches (source)](#apidoc.element.cash.vorpal.lodash.matches)
- description and source-code
```javascript
function matches(source) {
  return baseMatches(baseClone(source, CLONE_DEEP_FLAG));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.matchesProperty"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>matchesProperty (path, srcValue)](#apidoc.element.cash.vorpal.lodash.matchesProperty)
- description and source-code
```javascript
function matchesProperty(path, srcValue) {
  return baseMatchesProperty(path, baseClone(srcValue, CLONE_DEEP_FLAG));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.max"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>max (array)](#apidoc.element.cash.vorpal.lodash.max)
- description and source-code
```javascript
function max(array) {
  return (array && array.length)
    ? baseExtremum(array, identity, baseGt)
    : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.maxBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>maxBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.maxBy)
- description and source-code
```javascript
function maxBy(array, iteratee) {
  return (array && array.length)
    ? baseExtremum(array, getIteratee(iteratee, 2), baseGt)
    : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.mean"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mean (array)](#apidoc.element.cash.vorpal.lodash.mean)
- description and source-code
```javascript
function mean(array) {
  return baseMean(array, identity);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.meanBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>meanBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.meanBy)
- description and source-code
```javascript
function meanBy(array, iteratee) {
  return baseMean(array, getIteratee(iteratee, 2));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.memoize"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>memoize (func, resolver)](#apidoc.element.cash.vorpal.lodash.memoize)
- description and source-code
```javascript
function memoize(func, resolver) {
  if (typeof func != 'function' || (resolver != null && typeof resolver != 'function')) {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  var memoized = function() {
    var args = arguments,
        key = resolver ? resolver.apply(this, args) : args[0],
        cache = memoized.cache;

    if (cache.has(key)) {
      return cache.get(key);
    }
    var result = func.apply(this, args);
    memoized.cache = cache.set(key, result) || cache;
    return result;
  };
  memoized.cache = new (memoize.Cache || MapCache);
  return memoized;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.merge"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>merge (object, sources)](#apidoc.element.cash.vorpal.lodash.merge)
- description and source-code
```javascript
merge = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.mergeWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mergeWith (object, sources)](#apidoc.element.cash.vorpal.lodash.mergeWith)
- description and source-code
```javascript
mergeWith = function (object, sources) {
  var index = -1,
      length = sources.length,
      customizer = length > 1 ? sources[length - 1] : undefined,
      guard = length > 2 ? sources[2] : undefined;

  customizer = (assigner.length > 3 && typeof customizer == 'function')
    ? (length--, customizer)
    : undefined;

  if (guard && isIterateeCall(sources[0], sources[1], guard)) {
    customizer = length < 3 ? undefined : customizer;
    length = 1;
  }
  object = Object(object);
  while (++index < length) {
    var source = sources[index];
    if (source) {
      assigner(object, source, index, customizer);
    }
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.method"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>method (path, args)](#apidoc.element.cash.vorpal.lodash.method)
- description and source-code
```javascript
method = function (path, args) {
  return function(object) {
    return baseInvoke(object, path, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.methodOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>methodOf (object, args)](#apidoc.element.cash.vorpal.lodash.methodOf)
- description and source-code
```javascript
methodOf = function (object, args) {
  return function(path) {
    return baseInvoke(object, path, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.min"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>min (array)](#apidoc.element.cash.vorpal.lodash.min)
- description and source-code
```javascript
function min(array) {
  return (array && array.length)
    ? baseExtremum(array, identity, baseLt)
    : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.minBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>minBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.minBy)
- description and source-code
```javascript
function minBy(array, iteratee) {
  return (array && array.length)
    ? baseExtremum(array, getIteratee(iteratee, 2), baseLt)
    : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.mixin"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>mixin (object, source, options)](#apidoc.element.cash.vorpal.lodash.mixin)
- description and source-code
```javascript
function mixin(object, source, options) {
  var props = keys(source),
      methodNames = baseFunctions(source, props);

  if (options == null &&
      !(isObject(source) && (methodNames.length || !props.length))) {
    options = source;
    source = object;
    object = this;
    methodNames = baseFunctions(source, keys(source));
  }
  var chain = !(isObject(options) && 'chain' in options) || !!options.chain,
      isFunc = isFunction(object);

  arrayEach(methodNames, function(methodName) {
    var func = source[methodName];
    object[methodName] = func;
    if (isFunc) {
      object.prototype[methodName] = function() {
        var chainAll = this.__chain__;
        if (chain || chainAll) {
          var result = object(this.__wrapped__),
              actions = result.__actions__ = copyArray(this.__actions__);

          actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
          result.__chain__ = chainAll;
          return result;
        }
        return func.apply(object, arrayPush([this.value()], arguments));
      };
    }
  });

  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.multiply"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>multiply (value, other)](#apidoc.element.cash.vorpal.lodash.multiply)
- description and source-code
```javascript
multiply = function (value, other) {
  var result;
  if (value === undefined && other === undefined) {
    return defaultValue;
  }
  if (value !== undefined) {
    result = value;
  }
  if (other !== undefined) {
    if (result === undefined) {
      return other;
    }
    if (typeof value == 'string' || typeof other == 'string') {
      value = baseToString(value);
      other = baseToString(other);
    } else {
      value = baseToNumber(value);
      other = baseToNumber(other);
    }
    result = operator(value, other);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.negate"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>negate (predicate)](#apidoc.element.cash.vorpal.lodash.negate)
- description and source-code
```javascript
function negate(predicate) {
  if (typeof predicate != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  return function() {
    var args = arguments;
    switch (args.length) {
      case 0: return !predicate.call(this);
      case 1: return !predicate.call(this, args[0]);
      case 2: return !predicate.call(this, args[0], args[1]);
      case 3: return !predicate.call(this, args[0], args[1], args[2]);
    }
    return !predicate.apply(this, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.noConflict"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>noConflict ()](#apidoc.element.cash.vorpal.lodash.noConflict)
- description and source-code
```javascript
function noConflict() {
  if (root._ === this) {
    root._ = oldDash;
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.noop"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>noop ()](#apidoc.element.cash.vorpal.lodash.noop)
- description and source-code
```javascript
function noop() {
  // No operation performed.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.now"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>now ()](#apidoc.element.cash.vorpal.lodash.now)
- description and source-code
```javascript
now = function () {
  return root.Date.now();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.nth"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>nth (array, n)](#apidoc.element.cash.vorpal.lodash.nth)
- description and source-code
```javascript
function nth(array, n) {
  return (array && array.length) ? baseNth(array, toInteger(n)) : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.nthArg"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>nthArg (n)](#apidoc.element.cash.vorpal.lodash.nthArg)
- description and source-code
```javascript
function nthArg(n) {
  n = toInteger(n);
  return baseRest(function(args) {
    return baseNth(args, n);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.omit"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>omit (object, paths)](#apidoc.element.cash.vorpal.lodash.omit)
- description and source-code
```javascript
omit = function (object, paths) {
  var result = {};
  if (object == null) {
    return result;
  }
  var isDeep = false;
  paths = arrayMap(paths, function(path) {
    path = castPath(path, object);
    isDeep || (isDeep = path.length > 1);
    return path;
  });
  copyObject(object, getAllKeysIn(object), result);
  if (isDeep) {
    result = baseClone(result, CLONE_DEEP_FLAG | CLONE_FLAT_FLAG | CLONE_SYMBOLS_FLAG, customOmitClone);
  }
  var length = paths.length;
  while (length--) {
    baseUnset(result, paths[length]);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.omitBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>omitBy (object, predicate)](#apidoc.element.cash.vorpal.lodash.omitBy)
- description and source-code
```javascript
function omitBy(object, predicate) {
  return pickBy(object, negate(getIteratee(predicate)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.once"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>once (func)](#apidoc.element.cash.vorpal.lodash.once)
- description and source-code
```javascript
function once(func) {
  return before(2, func);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.orderBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>orderBy (collection, iteratees, orders, guard)](#apidoc.element.cash.vorpal.lodash.orderBy)
- description and source-code
```javascript
function orderBy(collection, iteratees, orders, guard) {
  if (collection == null) {
    return [];
  }
  if (!isArray(iteratees)) {
    iteratees = iteratees == null ? [] : [iteratees];
  }
  orders = guard ? undefined : orders;
  if (!isArray(orders)) {
    orders = orders == null ? [] : [orders];
  }
  return baseOrderBy(collection, iteratees, orders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.over"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>over (iteratees)](#apidoc.element.cash.vorpal.lodash.over)
- description and source-code
```javascript
over = function (iteratees) {
  iteratees = arrayMap(iteratees, baseUnary(getIteratee()));
  return baseRest(function(args) {
    var thisArg = this;
    return arrayFunc(iteratees, function(iteratee) {
      return apply(iteratee, thisArg, args);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.overArgs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>overArgs (func, transforms)](#apidoc.element.cash.vorpal.lodash.overArgs)
- description and source-code
```javascript
overArgs = function (func, transforms) {
  transforms = (transforms.length == 1 && isArray(transforms[0]))
    ? arrayMap(transforms[0], baseUnary(getIteratee()))
    : arrayMap(baseFlatten(transforms, 1), baseUnary(getIteratee()));

  var funcsLength = transforms.length;
  return baseRest(function(args) {
    var index = -1,
        length = nativeMin(args.length, funcsLength);

    while (++index < length) {
      args[index] = transforms[index].call(this, args[index]);
    }
    return apply(func, this, args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.overEvery"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>overEvery (iteratees)](#apidoc.element.cash.vorpal.lodash.overEvery)
- description and source-code
```javascript
overEvery = function (iteratees) {
  iteratees = arrayMap(iteratees, baseUnary(getIteratee()));
  return baseRest(function(args) {
    var thisArg = this;
    return arrayFunc(iteratees, function(iteratee) {
      return apply(iteratee, thisArg, args);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.overSome"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>overSome (iteratees)](#apidoc.element.cash.vorpal.lodash.overSome)
- description and source-code
```javascript
overSome = function (iteratees) {
  iteratees = arrayMap(iteratees, baseUnary(getIteratee()));
  return baseRest(function(args) {
    var thisArg = this;
    return arrayFunc(iteratees, function(iteratee) {
      return apply(iteratee, thisArg, args);
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pad"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pad (string, length, chars)](#apidoc.element.cash.vorpal.lodash.pad)
- description and source-code
```javascript
function pad(string, length, chars) {
  string = toString(string);
  length = toInteger(length);

  var strLength = length ? stringSize(string) : 0;
  if (!length || strLength >= length) {
    return string;
  }
  var mid = (length - strLength) / 2;
  return (
    createPadding(nativeFloor(mid), chars) +
    string +
    createPadding(nativeCeil(mid), chars)
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.padEnd"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>padEnd (string, length, chars)](#apidoc.element.cash.vorpal.lodash.padEnd)
- description and source-code
```javascript
function padEnd(string, length, chars) {
  string = toString(string);
  length = toInteger(length);

  var strLength = length ? stringSize(string) : 0;
  return (length && strLength < length)
    ? (string + createPadding(length - strLength, chars))
    : string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.padStart"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>padStart (string, length, chars)](#apidoc.element.cash.vorpal.lodash.padStart)
- description and source-code
```javascript
function padStart(string, length, chars) {
  string = toString(string);
  length = toInteger(length);

  var strLength = length ? stringSize(string) : 0;
  return (length && strLength < length)
    ? (createPadding(length - strLength, chars) + string)
    : string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.parseInt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>parseInt (string, radix, guard)](#apidoc.element.cash.vorpal.lodash.parseInt)
- description and source-code
```javascript
function parseInt(string, radix, guard) {
  if (guard || radix == null) {
    radix = 0;
  } else if (radix) {
    radix = +radix;
  }
  return nativeParseInt(toString(string).replace(reTrimStart, ''), radix || 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.partial"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>partial (func, partials)](#apidoc.element.cash.vorpal.lodash.partial)
- description and source-code
```javascript
partial = function (func, partials) {
  var holders = replaceHolders(partials, getHolder(partial));
  return createWrap(func, WRAP_PARTIAL_FLAG, undefined, partials, holders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.partialRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>partialRight (func, partials)](#apidoc.element.cash.vorpal.lodash.partialRight)
- description and source-code
```javascript
partialRight = function (func, partials) {
  var holders = replaceHolders(partials, getHolder(partialRight));
  return createWrap(func, WRAP_PARTIAL_RIGHT_FLAG, undefined, partials, holders);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.partition"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>partition (collection, iteratee)](#apidoc.element.cash.vorpal.lodash.partition)
- description and source-code
```javascript
partition = function (collection, iteratee) {
  var func = isArray(collection) ? arrayAggregator : baseAggregator,
      accumulator = initializer ? initializer() : {};

  return func(collection, setter, getIteratee(iteratee, 2), accumulator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pick"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pick (object, paths)](#apidoc.element.cash.vorpal.lodash.pick)
- description and source-code
```javascript
pick = function (object, paths) {
  return object == null ? {} : basePick(object, paths);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pickBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pickBy (object, predicate)](#apidoc.element.cash.vorpal.lodash.pickBy)
- description and source-code
```javascript
function pickBy(object, predicate) {
  if (object == null) {
    return {};
  }
  var props = arrayMap(getAllKeysIn(object), function(prop) {
    return [prop];
  });
  predicate = getIteratee(predicate);
  return basePickBy(object, props, function(value, path) {
    return predicate(value, path[0]);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.property"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>property (path)](#apidoc.element.cash.vorpal.lodash.property)
- description and source-code
```javascript
function property(path) {
  return isKey(path) ? baseProperty(toKey(path)) : basePropertyDeep(path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.propertyOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>propertyOf (object)](#apidoc.element.cash.vorpal.lodash.propertyOf)
- description and source-code
```javascript
function propertyOf(object) {
  return function(path) {
    return object == null ? undefined : baseGet(object, path);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pull"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pull (array, values)](#apidoc.element.cash.vorpal.lodash.pull)
- description and source-code
```javascript
function pullAll(array, values) {
  return (array && array.length && values && values.length)
    ? basePullAll(array, values)
    : array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pullAll"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAll (array, values)](#apidoc.element.cash.vorpal.lodash.pullAll)
- description and source-code
```javascript
function pullAll(array, values) {
  return (array && array.length && values && values.length)
    ? basePullAll(array, values)
    : array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pullAllBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAllBy (array, values, iteratee)](#apidoc.element.cash.vorpal.lodash.pullAllBy)
- description and source-code
```javascript
function pullAllBy(array, values, iteratee) {
  return (array && array.length && values && values.length)
    ? basePullAll(array, values, getIteratee(iteratee, 2))
    : array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pullAllWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAllWith (array, values, comparator)](#apidoc.element.cash.vorpal.lodash.pullAllWith)
- description and source-code
```javascript
function pullAllWith(array, values, comparator) {
  return (array && array.length && values && values.length)
    ? basePullAll(array, values, undefined, comparator)
    : array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.pullAt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>pullAt (array, indexes)](#apidoc.element.cash.vorpal.lodash.pullAt)
- description and source-code
```javascript
pullAt = function (array, indexes) {
  var length = array == null ? 0 : array.length,
      result = baseAt(array, indexes);

  basePullAt(array, arrayMap(indexes, function(index) {
    return isIndex(index, length) ? +index : index;
  }).sort(compareAscending));

  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.random"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>random (lower, upper, floating)](#apidoc.element.cash.vorpal.lodash.random)
- description and source-code
```javascript
function random(lower, upper, floating) {
  if (floating && typeof floating != 'boolean' && isIterateeCall(lower, upper, floating)) {
    upper = floating = undefined;
  }
  if (floating === undefined) {
    if (typeof upper == 'boolean') {
      floating = upper;
      upper = undefined;
    }
    else if (typeof lower == 'boolean') {
      floating = lower;
      lower = undefined;
    }
  }
  if (lower === undefined && upper === undefined) {
    lower = 0;
    upper = 1;
  }
  else {
    lower = toFinite(lower);
    if (upper === undefined) {
      upper = lower;
      lower = 0;
    } else {
      upper = toFinite(upper);
    }
  }
  if (lower > upper) {
    var temp = lower;
    lower = upper;
    upper = temp;
  }
  if (floating || lower % 1 || upper % 1) {
    var rand = nativeRandom();
    return nativeMin(lower + (rand * (upper - lower + freeParseFloat('1e-' + ((rand + '').length - 1)))), upper);
  }
  return baseRandom(lower, upper);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.range"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>range (start, end, step)](#apidoc.element.cash.vorpal.lodash.range)
- description and source-code
```javascript
range = function (start, end, step) {
  if (step && typeof step != 'number' && isIterateeCall(start, end, step)) {
    end = step = undefined;
  }
  // Ensure the sign of '-0' is preserved.
  start = toFinite(start);
  if (end === undefined) {
    end = start;
    start = 0;
  } else {
    end = toFinite(end);
  }
  step = step === undefined ? (start < end ? 1 : -1) : toFinite(step);
  return baseRange(start, end, step, fromRight);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.rangeRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>rangeRight (start, end, step)](#apidoc.element.cash.vorpal.lodash.rangeRight)
- description and source-code
```javascript
rangeRight = function (start, end, step) {
  if (step && typeof step != 'number' && isIterateeCall(start, end, step)) {
    end = step = undefined;
  }
  // Ensure the sign of '-0' is preserved.
  start = toFinite(start);
  if (end === undefined) {
    end = start;
    start = 0;
  } else {
    end = toFinite(end);
  }
  step = step === undefined ? (start < end ? 1 : -1) : toFinite(step);
  return baseRange(start, end, step, fromRight);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.rearg"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>rearg (func, indexes)](#apidoc.element.cash.vorpal.lodash.rearg)
- description and source-code
```javascript
rearg = function (func, indexes) {
  return createWrap(func, WRAP_REARG_FLAG, undefined, undefined, undefined, indexes);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.reduce"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reduce (collection, iteratee, accumulator)](#apidoc.element.cash.vorpal.lodash.reduce)
- description and source-code
```javascript
function reduce(collection, iteratee, accumulator) {
  var func = isArray(collection) ? arrayReduce : baseReduce,
      initAccum = arguments.length < 3;

  return func(collection, getIteratee(iteratee, 4), accumulator, initAccum, baseEach);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.reduceRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reduceRight (collection, iteratee, accumulator)](#apidoc.element.cash.vorpal.lodash.reduceRight)
- description and source-code
```javascript
function reduceRight(collection, iteratee, accumulator) {
  var func = isArray(collection) ? arrayReduceRight : baseReduce,
      initAccum = arguments.length < 3;

  return func(collection, getIteratee(iteratee, 4), accumulator, initAccum, baseEachRight);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.reject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reject (collection, predicate)](#apidoc.element.cash.vorpal.lodash.reject)
- description and source-code
```javascript
function reject(collection, predicate) {
  var func = isArray(collection) ? arrayFilter : baseFilter;
  return func(collection, negate(getIteratee(predicate, 3)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.remove"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>remove (array, predicate)](#apidoc.element.cash.vorpal.lodash.remove)
- description and source-code
```javascript
function remove(array, predicate) {
  var result = [];
  if (!(array && array.length)) {
    return result;
  }
  var index = -1,
      indexes = [],
      length = array.length;

  predicate = getIteratee(predicate, 3);
  while (++index < length) {
    var value = array[index];
    if (predicate(value, index, array)) {
      result.push(value);
      indexes.push(index);
    }
  }
  basePullAt(array, indexes);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.repeat"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>repeat (string, n, guard)](#apidoc.element.cash.vorpal.lodash.repeat)
- description and source-code
```javascript
function repeat(string, n, guard) {
  if ((guard ? isIterateeCall(string, n, guard) : n === undefined)) {
    n = 1;
  } else {
    n = toInteger(n);
  }
  return baseRepeat(toString(string), n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.replace"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>replace ()](#apidoc.element.cash.vorpal.lodash.replace)
- description and source-code
```javascript
function replace() {
  var args = arguments,
      string = toString(args[0]);

  return args.length < 3 ? string : string.replace(args[1], args[2]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.rest"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>rest (func, start)](#apidoc.element.cash.vorpal.lodash.rest)
- description and source-code
```javascript
function rest(func, start) {
  if (typeof func != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  start = start === undefined ? start : toInteger(start);
  return baseRest(func, start);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.result"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>result (object, path, defaultValue)](#apidoc.element.cash.vorpal.lodash.result)
- description and source-code
```javascript
function result(object, path, defaultValue) {
  path = castPath(path, object);

  var index = -1,
      length = path.length;

  // Ensure the loop is entered when path is empty.
  if (!length) {
    length = 1;
    object = undefined;
  }
  while (++index < length) {
    var value = object == null ? undefined : object[toKey(path[index])];
    if (value === undefined) {
      index = length;
      value = defaultValue;
    }
    object = isFunction(value) ? value.call(object) : value;
  }
  return object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.reverse"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>reverse (array)](#apidoc.element.cash.vorpal.lodash.reverse)
- description and source-code
```javascript
function reverse(array) {
  return array == null ? array : nativeReverse.call(array);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.round"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>round (number, precision)](#apidoc.element.cash.vorpal.lodash.round)
- description and source-code
```javascript
round = function (number, precision) {
  number = toNumber(number);
  precision = precision == null ? 0 : nativeMin(toInteger(precision), 292);
  if (precision) {
    // Shift with exponential notation to avoid floating-point issues.
    // See [MDN](https://mdn.io/round#Examples) for more details.
    var pair = (toString(number) + 'e').split('e'),
        value = func(pair[0] + 'e' + (+pair[1] + precision));

    pair = (toString(value) + 'e').split('e');
    return +(pair[0] + 'e' + (+pair[1] - precision));
  }
  return func(number);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.runInContext"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>runInContext (context)](#apidoc.element.cash.vorpal.lodash.runInContext)
- description and source-code
```javascript
function runInContext(context) {
  context = context == null ? root : _.defaults(root.Object(), context, _.pick(root, contextProps));

<span class="apidocCodeCommentSpan">  /** Built-in constructor references. */
</span>  var Array = context.Array,
      Date = context.Date,
      Error = context.Error,
      Function = context.Function,
      Math = context.Math,
      Object = context.Object,
      RegExp = context.RegExp,
      String = context.String,
      TypeError = context.TypeError;

  /** Used for built-in method references. */
  var arrayProto = Array.prototype,
      funcProto = Function.prototype,
      objectProto = Object.prototype;

  /** Used to detect overreaching core-js shims. */
  var coreJsData = context['__core-js_shared__'];

  /** Used to resolve the decompiled source of functions. */
  var funcToString = funcProto.toString;

  /** Used to check objects for own properties. */
  var hasOwnProperty = objectProto.hasOwnProperty;

  /** Used to generate unique IDs. */
  var idCounter = 0;

  /** Used to detect methods masquerading as native. */
  var maskSrcKey = (function() {
    var uid = /[^.]+$/.exec(coreJsData && coreJsData.keys && coreJsData.keys.IE_PROTO || '');
    return uid ? ('Symbol(src)_1.' + uid) : '';
  }());

  /**
   * Used to resolve the
   * ['toStringTag'](http://ecma-international.org/ecma-262/7.0/#sec-object.prototype.tostring)
   * of values.
   */
  var nativeObjectToString = objectProto.toString;

  /** Used to infer the 'Object' constructor. */
  var objectCtorString = funcToString.call(Object);

  /** Used to restore the original '_' reference in '_.noConflict'. */
  var oldDash = root._;

  /** Used to detect if a method is native. */
  var reIsNative = RegExp('^' +
    funcToString.call(hasOwnProperty).replace(reRegExpChar, '\\$&')
    .replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, '$1.*?') + '$'
  );

  /** Built-in value references. */
  var Buffer = moduleExports ? context.Buffer : undefined,
      Symbol = context.Symbol,
      Uint8Array = context.Uint8Array,
      allocUnsafe = Buffer ? Buffer.allocUnsafe : undefined,
      getPrototype = overArg(Object.getPrototypeOf, Object),
      objectCreate = Object.create,
      propertyIsEnumerable = objectProto.propertyIsEnumerable,
      splice = arrayProto.splice,
      spreadableSymbol = Symbol ? Symbol.isConcatSpreadable : undefined,
      symIterator = Symbol ? Symbol.iterator : undefined,
      symToStringTag = Symbol ? Symbol.toStringTag : undefined;

  var defineProperty = (function() {
    try {
      var func = getNative(Object, 'defineProperty');
      func({}, '', {});
      return func;
    } catch (e) {}
  }());

  /** Mocked built-ins. */
  var ctxClearTimeout = context.clearTimeout !== root.clearTimeout && context.clearTimeout,
      ctxNow = Date && Date.now !== root.Date.now && Date.now,
      ctxSetTimeout = context.setTimeout !== root.setTimeout && context.setTimeout;

  /* Built-in method references for those with the same name as other 'lodash' methods. */
  var nativeCeil = Math.ceil,
      nativeFloor = Math.floor,
      nativeGetSymbols = Object.getOwnPropertySymbols,
      nativeIsBuffer = Buffer ? Buffer.isBuffer : undefined,
      nativeIsFinite = context.isFinite,
      nativeJoin = arrayProto.join,
      nativeKeys = overArg(Object.keys, Object),
      nativeMax = Math.max,
      nativeMin = Math.min,
      nativeNow = Date.now,
      nativeParseInt = context.parseInt,
      nativeRandom = Math.random,
      nativeReverse = arrayProto.reverse;

  /* Built-in method references that are verified to be native. */
  var DataView = getNative(context, 'DataView'),
      Map = getNative(context, 'Map'),
      Promise = getNative(context, 'Promise'),
      Set = getNative(context, 'Set'),
      WeakMap = getNative(context, 'WeakMap'),
      nativeCreate = getNative(Object, 'create');

  /** Used to store function metadata. */
  var metaMap = WeakMap && new WeakMap;

  /** Used to lookup unminified function names. */
  var realNames = {};

  /** Used to detect maps, sets, and weakmaps. */
  var dataViewCtorString = toSource(D ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sample"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sample (collection)](#apidoc.element.cash.vorpal.lodash.sample)
- description and source-code
```javascript
function sample(collection) {
  var func = isArray(collection) ? arraySample : baseSample;
  return func(collection);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sampleSize"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sampleSize (collection, n, guard)](#apidoc.element.cash.vorpal.lodash.sampleSize)
- description and source-code
```javascript
function sampleSize(collection, n, guard) {
  if ((guard ? isIterateeCall(collection, n, guard) : n === undefined)) {
    n = 1;
  } else {
    n = toInteger(n);
  }
  var func = isArray(collection) ? arraySampleSize : baseSampleSize;
  return func(collection, n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.set"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>set (object, path, value)](#apidoc.element.cash.vorpal.lodash.set)
- description and source-code
```javascript
function set(object, path, value) {
  return object == null ? object : baseSet(object, path, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.setWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>setWith (object, path, value, customizer)](#apidoc.element.cash.vorpal.lodash.setWith)
- description and source-code
```javascript
function setWith(object, path, value, customizer) {
  customizer = typeof customizer == 'function' ? customizer : undefined;
  return object == null ? object : baseSet(object, path, value, customizer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.shuffle"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>shuffle (collection)](#apidoc.element.cash.vorpal.lodash.shuffle)
- description and source-code
```javascript
function shuffle(collection) {
  var func = isArray(collection) ? arrayShuffle : baseShuffle;
  return func(collection);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.size"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>size (collection)](#apidoc.element.cash.vorpal.lodash.size)
- description and source-code
```javascript
function size(collection) {
  if (collection == null) {
    return 0;
  }
  if (isArrayLike(collection)) {
    return isString(collection) ? stringSize(collection) : collection.length;
  }
  var tag = getTag(collection);
  if (tag == mapTag || tag == setTag) {
    return collection.size;
  }
  return baseKeys(collection).length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.slice"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>slice (array, start, end)](#apidoc.element.cash.vorpal.lodash.slice)
- description and source-code
```javascript
function slice(array, start, end) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return [];
  }
  if (end && typeof end != 'number' && isIterateeCall(array, start, end)) {
    start = 0;
    end = length;
  }
  else {
    start = start == null ? 0 : toInteger(start);
    end = end === undefined ? length : toInteger(end);
  }
  return baseSlice(array, start, end);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.snakeCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>snakeCase (string)](#apidoc.element.cash.vorpal.lodash.snakeCase)
- description and source-code
```javascript
snakeCase = function (string) {
  return arrayReduce(words(deburr(string).replace(reApos, '')), callback, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.some"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>some (collection, predicate, guard)](#apidoc.element.cash.vorpal.lodash.some)
- description and source-code
```javascript
function some(collection, predicate, guard) {
  var func = isArray(collection) ? arraySome : baseSome;
  if (guard && isIterateeCall(collection, predicate, guard)) {
    predicate = undefined;
  }
  return func(collection, getIteratee(predicate, 3));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortBy (collection, iteratees)](#apidoc.element.cash.vorpal.lodash.sortBy)
- description and source-code
```javascript
sortBy = function (collection, iteratees) {
  if (collection == null) {
    return [];
  }
  var length = iteratees.length;
  if (length > 1 && isIterateeCall(collection, iteratees[0], iteratees[1])) {
    iteratees = [];
  } else if (length > 2 && isIterateeCall(iteratees[0], iteratees[1], iteratees[2])) {
    iteratees = [iteratees[0]];
  }
  return baseOrderBy(collection, baseFlatten(iteratees, 1), []);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedIndex (array, value)](#apidoc.element.cash.vorpal.lodash.sortedIndex)
- description and source-code
```javascript
function sortedIndex(array, value) {
  return baseSortedIndex(array, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedIndexBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedIndexBy (array, value, iteratee)](#apidoc.element.cash.vorpal.lodash.sortedIndexBy)
- description and source-code
```javascript
function sortedIndexBy(array, value, iteratee) {
  return baseSortedIndexBy(array, value, getIteratee(iteratee, 2));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedIndexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedIndexOf (array, value)](#apidoc.element.cash.vorpal.lodash.sortedIndexOf)
- description and source-code
```javascript
function sortedIndexOf(array, value) {
  var length = array == null ? 0 : array.length;
  if (length) {
    var index = baseSortedIndex(array, value);
    if (index < length && eq(array[index], value)) {
      return index;
    }
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedLastIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedLastIndex (array, value)](#apidoc.element.cash.vorpal.lodash.sortedLastIndex)
- description and source-code
```javascript
function sortedLastIndex(array, value) {
  return baseSortedIndex(array, value, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedLastIndexBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedLastIndexBy (array, value, iteratee)](#apidoc.element.cash.vorpal.lodash.sortedLastIndexBy)
- description and source-code
```javascript
function sortedLastIndexBy(array, value, iteratee) {
  return baseSortedIndexBy(array, value, getIteratee(iteratee, 2), true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedLastIndexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedLastIndexOf (array, value)](#apidoc.element.cash.vorpal.lodash.sortedLastIndexOf)
- description and source-code
```javascript
function sortedLastIndexOf(array, value) {
  var length = array == null ? 0 : array.length;
  if (length) {
    var index = baseSortedIndex(array, value, true) - 1;
    if (eq(array[index], value)) {
      return index;
    }
  }
  return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedUniq"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedUniq (array)](#apidoc.element.cash.vorpal.lodash.sortedUniq)
- description and source-code
```javascript
function sortedUniq(array) {
  return (array && array.length)
    ? baseSortedUniq(array)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sortedUniqBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sortedUniqBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.sortedUniqBy)
- description and source-code
```javascript
function sortedUniqBy(array, iteratee) {
  return (array && array.length)
    ? baseSortedUniq(array, getIteratee(iteratee, 2))
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.split"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>split (string, separator, limit)](#apidoc.element.cash.vorpal.lodash.split)
- description and source-code
```javascript
function split(string, separator, limit) {
  if (limit && typeof limit != 'number' && isIterateeCall(string, separator, limit)) {
    separator = limit = undefined;
  }
  limit = limit === undefined ? MAX_ARRAY_LENGTH : limit >>> 0;
  if (!limit) {
    return [];
  }
  string = toString(string);
  if (string && (
        typeof separator == 'string' ||
        (separator != null && !isRegExp(separator))
      )) {
    separator = baseToString(separator);
    if (!separator && hasUnicode(string)) {
      return castSlice(stringToArray(string), 0, limit);
    }
  }
  return string.split(separator, limit);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.spread"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>spread (func, start)](#apidoc.element.cash.vorpal.lodash.spread)
- description and source-code
```javascript
function spread(func, start) {
  if (typeof func != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  start = start == null ? 0 : nativeMax(toInteger(start), 0);
  return baseRest(function(args) {
    var array = args[start],
        otherArgs = castSlice(args, 0, start);

    if (array) {
      arrayPush(otherArgs, array);
    }
    return apply(func, this, otherArgs);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.startCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>startCase (string)](#apidoc.element.cash.vorpal.lodash.startCase)
- description and source-code
```javascript
startCase = function (string) {
  return arrayReduce(words(deburr(string).replace(reApos, '')), callback, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.startsWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>startsWith (string, target, position)](#apidoc.element.cash.vorpal.lodash.startsWith)
- description and source-code
```javascript
function startsWith(string, target, position) {
  string = toString(string);
  position = position == null
    ? 0
    : baseClamp(toInteger(position), 0, string.length);

  target = baseToString(target);
  return string.slice(position, position + target.length) == target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.stubArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubArray ()](#apidoc.element.cash.vorpal.lodash.stubArray)
- description and source-code
```javascript
function stubArray() {
  return [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.stubFalse"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubFalse ()](#apidoc.element.cash.vorpal.lodash.stubFalse)
- description and source-code
```javascript
function stubFalse() {
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.stubObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubObject ()](#apidoc.element.cash.vorpal.lodash.stubObject)
- description and source-code
```javascript
function stubObject() {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.stubString"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubString ()](#apidoc.element.cash.vorpal.lodash.stubString)
- description and source-code
```javascript
function stubString() {
  return '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.stubTrue"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>stubTrue ()](#apidoc.element.cash.vorpal.lodash.stubTrue)
- description and source-code
```javascript
function stubTrue() {
  return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.subtract"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>subtract (value, other)](#apidoc.element.cash.vorpal.lodash.subtract)
- description and source-code
```javascript
subtract = function (value, other) {
  var result;
  if (value === undefined && other === undefined) {
    return defaultValue;
  }
  if (value !== undefined) {
    result = value;
  }
  if (other !== undefined) {
    if (result === undefined) {
      return other;
    }
    if (typeof value == 'string' || typeof other == 'string') {
      value = baseToString(value);
      other = baseToString(other);
    } else {
      value = baseToNumber(value);
      other = baseToNumber(other);
    }
    result = operator(value, other);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sum"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sum (array)](#apidoc.element.cash.vorpal.lodash.sum)
- description and source-code
```javascript
function sum(array) {
  return (array && array.length)
    ? baseSum(array, identity)
    : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.sumBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>sumBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.sumBy)
- description and source-code
```javascript
function sumBy(array, iteratee) {
  return (array && array.length)
    ? baseSum(array, getIteratee(iteratee, 2))
    : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.tail"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>tail (array)](#apidoc.element.cash.vorpal.lodash.tail)
- description and source-code
```javascript
function tail(array) {
  var length = array == null ? 0 : array.length;
  return length ? baseSlice(array, 1, length) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.take"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>take (array, n, guard)](#apidoc.element.cash.vorpal.lodash.take)
- description and source-code
```javascript
function take(array, n, guard) {
  if (!(array && array.length)) {
    return [];
  }
  n = (guard || n === undefined) ? 1 : toInteger(n);
  return baseSlice(array, 0, n < 0 ? 0 : n);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.takeRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>takeRight (array, n, guard)](#apidoc.element.cash.vorpal.lodash.takeRight)
- description and source-code
```javascript
function takeRight(array, n, guard) {
  var length = array == null ? 0 : array.length;
  if (!length) {
    return [];
  }
  n = (guard || n === undefined) ? 1 : toInteger(n);
  n = length - n;
  return baseSlice(array, n < 0 ? 0 : n, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.takeRightWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>takeRightWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.takeRightWhile)
- description and source-code
```javascript
function takeRightWhile(array, predicate) {
  return (array && array.length)
    ? baseWhile(array, getIteratee(predicate, 3), false, true)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.takeWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>takeWhile (array, predicate)](#apidoc.element.cash.vorpal.lodash.takeWhile)
- description and source-code
```javascript
function takeWhile(array, predicate) {
  return (array && array.length)
    ? baseWhile(array, getIteratee(predicate, 3))
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.tap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>tap (value, interceptor)](#apidoc.element.cash.vorpal.lodash.tap)
- description and source-code
```javascript
function tap(value, interceptor) {
  interceptor(value);
  return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.template"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>template (string, options, guard)](#apidoc.element.cash.vorpal.lodash.template)
- description and source-code
```javascript
function template(string, options, guard) {
  // Based on John Resig's 'tmpl' implementation
  // (http://ejohn.org/blog/javascript-micro-templating/)
  // and Laura Doktorova's doT.js (https://github.com/olado/doT).
  var settings = lodash.templateSettings;

  if (guard && isIterateeCall(string, options, guard)) {
    options = undefined;
  }
  string = toString(string);
  options = assignInWith({}, options, settings, customDefaultsAssignIn);

  var imports = assignInWith({}, options.imports, settings.imports, customDefaultsAssignIn),
      importsKeys = keys(imports),
      importsValues = baseValues(imports, importsKeys);

  var isEscaping,
      isEvaluating,
      index = 0,
      interpolate = options.interpolate || reNoMatch,
      source = "__p += '";

  // Compile the regexp to match each delimiter.
  var reDelimiters = RegExp(
    (options.escape || reNoMatch).source + '|' +
    interpolate.source + '|' +
    (interpolate === reInterpolate ? reEsTemplate : reNoMatch).source + '|' +
    (options.evaluate || reNoMatch).source + '|$'
  , 'g');

  // Use a sourceURL for easier debugging.
  var sourceURL = '//# sourceURL=' +
    ('sourceURL' in options
      ? options.sourceURL
      : ('lodash.templateSources[' + (++templateCounter) + ']')
    ) + '\n';

  string.replace(reDelimiters, function(match, escapeValue, interpolateValue, esTemplateValue, evaluateValue, offset) {
    interpolateValue || (interpolateValue = esTemplateValue);

    // Escape characters that can't be included in string literals.
    source += string.slice(index, offset).replace(reUnescapedString, escapeStringChar);

    // Replace delimiters with snippets.
    if (escapeValue) {
      isEscaping = true;
      source += "' +\n__e(" + escapeValue + ") +\n'";
    }
    if (evaluateValue) {
      isEvaluating = true;
      source += "';\n" + evaluateValue + ";\n__p += '";
    }
    if (interpolateValue) {
      source += "' +\n((__t = (" + interpolateValue + ")) == null ? '' : __t) +\n'";
    }
    index = offset + match.length;

    // The JS engine embedded in Adobe products needs 'match' returned in
    // order to produce the correct 'offset' value.
    return match;
  });

  source += "';\n";

  // If 'variable' is not specified wrap a with-statement around the generated
  // code to add the data object to the top of the scope chain.
  var variable = options.variable;
  if (!variable) {
    source = 'with (obj) {\n' + source + '\n}\n';
  }
  // Cleanup code by stripping empty strings.
  source = (isEvaluating ? source.replace(reEmptyStringLeading, '') : source)
    .replace(reEmptyStringMiddle, '$1')
    .replace(reEmptyStringTrailing, '$1;');

  // Frame code as the function body.
  source = 'function(' + (variable || 'obj') + ') {\n' +
    (variable
      ? ''
      : 'obj || (obj = {});\n'
    ) +
    "var __t, __p = ''" +
    (isEscaping
       ? ', __e = _.escape'
       : ''
    ) +
    (isEvaluating
      ? ', __j = Array.prototype.join;\n' +
        "function print() { __p += __j.call(arguments, '') }\n"
      : ';\n'
    ) +
    source +
    'return __p\n}';

  var result = attempt(function() {
    return Function(importsKeys, sourceURL + 'return ' + source)
      .apply(undefined, importsValues);
  });

  // Provide the compiled function's source by its 'toString' method or
  // the 'source' property as a convenience for inlining compiled templates.
  result.source = source;
  if (isError(result)) {
    throw result;
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.throttle"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>throttle (func, wait, options)](#apidoc.element.cash.vorpal.lodash.throttle)
- description and source-code
```javascript
function throttle(func, wait, options) {
  var leading = true,
      trailing = true;

  if (typeof func != 'function') {
    throw new TypeError(FUNC_ERROR_TEXT);
  }
  if (isObject(options)) {
    leading = 'leading' in options ? !!options.leading : leading;
    trailing = 'trailing' in options ? !!options.trailing : trailing;
  }
  return debounce(func, wait, {
    'leading': leading,
    'maxWait': wait,
    'trailing': trailing
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.thru"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>thru (value, interceptor)](#apidoc.element.cash.vorpal.lodash.thru)
- description and source-code
```javascript
function thru(value, interceptor) {
  return interceptor(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.times"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>times (n, iteratee)](#apidoc.element.cash.vorpal.lodash.times)
- description and source-code
```javascript
function times(n, iteratee) {
  n = toInteger(n);
  if (n < 1 || n > MAX_SAFE_INTEGER) {
    return [];
  }
  var index = MAX_ARRAY_LENGTH,
      length = nativeMin(n, MAX_ARRAY_LENGTH);

  iteratee = getIteratee(iteratee);
  n -= MAX_ARRAY_LENGTH;

  var result = baseTimes(length, iteratee);
  while (++index < n) {
    iteratee(index);
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toArray (value)](#apidoc.element.cash.vorpal.lodash.toArray)
- description and source-code
```javascript
function toArray(value) {
  if (!value) {
    return [];
  }
  if (isArrayLike(value)) {
    return isString(value) ? stringToArray(value) : copyArray(value);
  }
  if (symIterator && value[symIterator]) {
    return iteratorToArray(value[symIterator]());
  }
  var tag = getTag(value),
      func = tag == mapTag ? mapToArray : (tag == setTag ? setToArray : values);

  return func(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toFinite"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toFinite (value)](#apidoc.element.cash.vorpal.lodash.toFinite)
- description and source-code
```javascript
function toFinite(value) {
  if (!value) {
    return value === 0 ? value : 0;
  }
  value = toNumber(value);
  if (value === INFINITY || value === -INFINITY) {
    var sign = (value < 0 ? -1 : 1);
    return sign * MAX_INTEGER;
  }
  return value === value ? value : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toInteger (value)](#apidoc.element.cash.vorpal.lodash.toInteger)
- description and source-code
```javascript
function toInteger(value) {
  var result = toFinite(value),
      remainder = result % 1;

  return result === result ? (remainder ? result - remainder : result) : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toLength"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toLength (value)](#apidoc.element.cash.vorpal.lodash.toLength)
- description and source-code
```javascript
function toLength(value) {
  return value ? baseClamp(toInteger(value), 0, MAX_ARRAY_LENGTH) : 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toLower"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toLower (value)](#apidoc.element.cash.vorpal.lodash.toLower)
- description and source-code
```javascript
function toLower(value) {
  return toString(value).toLowerCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toNumber"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toNumber (value)](#apidoc.element.cash.vorpal.lodash.toNumber)
- description and source-code
```javascript
function toNumber(value) {
  if (typeof value == 'number') {
    return value;
  }
  if (isSymbol(value)) {
    return NAN;
  }
  if (isObject(value)) {
    var other = typeof value.valueOf == 'function' ? value.valueOf() : value;
    value = isObject(other) ? (other + '') : other;
  }
  if (typeof value != 'string') {
    return value === 0 ? value : +value;
  }
  value = value.replace(reTrim, '');
  var isBinary = reIsBinary.test(value);
  return (isBinary || reIsOctal.test(value))
    ? freeParseInt(value.slice(2), isBinary ? 2 : 8)
    : (reIsBadHex.test(value) ? NAN : +value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toPairs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPairs (object)](#apidoc.element.cash.vorpal.lodash.toPairs)
- description and source-code
```javascript
toPairs = function (object) {
  var tag = getTag(object);
  if (tag == mapTag) {
    return mapToArray(object);
  }
  if (tag == setTag) {
    return setToPairs(object);
  }
  return baseToPairs(object, keysFunc(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toPairsIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPairsIn (object)](#apidoc.element.cash.vorpal.lodash.toPairsIn)
- description and source-code
```javascript
toPairsIn = function (object) {
  var tag = getTag(object);
  if (tag == mapTag) {
    return mapToArray(object);
  }
  if (tag == setTag) {
    return setToPairs(object);
  }
  return baseToPairs(object, keysFunc(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toPath"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPath (value)](#apidoc.element.cash.vorpal.lodash.toPath)
- description and source-code
```javascript
function toPath(value) {
  if (isArray(value)) {
    return arrayMap(value, toKey);
  }
  return isSymbol(value) ? [value] : copyArray(stringToPath(toString(value)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toPlainObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toPlainObject (value)](#apidoc.element.cash.vorpal.lodash.toPlainObject)
- description and source-code
```javascript
function toPlainObject(value) {
  return copyObject(value, keysIn(value));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toSafeInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toSafeInteger (value)](#apidoc.element.cash.vorpal.lodash.toSafeInteger)
- description and source-code
```javascript
function toSafeInteger(value) {
  return value
    ? baseClamp(toInteger(value), -MAX_SAFE_INTEGER, MAX_SAFE_INTEGER)
    : (value === 0 ? value : 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toString"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toString (value)](#apidoc.element.cash.vorpal.lodash.toString)
- description and source-code
```javascript
function toString(value) {
  return value == null ? '' : baseToString(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.toUpper"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>toUpper (value)](#apidoc.element.cash.vorpal.lodash.toUpper)
- description and source-code
```javascript
function toUpper(value) {
  return toString(value).toUpperCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.transform"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>transform (object, iteratee, accumulator)](#apidoc.element.cash.vorpal.lodash.transform)
- description and source-code
```javascript
function transform(object, iteratee, accumulator) {
  var isArr = isArray(object),
      isArrLike = isArr || isBuffer(object) || isTypedArray(object);

  iteratee = getIteratee(iteratee, 4);
  if (accumulator == null) {
    var Ctor = object && object.constructor;
    if (isArrLike) {
      accumulator = isArr ? new Ctor : [];
    }
    else if (isObject(object)) {
      accumulator = isFunction(Ctor) ? baseCreate(getPrototype(object)) : {};
    }
    else {
      accumulator = {};
    }
  }
  (isArrLike ? arrayEach : baseForOwn)(object, function(value, index, object) {
    return iteratee(accumulator, value, index, object);
  });
  return accumulator;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.trim"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>trim (string, chars, guard)](#apidoc.element.cash.vorpal.lodash.trim)
- description and source-code
```javascript
function trim(string, chars, guard) {
  string = toString(string);
  if (string && (guard || chars === undefined)) {
    return string.replace(reTrim, '');
  }
  if (!string || !(chars = baseToString(chars))) {
    return string;
  }
  var strSymbols = stringToArray(string),
      chrSymbols = stringToArray(chars),
      start = charsStartIndex(strSymbols, chrSymbols),
      end = charsEndIndex(strSymbols, chrSymbols) + 1;

  return castSlice(strSymbols, start, end).join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.trimEnd"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>trimEnd (string, chars, guard)](#apidoc.element.cash.vorpal.lodash.trimEnd)
- description and source-code
```javascript
function trimEnd(string, chars, guard) {
  string = toString(string);
  if (string && (guard || chars === undefined)) {
    return string.replace(reTrimEnd, '');
  }
  if (!string || !(chars = baseToString(chars))) {
    return string;
  }
  var strSymbols = stringToArray(string),
      end = charsEndIndex(strSymbols, stringToArray(chars)) + 1;

  return castSlice(strSymbols, 0, end).join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.trimStart"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>trimStart (string, chars, guard)](#apidoc.element.cash.vorpal.lodash.trimStart)
- description and source-code
```javascript
function trimStart(string, chars, guard) {
  string = toString(string);
  if (string && (guard || chars === undefined)) {
    return string.replace(reTrimStart, '');
  }
  if (!string || !(chars = baseToString(chars))) {
    return string;
  }
  var strSymbols = stringToArray(string),
      start = charsStartIndex(strSymbols, stringToArray(chars));

  return castSlice(strSymbols, start).join('');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.truncate"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>truncate (string, options)](#apidoc.element.cash.vorpal.lodash.truncate)
- description and source-code
```javascript
function truncate(string, options) {
  var length = DEFAULT_TRUNC_LENGTH,
      omission = DEFAULT_TRUNC_OMISSION;

  if (isObject(options)) {
    var separator = 'separator' in options ? options.separator : separator;
    length = 'length' in options ? toInteger(options.length) : length;
    omission = 'omission' in options ? baseToString(options.omission) : omission;
  }
  string = toString(string);

  var strLength = string.length;
  if (hasUnicode(string)) {
    var strSymbols = stringToArray(string);
    strLength = strSymbols.length;
  }
  if (length >= strLength) {
    return string;
  }
  var end = length - stringSize(omission);
  if (end < 1) {
    return omission;
  }
  var result = strSymbols
    ? castSlice(strSymbols, 0, end).join('')
    : string.slice(0, end);

  if (separator === undefined) {
    return result + omission;
  }
  if (strSymbols) {
    end += (result.length - end);
  }
  if (isRegExp(separator)) {
    if (string.slice(end).search(separator)) {
      var match,
          substring = result;

      if (!separator.global) {
        separator = RegExp(separator.source, toString(reFlags.exec(separator)) + 'g');
      }
      separator.lastIndex = 0;
      while ((match = separator.exec(substring))) {
        var newEnd = match.index;
      }
      result = result.slice(0, newEnd === undefined ? end : newEnd);
    }
  } else if (string.indexOf(baseToString(separator), end) != end) {
    var index = result.lastIndexOf(separator);
    if (index > -1) {
      result = result.slice(0, index);
    }
  }
  return result + omission;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unary"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unary (func)](#apidoc.element.cash.vorpal.lodash.unary)
- description and source-code
```javascript
function unary(func) {
  return ary(func, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unescape"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unescape (string)](#apidoc.element.cash.vorpal.lodash.unescape)
- description and source-code
```javascript
function unescape(string) {
  string = toString(string);
  return (string && reHasEscapedHtml.test(string))
    ? string.replace(reEscapedHtml, unescapeHtmlChar)
    : string;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.union"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>union (arrays)](#apidoc.element.cash.vorpal.lodash.union)
- description and source-code
```javascript
union = function (arrays) {
  return baseUniq(baseFlatten(arrays, 1, isArrayLikeObject, true));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unionBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unionBy (arrays)](#apidoc.element.cash.vorpal.lodash.unionBy)
- description and source-code
```javascript
unionBy = function (arrays) {
  var iteratee = last(arrays);
  if (isArrayLikeObject(iteratee)) {
    iteratee = undefined;
  }
  return baseUniq(baseFlatten(arrays, 1, isArrayLikeObject, true), getIteratee(iteratee, 2));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unionWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unionWith (arrays)](#apidoc.element.cash.vorpal.lodash.unionWith)
- description and source-code
```javascript
unionWith = function (arrays) {
  var comparator = last(arrays);
  comparator = typeof comparator == 'function' ? comparator : undefined;
  return baseUniq(baseFlatten(arrays, 1, isArrayLikeObject, true), undefined, comparator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.uniq"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniq (array)](#apidoc.element.cash.vorpal.lodash.uniq)
- description and source-code
```javascript
function uniq(array) {
  return (array && array.length) ? baseUniq(array) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.uniqBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniqBy (array, iteratee)](#apidoc.element.cash.vorpal.lodash.uniqBy)
- description and source-code
```javascript
function uniqBy(array, iteratee) {
  return (array && array.length) ? baseUniq(array, getIteratee(iteratee, 2)) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.uniqWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniqWith (array, comparator)](#apidoc.element.cash.vorpal.lodash.uniqWith)
- description and source-code
```javascript
function uniqWith(array, comparator) {
  comparator = typeof comparator == 'function' ? comparator : undefined;
  return (array && array.length) ? baseUniq(array, undefined, comparator) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.uniqueId"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>uniqueId (prefix)](#apidoc.element.cash.vorpal.lodash.uniqueId)
- description and source-code
```javascript
function uniqueId(prefix) {
  var id = ++idCounter;
  return toString(prefix) + id;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unset"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unset (object, path)](#apidoc.element.cash.vorpal.lodash.unset)
- description and source-code
```javascript
function unset(object, path) {
  return object == null ? true : baseUnset(object, path);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unzip"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unzip (array)](#apidoc.element.cash.vorpal.lodash.unzip)
- description and source-code
```javascript
function unzip(array) {
  if (!(array && array.length)) {
    return [];
  }
  var length = 0;
  array = arrayFilter(array, function(group) {
    if (isArrayLikeObject(group)) {
      length = nativeMax(group.length, length);
      return true;
    }
  });
  return baseTimes(length, function(index) {
    return arrayMap(array, baseProperty(index));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.unzipWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>unzipWith (array, iteratee)](#apidoc.element.cash.vorpal.lodash.unzipWith)
- description and source-code
```javascript
function unzipWith(array, iteratee) {
  if (!(array && array.length)) {
    return [];
  }
  var result = unzip(array);
  if (iteratee == null) {
    return result;
  }
  return arrayMap(result, function(group) {
    return apply(iteratee, undefined, group);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.update"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>update (object, path, updater)](#apidoc.element.cash.vorpal.lodash.update)
- description and source-code
```javascript
function update(object, path, updater) {
  return object == null ? object : baseUpdate(object, path, castFunction(updater));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.updateWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>updateWith (object, path, updater, customizer)](#apidoc.element.cash.vorpal.lodash.updateWith)
- description and source-code
```javascript
function updateWith(object, path, updater, customizer) {
  customizer = typeof customizer == 'function' ? customizer : undefined;
  return object == null ? object : baseUpdate(object, path, castFunction(updater), customizer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.upperCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>upperCase (string)](#apidoc.element.cash.vorpal.lodash.upperCase)
- description and source-code
```javascript
upperCase = function (string) {
  return arrayReduce(words(deburr(string).replace(reApos, '')), callback, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.upperFirst"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>upperFirst (string)](#apidoc.element.cash.vorpal.lodash.upperFirst)
- description and source-code
```javascript
upperFirst = function (string) {
  string = toString(string);

  var strSymbols = hasUnicode(string)
    ? stringToArray(string)
    : undefined;

  var chr = strSymbols
    ? strSymbols[0]
    : string.charAt(0);

  var trailing = strSymbols
    ? castSlice(strSymbols, 1).join('')
    : string.slice(1);

  return chr[methodName]() + trailing;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.values"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>values (object)](#apidoc.element.cash.vorpal.lodash.values)
- description and source-code
```javascript
function values(object) {
  return object == null ? [] : baseValues(object, keys(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.valuesIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>valuesIn (object)](#apidoc.element.cash.vorpal.lodash.valuesIn)
- description and source-code
```javascript
function valuesIn(object) {
  return object == null ? [] : baseValues(object, keysIn(object));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.without"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>without (array, values)](#apidoc.element.cash.vorpal.lodash.without)
- description and source-code
```javascript
without = function (array, values) {
  return isArrayLikeObject(array)
    ? baseDifference(array, values)
    : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.words"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>words (string, pattern, guard)](#apidoc.element.cash.vorpal.lodash.words)
- description and source-code
```javascript
function words(string, pattern, guard) {
  string = toString(string);
  pattern = guard ? undefined : pattern;

  if (pattern === undefined) {
    return hasUnicodeWord(string) ? unicodeWords(string) : asciiWords(string);
  }
  return string.match(pattern) || [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.wrap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>wrap (value, wrapper)](#apidoc.element.cash.vorpal.lodash.wrap)
- description and source-code
```javascript
function wrap(value, wrapper) {
  return partial(castFunction(wrapper), value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.xor"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>xor (arrays)](#apidoc.element.cash.vorpal.lodash.xor)
- description and source-code
```javascript
xor = function (arrays) {
  return baseXor(arrayFilter(arrays, isArrayLikeObject));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.xorBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>xorBy (arrays)](#apidoc.element.cash.vorpal.lodash.xorBy)
- description and source-code
```javascript
xorBy = function (arrays) {
  var iteratee = last(arrays);
  if (isArrayLikeObject(iteratee)) {
    iteratee = undefined;
  }
  return baseXor(arrayFilter(arrays, isArrayLikeObject), getIteratee(iteratee, 2));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.xorWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>xorWith (arrays)](#apidoc.element.cash.vorpal.lodash.xorWith)
- description and source-code
```javascript
xorWith = function (arrays) {
  var comparator = last(arrays);
  comparator = typeof comparator == 'function' ? comparator : undefined;
  return baseXor(arrayFilter(arrays, isArrayLikeObject), undefined, comparator);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.zip"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zip (array)](#apidoc.element.cash.vorpal.lodash.zip)
- description and source-code
```javascript
function unzip(array) {
  if (!(array && array.length)) {
    return [];
  }
  var length = 0;
  array = arrayFilter(array, function(group) {
    if (isArrayLikeObject(group)) {
      length = nativeMax(group.length, length);
      return true;
    }
  });
  return baseTimes(length, function(index) {
    return arrayMap(array, baseProperty(index));
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.zipObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zipObject (props, values)](#apidoc.element.cash.vorpal.lodash.zipObject)
- description and source-code
```javascript
function zipObject(props, values) {
  return baseZipObject(props || [], values || [], assignValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.zipObjectDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zipObjectDeep (props, values)](#apidoc.element.cash.vorpal.lodash.zipObjectDeep)
- description and source-code
```javascript
function zipObjectDeep(props, values) {
  return baseZipObject(props || [], values || [], baseSet);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.zipWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.</span>zipWith (arrays)](#apidoc.element.cash.vorpal.lodash.zipWith)
- description and source-code
```javascript
zipWith = function (arrays) {
  var length = arrays.length,
      iteratee = length > 1 ? arrays[length - 1] : undefined;

  iteratee = typeof iteratee == 'function' ? (arrays.pop(), iteratee) : undefined;
  return unzipWith(arrays, iteratee);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.lodash.prototype"></a>[module cash.vorpal.lodash.prototype](#apidoc.module.cash.vorpal.lodash.prototype)

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.add"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>add ()](#apidoc.element.cash.vorpal.lodash.prototype.add)
- description and source-code
```javascript
add = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.after"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>after ()](#apidoc.element.cash.vorpal.lodash.prototype.after)
- description and source-code
```javascript
after = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.ary"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>ary ()](#apidoc.element.cash.vorpal.lodash.prototype.ary)
- description and source-code
```javascript
ary = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.assign"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assign ()](#apidoc.element.cash.vorpal.lodash.prototype.assign)
- description and source-code
```javascript
assign = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.assignIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assignIn ()](#apidoc.element.cash.vorpal.lodash.prototype.assignIn)
- description and source-code
```javascript
assignIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.assignInWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assignInWith ()](#apidoc.element.cash.vorpal.lodash.prototype.assignInWith)
- description and source-code
```javascript
assignInWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.assignWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>assignWith ()](#apidoc.element.cash.vorpal.lodash.prototype.assignWith)
- description and source-code
```javascript
assignWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.at"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>at (paths)](#apidoc.element.cash.vorpal.lodash.prototype.at)
- description and source-code
```javascript
at = function (paths) {
  var length = paths.length,
      start = length ? paths[0] : 0,
      value = this.__wrapped__,
      interceptor = function(object) { return baseAt(object, paths); };

  if (length > 1 || this.__actions__.length ||
      !(value instanceof LazyWrapper) || !isIndex(start)) {
    return this.thru(interceptor);
  }
  value = value.slice(start, +start + (length ? 1 : 0));
  value.__actions__.push({
    'func': thru,
    'args': [interceptor],
    'thisArg': undefined
  });
  return new LodashWrapper(value, this.__chain__).thru(function(array) {
    if (length && !array.length) {
      array.push(undefined);
    }
    return array;
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.attempt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>attempt ()](#apidoc.element.cash.vorpal.lodash.prototype.attempt)
- description and source-code
```javascript
attempt = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.before"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>before ()](#apidoc.element.cash.vorpal.lodash.prototype.before)
- description and source-code
```javascript
before = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.bind"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>bind ()](#apidoc.element.cash.vorpal.lodash.prototype.bind)
- description and source-code
```javascript
bind = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.bindAll"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>bindAll ()](#apidoc.element.cash.vorpal.lodash.prototype.bindAll)
- description and source-code
```javascript
bindAll = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.bindKey"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>bindKey ()](#apidoc.element.cash.vorpal.lodash.prototype.bindKey)
- description and source-code
```javascript
bindKey = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.camelCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>camelCase ()](#apidoc.element.cash.vorpal.lodash.prototype.camelCase)
- description and source-code
```javascript
camelCase = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.capitalize"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>capitalize ()](#apidoc.element.cash.vorpal.lodash.prototype.capitalize)
- description and source-code
```javascript
capitalize = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.castArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>castArray ()](#apidoc.element.cash.vorpal.lodash.prototype.castArray)
- description and source-code
```javascript
castArray = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.ceil"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>ceil ()](#apidoc.element.cash.vorpal.lodash.prototype.ceil)
- description and source-code
```javascript
ceil = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.chain"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>chain ()](#apidoc.element.cash.vorpal.lodash.prototype.chain)
- description and source-code
```javascript
function wrapperChain() {
  return chain(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.chunk"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>chunk ()](#apidoc.element.cash.vorpal.lodash.prototype.chunk)
- description and source-code
```javascript
chunk = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.clamp"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>clamp ()](#apidoc.element.cash.vorpal.lodash.prototype.clamp)
- description and source-code
```javascript
clamp = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.clone"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>clone ()](#apidoc.element.cash.vorpal.lodash.prototype.clone)
- description and source-code
```javascript
clone = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.cloneDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cloneDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.cloneDeep)
- description and source-code
```javascript
cloneDeep = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.cloneDeepWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cloneDeepWith ()](#apidoc.element.cash.vorpal.lodash.prototype.cloneDeepWith)
- description and source-code
```javascript
cloneDeepWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.cloneWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cloneWith ()](#apidoc.element.cash.vorpal.lodash.prototype.cloneWith)
- description and source-code
```javascript
cloneWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.commit"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>commit ()](#apidoc.element.cash.vorpal.lodash.prototype.commit)
- description and source-code
```javascript
function wrapperCommit() {
  return new LodashWrapper(this.value(), this.__chain__);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.compact"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>compact ()](#apidoc.element.cash.vorpal.lodash.prototype.compact)
- description and source-code
```javascript
compact = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.concat"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>concat ()](#apidoc.element.cash.vorpal.lodash.prototype.concat)
- description and source-code
```javascript
concat = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.cond"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>cond ()](#apidoc.element.cash.vorpal.lodash.prototype.cond)
- description and source-code
```javascript
cond = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.conforms"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>conforms ()](#apidoc.element.cash.vorpal.lodash.prototype.conforms)
- description and source-code
```javascript
conforms = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.conformsTo"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>conformsTo ()](#apidoc.element.cash.vorpal.lodash.prototype.conformsTo)
- description and source-code
```javascript
conformsTo = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.constant"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>constant ()](#apidoc.element.cash.vorpal.lodash.prototype.constant)
- description and source-code
```javascript
constant = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.countBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>countBy ()](#apidoc.element.cash.vorpal.lodash.prototype.countBy)
- description and source-code
```javascript
countBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.create"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>create ()](#apidoc.element.cash.vorpal.lodash.prototype.create)
- description and source-code
```javascript
create = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.curry"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>curry ()](#apidoc.element.cash.vorpal.lodash.prototype.curry)
- description and source-code
```javascript
curry = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.curryRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>curryRight ()](#apidoc.element.cash.vorpal.lodash.prototype.curryRight)
- description and source-code
```javascript
curryRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.debounce"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>debounce ()](#apidoc.element.cash.vorpal.lodash.prototype.debounce)
- description and source-code
```javascript
debounce = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.deburr"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>deburr ()](#apidoc.element.cash.vorpal.lodash.prototype.deburr)
- description and source-code
```javascript
deburr = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.defaultTo"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defaultTo ()](#apidoc.element.cash.vorpal.lodash.prototype.defaultTo)
- description and source-code
```javascript
defaultTo = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.defaults"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defaults ()](#apidoc.element.cash.vorpal.lodash.prototype.defaults)
- description and source-code
```javascript
defaults = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.defaultsDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defaultsDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.defaultsDeep)
- description and source-code
```javascript
defaultsDeep = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.defer"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>defer ()](#apidoc.element.cash.vorpal.lodash.prototype.defer)
- description and source-code
```javascript
defer = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.delay"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>delay ()](#apidoc.element.cash.vorpal.lodash.prototype.delay)
- description and source-code
```javascript
delay = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.difference"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>difference ()](#apidoc.element.cash.vorpal.lodash.prototype.difference)
- description and source-code
```javascript
difference = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.differenceBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>differenceBy ()](#apidoc.element.cash.vorpal.lodash.prototype.differenceBy)
- description and source-code
```javascript
differenceBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.differenceWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>differenceWith ()](#apidoc.element.cash.vorpal.lodash.prototype.differenceWith)
- description and source-code
```javascript
differenceWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.divide"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>divide ()](#apidoc.element.cash.vorpal.lodash.prototype.divide)
- description and source-code
```javascript
divide = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.drop"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>drop ()](#apidoc.element.cash.vorpal.lodash.prototype.drop)
- description and source-code
```javascript
drop = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.dropRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>dropRight ()](#apidoc.element.cash.vorpal.lodash.prototype.dropRight)
- description and source-code
```javascript
dropRight = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.dropRightWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>dropRightWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.dropRightWhile)
- description and source-code
```javascript
dropRightWhile = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.dropWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>dropWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.dropWhile)
- description and source-code
```javascript
dropWhile = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.each"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>each ()](#apidoc.element.cash.vorpal.lodash.prototype.each)
- description and source-code
```javascript
each = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.eachRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>eachRight ()](#apidoc.element.cash.vorpal.lodash.prototype.eachRight)
- description and source-code
```javascript
eachRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.endsWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>endsWith ()](#apidoc.element.cash.vorpal.lodash.prototype.endsWith)
- description and source-code
```javascript
endsWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.entries"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>entries ()](#apidoc.element.cash.vorpal.lodash.prototype.entries)
- description and source-code
```javascript
entries = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.entriesIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>entriesIn ()](#apidoc.element.cash.vorpal.lodash.prototype.entriesIn)
- description and source-code
```javascript
entriesIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.eq"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>eq ()](#apidoc.element.cash.vorpal.lodash.prototype.eq)
- description and source-code
```javascript
eq = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.escape"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>escape ()](#apidoc.element.cash.vorpal.lodash.prototype.escape)
- description and source-code
```javascript
escape = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.escapeRegExp"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>escapeRegExp ()](#apidoc.element.cash.vorpal.lodash.prototype.escapeRegExp)
- description and source-code
```javascript
escapeRegExp = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.every"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>every ()](#apidoc.element.cash.vorpal.lodash.prototype.every)
- description and source-code
```javascript
every = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.extend"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>extend ()](#apidoc.element.cash.vorpal.lodash.prototype.extend)
- description and source-code
```javascript
extend = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.extendWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>extendWith ()](#apidoc.element.cash.vorpal.lodash.prototype.extendWith)
- description and source-code
```javascript
extendWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.fill"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>fill ()](#apidoc.element.cash.vorpal.lodash.prototype.fill)
- description and source-code
```javascript
fill = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.filter"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>filter ()](#apidoc.element.cash.vorpal.lodash.prototype.filter)
- description and source-code
```javascript
filter = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.find"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>find ()](#apidoc.element.cash.vorpal.lodash.prototype.find)
- description and source-code
```javascript
find = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.findIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.findIndex)
- description and source-code
```javascript
findIndex = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.findKey"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findKey ()](#apidoc.element.cash.vorpal.lodash.prototype.findKey)
- description and source-code
```javascript
findKey = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.findLast"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findLast ()](#apidoc.element.cash.vorpal.lodash.prototype.findLast)
- description and source-code
```javascript
findLast = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.findLastIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findLastIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.findLastIndex)
- description and source-code
```javascript
findLastIndex = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.findLastKey"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>findLastKey ()](#apidoc.element.cash.vorpal.lodash.prototype.findLastKey)
- description and source-code
```javascript
findLastKey = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.first"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>first ()](#apidoc.element.cash.vorpal.lodash.prototype.first)
- description and source-code
```javascript
first = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flatMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatMap ()](#apidoc.element.cash.vorpal.lodash.prototype.flatMap)
- description and source-code
```javascript
flatMap = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flatMapDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatMapDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.flatMapDeep)
- description and source-code
```javascript
flatMapDeep = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flatMapDepth"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatMapDepth ()](#apidoc.element.cash.vorpal.lodash.prototype.flatMapDepth)
- description and source-code
```javascript
flatMapDepth = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flatten"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flatten ()](#apidoc.element.cash.vorpal.lodash.prototype.flatten)
- description and source-code
```javascript
flatten = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flattenDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flattenDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.flattenDeep)
- description and source-code
```javascript
flattenDeep = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flattenDepth"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flattenDepth ()](#apidoc.element.cash.vorpal.lodash.prototype.flattenDepth)
- description and source-code
```javascript
flattenDepth = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flip"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flip ()](#apidoc.element.cash.vorpal.lodash.prototype.flip)
- description and source-code
```javascript
flip = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.floor"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>floor ()](#apidoc.element.cash.vorpal.lodash.prototype.floor)
- description and source-code
```javascript
floor = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flow"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flow ()](#apidoc.element.cash.vorpal.lodash.prototype.flow)
- description and source-code
```javascript
flow = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.flowRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>flowRight ()](#apidoc.element.cash.vorpal.lodash.prototype.flowRight)
- description and source-code
```javascript
flowRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.forEach"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forEach ()](#apidoc.element.cash.vorpal.lodash.prototype.forEach)
- description and source-code
```javascript
forEach = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.forEachRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forEachRight ()](#apidoc.element.cash.vorpal.lodash.prototype.forEachRight)
- description and source-code
```javascript
forEachRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.forIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forIn ()](#apidoc.element.cash.vorpal.lodash.prototype.forIn)
- description and source-code
```javascript
forIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.forInRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forInRight ()](#apidoc.element.cash.vorpal.lodash.prototype.forInRight)
- description and source-code
```javascript
forInRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.forOwn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forOwn ()](#apidoc.element.cash.vorpal.lodash.prototype.forOwn)
- description and source-code
```javascript
forOwn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.forOwnRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>forOwnRight ()](#apidoc.element.cash.vorpal.lodash.prototype.forOwnRight)
- description and source-code
```javascript
forOwnRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.fromPairs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>fromPairs ()](#apidoc.element.cash.vorpal.lodash.prototype.fromPairs)
- description and source-code
```javascript
fromPairs = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.functions"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>functions ()](#apidoc.element.cash.vorpal.lodash.prototype.functions)
- description and source-code
```javascript
functions = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.functionsIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>functionsIn ()](#apidoc.element.cash.vorpal.lodash.prototype.functionsIn)
- description and source-code
```javascript
functionsIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.get"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>get ()](#apidoc.element.cash.vorpal.lodash.prototype.get)
- description and source-code
```javascript
get = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.groupBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>groupBy ()](#apidoc.element.cash.vorpal.lodash.prototype.groupBy)
- description and source-code
```javascript
groupBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.gt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>gt ()](#apidoc.element.cash.vorpal.lodash.prototype.gt)
- description and source-code
```javascript
gt = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.gte"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>gte ()](#apidoc.element.cash.vorpal.lodash.prototype.gte)
- description and source-code
```javascript
gte = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.has"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>has ()](#apidoc.element.cash.vorpal.lodash.prototype.has)
- description and source-code
```javascript
has = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.hasIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>hasIn ()](#apidoc.element.cash.vorpal.lodash.prototype.hasIn)
- description and source-code
```javascript
hasIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.head"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>head ()](#apidoc.element.cash.vorpal.lodash.prototype.head)
- description and source-code
```javascript
head = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.identity"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>identity ()](#apidoc.element.cash.vorpal.lodash.prototype.identity)
- description and source-code
```javascript
identity = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.inRange"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>inRange ()](#apidoc.element.cash.vorpal.lodash.prototype.inRange)
- description and source-code
```javascript
inRange = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.includes"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>includes ()](#apidoc.element.cash.vorpal.lodash.prototype.includes)
- description and source-code
```javascript
includes = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>indexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.indexOf)
- description and source-code
```javascript
indexOf = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.initial"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>initial ()](#apidoc.element.cash.vorpal.lodash.prototype.initial)
- description and source-code
```javascript
initial = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.intersection"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>intersection ()](#apidoc.element.cash.vorpal.lodash.prototype.intersection)
- description and source-code
```javascript
intersection = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.intersectionBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>intersectionBy ()](#apidoc.element.cash.vorpal.lodash.prototype.intersectionBy)
- description and source-code
```javascript
intersectionBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.intersectionWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>intersectionWith ()](#apidoc.element.cash.vorpal.lodash.prototype.intersectionWith)
- description and source-code
```javascript
intersectionWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.invert"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invert ()](#apidoc.element.cash.vorpal.lodash.prototype.invert)
- description and source-code
```javascript
invert = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.invertBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invertBy ()](#apidoc.element.cash.vorpal.lodash.prototype.invertBy)
- description and source-code
```javascript
invertBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.invoke"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invoke ()](#apidoc.element.cash.vorpal.lodash.prototype.invoke)
- description and source-code
```javascript
invoke = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.invokeMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>invokeMap ()](#apidoc.element.cash.vorpal.lodash.prototype.invokeMap)
- description and source-code
```javascript
invokeMap = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isArguments"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArguments ()](#apidoc.element.cash.vorpal.lodash.prototype.isArguments)
- description and source-code
```javascript
isArguments = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArray ()](#apidoc.element.cash.vorpal.lodash.prototype.isArray)
- description and source-code
```javascript
isArray = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isArrayBuffer"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArrayBuffer ()](#apidoc.element.cash.vorpal.lodash.prototype.isArrayBuffer)
- description and source-code
```javascript
isArrayBuffer = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isArrayLike"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArrayLike ()](#apidoc.element.cash.vorpal.lodash.prototype.isArrayLike)
- description and source-code
```javascript
isArrayLike = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isArrayLikeObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isArrayLikeObject ()](#apidoc.element.cash.vorpal.lodash.prototype.isArrayLikeObject)
- description and source-code
```javascript
isArrayLikeObject = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isBoolean"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isBoolean ()](#apidoc.element.cash.vorpal.lodash.prototype.isBoolean)
- description and source-code
```javascript
isBoolean = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isBuffer"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isBuffer ()](#apidoc.element.cash.vorpal.lodash.prototype.isBuffer)
- description and source-code
```javascript
isBuffer = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isDate"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isDate ()](#apidoc.element.cash.vorpal.lodash.prototype.isDate)
- description and source-code
```javascript
isDate = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isElement"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isElement ()](#apidoc.element.cash.vorpal.lodash.prototype.isElement)
- description and source-code
```javascript
isElement = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isEmpty ()](#apidoc.element.cash.vorpal.lodash.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isEqual"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isEqual ()](#apidoc.element.cash.vorpal.lodash.prototype.isEqual)
- description and source-code
```javascript
isEqual = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isEqualWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isEqualWith ()](#apidoc.element.cash.vorpal.lodash.prototype.isEqualWith)
- description and source-code
```javascript
isEqualWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isError"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isError ()](#apidoc.element.cash.vorpal.lodash.prototype.isError)
- description and source-code
```javascript
isError = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isFinite"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isFinite ()](#apidoc.element.cash.vorpal.lodash.prototype.isFinite)
- description and source-code
```javascript
isFinite = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isFunction"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isFunction ()](#apidoc.element.cash.vorpal.lodash.prototype.isFunction)
- description and source-code
```javascript
isFunction = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.isInteger)
- description and source-code
```javascript
isInteger = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isLength"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isLength ()](#apidoc.element.cash.vorpal.lodash.prototype.isLength)
- description and source-code
```javascript
isLength = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isMap ()](#apidoc.element.cash.vorpal.lodash.prototype.isMap)
- description and source-code
```javascript
isMap = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isMatch"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isMatch ()](#apidoc.element.cash.vorpal.lodash.prototype.isMatch)
- description and source-code
```javascript
isMatch = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isMatchWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isMatchWith ()](#apidoc.element.cash.vorpal.lodash.prototype.isMatchWith)
- description and source-code
```javascript
isMatchWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isNaN"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNaN ()](#apidoc.element.cash.vorpal.lodash.prototype.isNaN)
- description and source-code
```javascript
isNaN = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isNative"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNative ()](#apidoc.element.cash.vorpal.lodash.prototype.isNative)
- description and source-code
```javascript
isNative = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isNil"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNil ()](#apidoc.element.cash.vorpal.lodash.prototype.isNil)
- description and source-code
```javascript
isNil = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isNull"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNull ()](#apidoc.element.cash.vorpal.lodash.prototype.isNull)
- description and source-code
```javascript
isNull = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isNumber"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isNumber ()](#apidoc.element.cash.vorpal.lodash.prototype.isNumber)
- description and source-code
```javascript
isNumber = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isObject ()](#apidoc.element.cash.vorpal.lodash.prototype.isObject)
- description and source-code
```javascript
isObject = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isObjectLike"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isObjectLike ()](#apidoc.element.cash.vorpal.lodash.prototype.isObjectLike)
- description and source-code
```javascript
isObjectLike = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isPlainObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isPlainObject ()](#apidoc.element.cash.vorpal.lodash.prototype.isPlainObject)
- description and source-code
```javascript
isPlainObject = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isRegExp"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isRegExp ()](#apidoc.element.cash.vorpal.lodash.prototype.isRegExp)
- description and source-code
```javascript
isRegExp = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isSafeInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isSafeInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.isSafeInteger)
- description and source-code
```javascript
isSafeInteger = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isSet"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isSet ()](#apidoc.element.cash.vorpal.lodash.prototype.isSet)
- description and source-code
```javascript
isSet = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isString"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isString ()](#apidoc.element.cash.vorpal.lodash.prototype.isString)
- description and source-code
```javascript
isString = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isSymbol"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isSymbol ()](#apidoc.element.cash.vorpal.lodash.prototype.isSymbol)
- description and source-code
```javascript
isSymbol = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isTypedArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isTypedArray ()](#apidoc.element.cash.vorpal.lodash.prototype.isTypedArray)
- description and source-code
```javascript
isTypedArray = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isUndefined"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isUndefined ()](#apidoc.element.cash.vorpal.lodash.prototype.isUndefined)
- description and source-code
```javascript
isUndefined = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isWeakMap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isWeakMap ()](#apidoc.element.cash.vorpal.lodash.prototype.isWeakMap)
- description and source-code
```javascript
isWeakMap = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.isWeakSet"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>isWeakSet ()](#apidoc.element.cash.vorpal.lodash.prototype.isWeakSet)
- description and source-code
```javascript
isWeakSet = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.iteratee"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>iteratee ()](#apidoc.element.cash.vorpal.lodash.prototype.iteratee)
- description and source-code
```javascript
iteratee = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.join"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>join ()](#apidoc.element.cash.vorpal.lodash.prototype.join)
- description and source-code
```javascript
join = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.kebabCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>kebabCase ()](#apidoc.element.cash.vorpal.lodash.prototype.kebabCase)
- description and source-code
```javascript
kebabCase = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.keyBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>keyBy ()](#apidoc.element.cash.vorpal.lodash.prototype.keyBy)
- description and source-code
```javascript
keyBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.keys"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>keys ()](#apidoc.element.cash.vorpal.lodash.prototype.keys)
- description and source-code
```javascript
keys = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.keysIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>keysIn ()](#apidoc.element.cash.vorpal.lodash.prototype.keysIn)
- description and source-code
```javascript
keysIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.last"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>last ()](#apidoc.element.cash.vorpal.lodash.prototype.last)
- description and source-code
```javascript
last = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lastIndexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.lastIndexOf)
- description and source-code
```javascript
lastIndexOf = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.lowerCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lowerCase ()](#apidoc.element.cash.vorpal.lodash.prototype.lowerCase)
- description and source-code
```javascript
lowerCase = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.lowerFirst"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lowerFirst ()](#apidoc.element.cash.vorpal.lodash.prototype.lowerFirst)
- description and source-code
```javascript
lowerFirst = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.lt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lt ()](#apidoc.element.cash.vorpal.lodash.prototype.lt)
- description and source-code
```javascript
lt = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.lte"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>lte ()](#apidoc.element.cash.vorpal.lodash.prototype.lte)
- description and source-code
```javascript
lte = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.map"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>map ()](#apidoc.element.cash.vorpal.lodash.prototype.map)
- description and source-code
```javascript
map = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.mapKeys"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mapKeys ()](#apidoc.element.cash.vorpal.lodash.prototype.mapKeys)
- description and source-code
```javascript
mapKeys = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.mapValues"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mapValues ()](#apidoc.element.cash.vorpal.lodash.prototype.mapValues)
- description and source-code
```javascript
mapValues = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.matches"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>matches ()](#apidoc.element.cash.vorpal.lodash.prototype.matches)
- description and source-code
```javascript
matches = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.matchesProperty"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>matchesProperty ()](#apidoc.element.cash.vorpal.lodash.prototype.matchesProperty)
- description and source-code
```javascript
matchesProperty = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.max"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>max ()](#apidoc.element.cash.vorpal.lodash.prototype.max)
- description and source-code
```javascript
max = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.maxBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>maxBy ()](#apidoc.element.cash.vorpal.lodash.prototype.maxBy)
- description and source-code
```javascript
maxBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.mean"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mean ()](#apidoc.element.cash.vorpal.lodash.prototype.mean)
- description and source-code
```javascript
mean = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.meanBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>meanBy ()](#apidoc.element.cash.vorpal.lodash.prototype.meanBy)
- description and source-code
```javascript
meanBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.memoize"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>memoize ()](#apidoc.element.cash.vorpal.lodash.prototype.memoize)
- description and source-code
```javascript
memoize = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.merge"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>merge ()](#apidoc.element.cash.vorpal.lodash.prototype.merge)
- description and source-code
```javascript
merge = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.mergeWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mergeWith ()](#apidoc.element.cash.vorpal.lodash.prototype.mergeWith)
- description and source-code
```javascript
mergeWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.method"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>method ()](#apidoc.element.cash.vorpal.lodash.prototype.method)
- description and source-code
```javascript
method = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.methodOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>methodOf ()](#apidoc.element.cash.vorpal.lodash.prototype.methodOf)
- description and source-code
```javascript
methodOf = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.min"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>min ()](#apidoc.element.cash.vorpal.lodash.prototype.min)
- description and source-code
```javascript
min = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.minBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>minBy ()](#apidoc.element.cash.vorpal.lodash.prototype.minBy)
- description and source-code
```javascript
minBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.mixin"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>mixin ()](#apidoc.element.cash.vorpal.lodash.prototype.mixin)
- description and source-code
```javascript
mixin = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.multiply"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>multiply ()](#apidoc.element.cash.vorpal.lodash.prototype.multiply)
- description and source-code
```javascript
multiply = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.negate"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>negate ()](#apidoc.element.cash.vorpal.lodash.prototype.negate)
- description and source-code
```javascript
negate = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.next"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>next ()](#apidoc.element.cash.vorpal.lodash.prototype.next)
- description and source-code
```javascript
function wrapperNext() {
  if (this.__values__ === undefined) {
    this.__values__ = toArray(this.value());
  }
  var done = this.__index__ >= this.__values__.length,
      value = done ? undefined : this.__values__[this.__index__++];

  return { 'done': done, 'value': value };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.noConflict"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>noConflict ()](#apidoc.element.cash.vorpal.lodash.prototype.noConflict)
- description and source-code
```javascript
noConflict = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.noop"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>noop ()](#apidoc.element.cash.vorpal.lodash.prototype.noop)
- description and source-code
```javascript
noop = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.now"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>now ()](#apidoc.element.cash.vorpal.lodash.prototype.now)
- description and source-code
```javascript
now = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.nth"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>nth ()](#apidoc.element.cash.vorpal.lodash.prototype.nth)
- description and source-code
```javascript
nth = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.nthArg"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>nthArg ()](#apidoc.element.cash.vorpal.lodash.prototype.nthArg)
- description and source-code
```javascript
nthArg = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.omit"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>omit ()](#apidoc.element.cash.vorpal.lodash.prototype.omit)
- description and source-code
```javascript
omit = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.omitBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>omitBy ()](#apidoc.element.cash.vorpal.lodash.prototype.omitBy)
- description and source-code
```javascript
omitBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.once"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>once ()](#apidoc.element.cash.vorpal.lodash.prototype.once)
- description and source-code
```javascript
once = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.orderBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>orderBy ()](#apidoc.element.cash.vorpal.lodash.prototype.orderBy)
- description and source-code
```javascript
orderBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.over"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>over ()](#apidoc.element.cash.vorpal.lodash.prototype.over)
- description and source-code
```javascript
over = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.overArgs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>overArgs ()](#apidoc.element.cash.vorpal.lodash.prototype.overArgs)
- description and source-code
```javascript
overArgs = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.overEvery"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>overEvery ()](#apidoc.element.cash.vorpal.lodash.prototype.overEvery)
- description and source-code
```javascript
overEvery = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.overSome"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>overSome ()](#apidoc.element.cash.vorpal.lodash.prototype.overSome)
- description and source-code
```javascript
overSome = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pad"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pad ()](#apidoc.element.cash.vorpal.lodash.prototype.pad)
- description and source-code
```javascript
pad = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.padEnd"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>padEnd ()](#apidoc.element.cash.vorpal.lodash.prototype.padEnd)
- description and source-code
```javascript
padEnd = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.padStart"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>padStart ()](#apidoc.element.cash.vorpal.lodash.prototype.padStart)
- description and source-code
```javascript
padStart = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.parseInt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>parseInt ()](#apidoc.element.cash.vorpal.lodash.prototype.parseInt)
- description and source-code
```javascript
parseInt = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.partial"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>partial ()](#apidoc.element.cash.vorpal.lodash.prototype.partial)
- description and source-code
```javascript
partial = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.partialRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>partialRight ()](#apidoc.element.cash.vorpal.lodash.prototype.partialRight)
- description and source-code
```javascript
partialRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.partition"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>partition ()](#apidoc.element.cash.vorpal.lodash.prototype.partition)
- description and source-code
```javascript
partition = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pick"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pick ()](#apidoc.element.cash.vorpal.lodash.prototype.pick)
- description and source-code
```javascript
pick = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pickBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pickBy ()](#apidoc.element.cash.vorpal.lodash.prototype.pickBy)
- description and source-code
```javascript
pickBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.plant"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>plant (value)](#apidoc.element.cash.vorpal.lodash.prototype.plant)
- description and source-code
```javascript
function wrapperPlant(value) {
  var result,
      parent = this;

  while (parent instanceof baseLodash) {
    var clone = wrapperClone(parent);
    clone.__index__ = 0;
    clone.__values__ = undefined;
    if (result) {
      previous.__wrapped__ = clone;
    } else {
      result = clone;
    }
    var previous = clone;
    parent = parent.__wrapped__;
  }
  previous.__wrapped__ = value;
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pop"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pop ()](#apidoc.element.cash.vorpal.lodash.prototype.pop)
- description and source-code
```javascript
pop = function () {
  var args = arguments;
  if (retUnwrapped && !this.__chain__) {
    var value = this.value();
    return func.apply(isArray(value) ? value : [], args);
  }
  return this[chainName](function(value) {
    return func.apply(isArray(value) ? value : [], args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.property"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>property ()](#apidoc.element.cash.vorpal.lodash.prototype.property)
- description and source-code
```javascript
property = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.propertyOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>propertyOf ()](#apidoc.element.cash.vorpal.lodash.prototype.propertyOf)
- description and source-code
```javascript
propertyOf = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pull"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pull ()](#apidoc.element.cash.vorpal.lodash.prototype.pull)
- description and source-code
```javascript
pull = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pullAll"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAll ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAll)
- description and source-code
```javascript
pullAll = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pullAllBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAllBy ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAllBy)
- description and source-code
```javascript
pullAllBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pullAllWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAllWith ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAllWith)
- description and source-code
```javascript
pullAllWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.pullAt"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>pullAt ()](#apidoc.element.cash.vorpal.lodash.prototype.pullAt)
- description and source-code
```javascript
pullAt = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.push"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>push ()](#apidoc.element.cash.vorpal.lodash.prototype.push)
- description and source-code
```javascript
push = function () {
  var args = arguments;
  if (retUnwrapped && !this.__chain__) {
    var value = this.value();
    return func.apply(isArray(value) ? value : [], args);
  }
  return this[chainName](function(value) {
    return func.apply(isArray(value) ? value : [], args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.random"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>random ()](#apidoc.element.cash.vorpal.lodash.prototype.random)
- description and source-code
```javascript
random = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.range"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>range ()](#apidoc.element.cash.vorpal.lodash.prototype.range)
- description and source-code
```javascript
range = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.rangeRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>rangeRight ()](#apidoc.element.cash.vorpal.lodash.prototype.rangeRight)
- description and source-code
```javascript
rangeRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.rearg"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>rearg ()](#apidoc.element.cash.vorpal.lodash.prototype.rearg)
- description and source-code
```javascript
rearg = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.reduce"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reduce ()](#apidoc.element.cash.vorpal.lodash.prototype.reduce)
- description and source-code
```javascript
reduce = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.reduceRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reduceRight ()](#apidoc.element.cash.vorpal.lodash.prototype.reduceRight)
- description and source-code
```javascript
reduceRight = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.reject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reject ()](#apidoc.element.cash.vorpal.lodash.prototype.reject)
- description and source-code
```javascript
reject = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.remove"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>remove ()](#apidoc.element.cash.vorpal.lodash.prototype.remove)
- description and source-code
```javascript
remove = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.repeat"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>repeat ()](#apidoc.element.cash.vorpal.lodash.prototype.repeat)
- description and source-code
```javascript
repeat = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.replace"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>replace ()](#apidoc.element.cash.vorpal.lodash.prototype.replace)
- description and source-code
```javascript
replace = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.rest"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>rest ()](#apidoc.element.cash.vorpal.lodash.prototype.rest)
- description and source-code
```javascript
rest = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.result"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>result ()](#apidoc.element.cash.vorpal.lodash.prototype.result)
- description and source-code
```javascript
result = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.reverse"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>reverse ()](#apidoc.element.cash.vorpal.lodash.prototype.reverse)
- description and source-code
```javascript
function wrapperReverse() {
  var value = this.__wrapped__;
  if (value instanceof LazyWrapper) {
    var wrapped = value;
    if (this.__actions__.length) {
      wrapped = new LazyWrapper(this);
    }
    wrapped = wrapped.reverse();
    wrapped.__actions__.push({
      'func': thru,
      'args': [reverse],
      'thisArg': undefined
    });
    return new LodashWrapper(wrapped, this.__chain__);
  }
  return this.thru(reverse);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.round"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>round ()](#apidoc.element.cash.vorpal.lodash.prototype.round)
- description and source-code
```javascript
round = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.runInContext"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>runInContext ()](#apidoc.element.cash.vorpal.lodash.prototype.runInContext)
- description and source-code
```javascript
runInContext = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sample"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sample ()](#apidoc.element.cash.vorpal.lodash.prototype.sample)
- description and source-code
```javascript
sample = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sampleSize"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sampleSize ()](#apidoc.element.cash.vorpal.lodash.prototype.sampleSize)
- description and source-code
```javascript
sampleSize = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.set"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>set ()](#apidoc.element.cash.vorpal.lodash.prototype.set)
- description and source-code
```javascript
set = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.setWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>setWith ()](#apidoc.element.cash.vorpal.lodash.prototype.setWith)
- description and source-code
```javascript
setWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.shift"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>shift ()](#apidoc.element.cash.vorpal.lodash.prototype.shift)
- description and source-code
```javascript
shift = function () {
  var args = arguments;
  if (retUnwrapped && !this.__chain__) {
    var value = this.value();
    return func.apply(isArray(value) ? value : [], args);
  }
  return this[chainName](function(value) {
    return func.apply(isArray(value) ? value : [], args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.shuffle"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>shuffle ()](#apidoc.element.cash.vorpal.lodash.prototype.shuffle)
- description and source-code
```javascript
shuffle = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.size"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>size ()](#apidoc.element.cash.vorpal.lodash.prototype.size)
- description and source-code
```javascript
size = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.slice"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>slice ()](#apidoc.element.cash.vorpal.lodash.prototype.slice)
- description and source-code
```javascript
slice = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.snakeCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>snakeCase ()](#apidoc.element.cash.vorpal.lodash.prototype.snakeCase)
- description and source-code
```javascript
snakeCase = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.some"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>some ()](#apidoc.element.cash.vorpal.lodash.prototype.some)
- description and source-code
```javascript
some = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sort"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sort ()](#apidoc.element.cash.vorpal.lodash.prototype.sort)
- description and source-code
```javascript
sort = function () {
  var args = arguments;
  if (retUnwrapped && !this.__chain__) {
    var value = this.value();
    return func.apply(isArray(value) ? value : [], args);
  }
  return this[chainName](function(value) {
    return func.apply(isArray(value) ? value : [], args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortBy)
- description and source-code
```javascript
sortBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedIndex)
- description and source-code
```javascript
sortedIndex = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedIndexBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedIndexBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedIndexBy)
- description and source-code
```javascript
sortedIndexBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedIndexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedIndexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedIndexOf)
- description and source-code
```javascript
sortedIndexOf = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndex"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedLastIndex ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndex)
- description and source-code
```javascript
sortedLastIndex = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndexBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedLastIndexBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndexBy)
- description and source-code
```javascript
sortedLastIndexBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndexOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedLastIndexOf ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedLastIndexOf)
- description and source-code
```javascript
sortedLastIndexOf = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedUniq"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedUniq ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedUniq)
- description and source-code
```javascript
sortedUniq = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sortedUniqBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sortedUniqBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sortedUniqBy)
- description and source-code
```javascript
sortedUniqBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.splice"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>splice ()](#apidoc.element.cash.vorpal.lodash.prototype.splice)
- description and source-code
```javascript
splice = function () {
  var args = arguments;
  if (retUnwrapped && !this.__chain__) {
    var value = this.value();
    return func.apply(isArray(value) ? value : [], args);
  }
  return this[chainName](function(value) {
    return func.apply(isArray(value) ? value : [], args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.split"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>split ()](#apidoc.element.cash.vorpal.lodash.prototype.split)
- description and source-code
```javascript
split = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.spread"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>spread ()](#apidoc.element.cash.vorpal.lodash.prototype.spread)
- description and source-code
```javascript
spread = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.startCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>startCase ()](#apidoc.element.cash.vorpal.lodash.prototype.startCase)
- description and source-code
```javascript
startCase = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.startsWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>startsWith ()](#apidoc.element.cash.vorpal.lodash.prototype.startsWith)
- description and source-code
```javascript
startsWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.stubArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubArray ()](#apidoc.element.cash.vorpal.lodash.prototype.stubArray)
- description and source-code
```javascript
stubArray = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.stubFalse"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubFalse ()](#apidoc.element.cash.vorpal.lodash.prototype.stubFalse)
- description and source-code
```javascript
stubFalse = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.stubObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubObject ()](#apidoc.element.cash.vorpal.lodash.prototype.stubObject)
- description and source-code
```javascript
stubObject = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.stubString"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubString ()](#apidoc.element.cash.vorpal.lodash.prototype.stubString)
- description and source-code
```javascript
stubString = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.stubTrue"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>stubTrue ()](#apidoc.element.cash.vorpal.lodash.prototype.stubTrue)
- description and source-code
```javascript
stubTrue = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.subtract"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>subtract ()](#apidoc.element.cash.vorpal.lodash.prototype.subtract)
- description and source-code
```javascript
subtract = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sum"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sum ()](#apidoc.element.cash.vorpal.lodash.prototype.sum)
- description and source-code
```javascript
sum = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.sumBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>sumBy ()](#apidoc.element.cash.vorpal.lodash.prototype.sumBy)
- description and source-code
```javascript
sumBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.tail"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>tail ()](#apidoc.element.cash.vorpal.lodash.prototype.tail)
- description and source-code
```javascript
tail = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.take"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>take ()](#apidoc.element.cash.vorpal.lodash.prototype.take)
- description and source-code
```javascript
take = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.takeRight"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>takeRight ()](#apidoc.element.cash.vorpal.lodash.prototype.takeRight)
- description and source-code
```javascript
takeRight = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.takeRightWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>takeRightWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.takeRightWhile)
- description and source-code
```javascript
takeRightWhile = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.takeWhile"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>takeWhile ()](#apidoc.element.cash.vorpal.lodash.prototype.takeWhile)
- description and source-code
```javascript
takeWhile = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.tap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>tap ()](#apidoc.element.cash.vorpal.lodash.prototype.tap)
- description and source-code
```javascript
tap = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.template"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>template ()](#apidoc.element.cash.vorpal.lodash.prototype.template)
- description and source-code
```javascript
template = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.throttle"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>throttle ()](#apidoc.element.cash.vorpal.lodash.prototype.throttle)
- description and source-code
```javascript
throttle = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.thru"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>thru ()](#apidoc.element.cash.vorpal.lodash.prototype.thru)
- description and source-code
```javascript
thru = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.times"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>times ()](#apidoc.element.cash.vorpal.lodash.prototype.times)
- description and source-code
```javascript
times = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toArray ()](#apidoc.element.cash.vorpal.lodash.prototype.toArray)
- description and source-code
```javascript
toArray = function () {
  var value = this.__wrapped__,
      args = isTaker ? [1] : arguments,
      isLazy = value instanceof LazyWrapper,
      iteratee = args[0],
      useLazy = isLazy || isArray(value);

  var interceptor = function(value) {
    var result = lodashFunc.apply(lodash, arrayPush([value], args));
    return (isTaker && chainAll) ? result[0] : result;
  };

  if (useLazy && checkIteratee && typeof iteratee == 'function' && iteratee.length != 1) {
    // Avoid lazy use if the iteratee has a "length" value other than '1'.
    isLazy = useLazy = false;
  }
  var chainAll = this.__chain__,
      isHybrid = !!this.__actions__.length,
      isUnwrapped = retUnwrapped && !chainAll,
      onlyLazy = isLazy && !isHybrid;

  if (!retUnwrapped && useLazy) {
    value = onlyLazy ? value : new LazyWrapper(this);
    var result = func.apply(value, args);
    result.__actions__.push({ 'func': thru, 'args': [interceptor], 'thisArg': undefined });
    return new LodashWrapper(result, chainAll);
  }
  if (isUnwrapped && onlyLazy) {
    return func.apply(this, args);
  }
  result = this.thru(interceptor);
  return isUnwrapped ? (isTaker ? result.value()[0] : result.value()) : result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toFinite"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toFinite ()](#apidoc.element.cash.vorpal.lodash.prototype.toFinite)
- description and source-code
```javascript
toFinite = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.toInteger)
- description and source-code
```javascript
toInteger = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toJSON ()](#apidoc.element.cash.vorpal.lodash.prototype.toJSON)
- description and source-code
```javascript
function wrapperValue() {
  return baseWrapperValue(this.__wrapped__, this.__actions__);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toLength"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toLength ()](#apidoc.element.cash.vorpal.lodash.prototype.toLength)
- description and source-code
```javascript
toLength = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toLower"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toLower ()](#apidoc.element.cash.vorpal.lodash.prototype.toLower)
- description and source-code
```javascript
toLower = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toNumber"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toNumber ()](#apidoc.element.cash.vorpal.lodash.prototype.toNumber)
- description and source-code
```javascript
toNumber = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toPairs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPairs ()](#apidoc.element.cash.vorpal.lodash.prototype.toPairs)
- description and source-code
```javascript
toPairs = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toPairsIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPairsIn ()](#apidoc.element.cash.vorpal.lodash.prototype.toPairsIn)
- description and source-code
```javascript
toPairsIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toPath"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPath ()](#apidoc.element.cash.vorpal.lodash.prototype.toPath)
- description and source-code
```javascript
toPath = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toPlainObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toPlainObject ()](#apidoc.element.cash.vorpal.lodash.prototype.toPlainObject)
- description and source-code
```javascript
toPlainObject = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toSafeInteger"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toSafeInteger ()](#apidoc.element.cash.vorpal.lodash.prototype.toSafeInteger)
- description and source-code
```javascript
toSafeInteger = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toString"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toString ()](#apidoc.element.cash.vorpal.lodash.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.toUpper"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>toUpper ()](#apidoc.element.cash.vorpal.lodash.prototype.toUpper)
- description and source-code
```javascript
toUpper = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.transform"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>transform ()](#apidoc.element.cash.vorpal.lodash.prototype.transform)
- description and source-code
```javascript
transform = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.trim"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>trim ()](#apidoc.element.cash.vorpal.lodash.prototype.trim)
- description and source-code
```javascript
trim = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.trimEnd"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>trimEnd ()](#apidoc.element.cash.vorpal.lodash.prototype.trimEnd)
- description and source-code
```javascript
trimEnd = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.trimStart"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>trimStart ()](#apidoc.element.cash.vorpal.lodash.prototype.trimStart)
- description and source-code
```javascript
trimStart = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.truncate"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>truncate ()](#apidoc.element.cash.vorpal.lodash.prototype.truncate)
- description and source-code
```javascript
truncate = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unary"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unary ()](#apidoc.element.cash.vorpal.lodash.prototype.unary)
- description and source-code
```javascript
unary = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unescape"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unescape ()](#apidoc.element.cash.vorpal.lodash.prototype.unescape)
- description and source-code
```javascript
unescape = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.union"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>union ()](#apidoc.element.cash.vorpal.lodash.prototype.union)
- description and source-code
```javascript
union = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unionBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unionBy ()](#apidoc.element.cash.vorpal.lodash.prototype.unionBy)
- description and source-code
```javascript
unionBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unionWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unionWith ()](#apidoc.element.cash.vorpal.lodash.prototype.unionWith)
- description and source-code
```javascript
unionWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.uniq"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniq ()](#apidoc.element.cash.vorpal.lodash.prototype.uniq)
- description and source-code
```javascript
uniq = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.uniqBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniqBy ()](#apidoc.element.cash.vorpal.lodash.prototype.uniqBy)
- description and source-code
```javascript
uniqBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.uniqWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniqWith ()](#apidoc.element.cash.vorpal.lodash.prototype.uniqWith)
- description and source-code
```javascript
uniqWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.uniqueId"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>uniqueId ()](#apidoc.element.cash.vorpal.lodash.prototype.uniqueId)
- description and source-code
```javascript
uniqueId = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unset"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unset ()](#apidoc.element.cash.vorpal.lodash.prototype.unset)
- description and source-code
```javascript
unset = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unshift"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unshift ()](#apidoc.element.cash.vorpal.lodash.prototype.unshift)
- description and source-code
```javascript
unshift = function () {
  var args = arguments;
  if (retUnwrapped && !this.__chain__) {
    var value = this.value();
    return func.apply(isArray(value) ? value : [], args);
  }
  return this[chainName](function(value) {
    return func.apply(isArray(value) ? value : [], args);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unzip"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unzip ()](#apidoc.element.cash.vorpal.lodash.prototype.unzip)
- description and source-code
```javascript
unzip = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.unzipWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>unzipWith ()](#apidoc.element.cash.vorpal.lodash.prototype.unzipWith)
- description and source-code
```javascript
unzipWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.update"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>update ()](#apidoc.element.cash.vorpal.lodash.prototype.update)
- description and source-code
```javascript
update = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.updateWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>updateWith ()](#apidoc.element.cash.vorpal.lodash.prototype.updateWith)
- description and source-code
```javascript
updateWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.upperCase"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>upperCase ()](#apidoc.element.cash.vorpal.lodash.prototype.upperCase)
- description and source-code
```javascript
upperCase = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.upperFirst"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>upperFirst ()](#apidoc.element.cash.vorpal.lodash.prototype.upperFirst)
- description and source-code
```javascript
upperFirst = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.value"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>value ()](#apidoc.element.cash.vorpal.lodash.prototype.value)
- description and source-code
```javascript
function wrapperValue() {
  return baseWrapperValue(this.__wrapped__, this.__actions__);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>valueOf ()](#apidoc.element.cash.vorpal.lodash.prototype.valueOf)
- description and source-code
```javascript
function wrapperValue() {
  return baseWrapperValue(this.__wrapped__, this.__actions__);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.values"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>values ()](#apidoc.element.cash.vorpal.lodash.prototype.values)
- description and source-code
```javascript
values = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.valuesIn"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>valuesIn ()](#apidoc.element.cash.vorpal.lodash.prototype.valuesIn)
- description and source-code
```javascript
valuesIn = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.without"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>without ()](#apidoc.element.cash.vorpal.lodash.prototype.without)
- description and source-code
```javascript
without = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.words"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>words ()](#apidoc.element.cash.vorpal.lodash.prototype.words)
- description and source-code
```javascript
words = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.wrap"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>wrap ()](#apidoc.element.cash.vorpal.lodash.prototype.wrap)
- description and source-code
```javascript
wrap = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.xor"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>xor ()](#apidoc.element.cash.vorpal.lodash.prototype.xor)
- description and source-code
```javascript
xor = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.xorBy"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>xorBy ()](#apidoc.element.cash.vorpal.lodash.prototype.xorBy)
- description and source-code
```javascript
xorBy = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.xorWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>xorWith ()](#apidoc.element.cash.vorpal.lodash.prototype.xorWith)
- description and source-code
```javascript
xorWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.zip"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zip ()](#apidoc.element.cash.vorpal.lodash.prototype.zip)
- description and source-code
```javascript
zip = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.zipObject"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zipObject ()](#apidoc.element.cash.vorpal.lodash.prototype.zipObject)
- description and source-code
```javascript
zipObject = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.zipObjectDeep"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zipObjectDeep ()](#apidoc.element.cash.vorpal.lodash.prototype.zipObjectDeep)
- description and source-code
```javascript
zipObjectDeep = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.lodash.prototype.zipWith"></a>[function <span class="apidocSignatureSpan">cash.vorpal.lodash.prototype.</span>zipWith ()](#apidoc.element.cash.vorpal.lodash.prototype.zipWith)
- description and source-code
```javascript
zipWith = function () {
  var chainAll = this.__chain__;
  if (chain || chainAll) {
    var result = object(this.__wrapped__),
        actions = result.__actions__ = copyArray(this.__actions__);

    actions.push({ 'func': func, 'args': arguments, 'thisArg': object });
    result.__chain__ = chainAll;
    return result;
  }
  return func.apply(object, arrayPush([this.value()], arguments));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.ui"></a>[module cash.vorpal.ui](#apidoc.module.cash.vorpal.ui)

#### <a name="apidoc.element.cash.vorpal.ui._sigint"></a>[function <span class="apidocSignatureSpan">cash.vorpal.ui.</span>_sigint ()](#apidoc.element.cash.vorpal.ui._sigint)
- description and source-code
```javascript
_sigint = function () {
  if (_this._sigintCount > 1) {
    process.exit(0);
  } else {
    var text = _this.input();
    if (!_this.parent) {
      // If Vorpal isn't shown, just exit.
      process.exit(0);
    } else if (_this.parent.session.cancelCommands) {
      // There are commands running if
      // cancelCommands function is available.
      _this.imprint();
      _this.submit('');
      _this._sigintCalled = false;
      _this._sigintCount = 0;
      _this.parent.session.emit('vorpal_command_cancel');
    } else if (String(text).trim() !== '') {
      _this.imprint();
      _this.submit('');
      _this._sigintCalled = false;
      _this._sigintCount = 0;
    } else {
      _this._sigintCalled = false;
      _this.delimiter(' ');
      _this.submit('');
      _this.log('(^C again to quit)');
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cash.vorpal.util"></a>[module cash.vorpal.util](#apidoc.module.cash.vorpal.util)

#### <a name="apidoc.element.cash.vorpal.util.buildCommandArgs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>buildCommandArgs (passedArgs, cmd, execCommand, isCommandArgKeyPairNormalized)](#apidoc.element.cash.vorpal.util.buildCommandArgs)
- description and source-code
```javascript
function buildCommandArgs(passedArgs, cmd, execCommand, isCommandArgKeyPairNormalized) {
  var args = { options: {} };

  if (isCommandArgKeyPairNormalized) {
    // Normalize all foo="bar" with "foo='bar'"
    // This helps implement unix-like key value pairs.
    var reg = /(['"]?)(\w+)=(?:(['"])((?:(?!\3).)*)\3|(\S+))\1/g;
    passedArgs = passedArgs.replace(reg, '"$2=\'$4$5\'"');
  }

  // Types are custom arg types passed
  // into 'minimist' as per its docs.
  var types = cmd._types || {};

  // Make a list of all boolean options
  // registered for this command. These are
  // simply commands that don't have required
  // or optional args.
  var booleans = [];
  cmd.options.forEach(function (opt) {
    if (opt.required === 0 && opt.optional === 0) {
      if (opt.short) {
        booleans.push(opt.short);
      }
      if (opt.long) {
        booleans.push(opt.long);
      }
    }
  });

  // Review the args passed into the command,
  // and filter out the boolean list to only those
  // options passed in.
  // This returns a boolean list of all options
  // passed in by the caller, which don't have
  // required or optional args.
  var passedArgParts = passedArgs.split(' ');
  types.boolean = booleans.map(function (str) {
    return String(str).replace(/^-*/, '');
  }).filter(function (str) {
    var match = false;
    var strings = ['-' + str, '--' + str, '--no-' + str];
    for (var i = 0; i < passedArgParts.length; ++i) {
      if (strings.indexOf(passedArgParts[i]) > -1) {
        match = true;
        break;
      }
    }
    return match;
  });

  // Use minimist to parse the args.
  var parsedArgs = this.parseArgs(passedArgs, types);

  function validateArg(arg, cmdArg) {
    return !(arg === undefined && cmdArg.required === true);
  }

  // Builds varidiac args and options.
  var valid = true;
  var remainingArgs = _.clone(parsedArgs._);
  for (var l = 0; l < 10; ++l) {
    var matchArg = cmd._args[l];
    var passedArg = parsedArgs._[l];
    if (matchArg !== undefined) {
      valid = !valid ? false : validateArg(parsedArgs._[l], matchArg);
      if (!valid) {
        break;
      }
      if (passedArg && matchArg.variadic === true) {
        args[matchArg.name] = remainingArgs;
      } else if (passedArg !== undefined) {
        args[matchArg.name] = passedArg;
        remainingArgs.shift();
      }
    }
  }

  if (!valid) {
    return '\n  Missing required argument. Showing Help:';
  }

  // Looks for ommitted required options and throws help.
  for (var m = 0; m < cmd.options.length; ++m) {
    var o = cmd.options[m];
    var short = String(o.short || '').replace(/-/g, '');
    var long = String(o.long || '').replace(/--no-/g, '').replace(/^-*/g, '');
    var exist = parsedArgs[short] !== undefined ? parsedArgs[short] : undefined;
    exist = exist === undefined && parsedArgs[long] !== undefined ? parsedArgs[long] : exist;
    var existsNotSet = exist === true || exist === false;
    if (existsNotSet && o.required !== 0) {
      return '\n  Missing required value for option ' + (o.long || o.short) + '. Showing Help:';
    }
    if (exist !== undefined) {
      args.options[long || short] = exist;
    }
  }

  // Looks for supplied options that don't
  // exist in the options list.
  // If the command allows unknown options,
  // adds it, otherwise throws help.
  var passedOpts = _.chain(parsedArgs).keys().pull('_').pull('help').value();

  var _loop = function _loop(key) {
    var opt = passedOpts[key];
    var optionFound = _.find(cmd.options, function (expected) {
      if ('--' + opt === expected.long || '--no-' + opt === expected.long || '-' + opt === expected.short) {
        return true;
      }
      return false;
    });
    if (optionFound === undefined) {
      if (cmd._allowUnknownOptions) {
        args.options[opt] = parsedArgs[opt];
      } else {
        return {
          v: '\n  Invalid option: \'' + opt + '\'. Showing Help:'
        };
      }
    }
  };

  for (var key in passedOpts) {
    var _ret = _loop(key);

    if ((typeof _ret === 'undefined' ? 'undefined' : _typeof(_ret)) = ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.fixArgsForApply"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>fixArgsForApply (obj)](#apidoc.element.cash.vorpal.util.fixArgsForApply)
- description and source-code
```javascript
function fixArgsForApply(obj) {
  if (!_.isObject(obj)) {
    if (!_.isArray(obj)) {
      return [obj];
    }
    return obj;
  }
  var argArray = [];
  for (var key in obj) {
    var aarg = obj[key];
    argArray.push(aarg);
  }
  return argArray;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.humanReadableArgName"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>humanReadableArgName (arg)](#apidoc.element.cash.vorpal.util.humanReadableArgName)
- description and source-code
```javascript
function humanReadableArgName(arg) {
  var nameOutput = arg.name + (arg.variadic === true ? '...' : '');
  return arg.required ? '<' + nameOutput + '>' : '[' + nameOutput + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.matchCommand"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>matchCommand (cmd, cmds)](#apidoc.element.cash.vorpal.util.matchCommand)
- description and source-code
```javascript
function matchCommand(cmd, cmds) {
  var parts = String(cmd).trim().split(' ');

  var match = undefined;
  var matchArgs = undefined;
  for (var i = 0; i < parts.length; ++i) {
    var subcommand = String(parts.slice(0, parts.length - i).join(' ')).trim();
    match = _.find(cmds, { _name: subcommand }) || match;
    if (!match) {
      for (var key in cmds) {
        var _cmd = cmds[key];
        var idx = _cmd._aliases.indexOf(subcommand);
        match = idx > -1 ? _cmd : match;
      }
    }
    if (match) {
      matchArgs = parts.slice(parts.length - i, parts.length).join(' ');
      break;
    }
  }
  // If there's no command match, check if the
  // there's a 'catch' command, which catches all
  // missed commands.
  if (!match) {
    match = _.find(cmds, { _catch: true });
    // If there is one, we still need to make sure we aren't
    // partially matching command groups, such as 'do things' when
    // there is a command 'do things well'. If we match partially,
    // we still want to show the help menu for that command group.
    if (match) {
      var allCommands = _.map(cmds, '_name');
      var wordMatch = false;
      for (var key in allCommands) {
        var _cmd2 = allCommands[key];
        var parts2 = String(_cmd2).split(' ');
        var cmdParts = String(match.command).split(' ');
        var matchAll = true;
        for (var k = 0; k < cmdParts.length; ++k) {
          if (parts2[k] !== cmdParts[k]) {
            matchAll = false;
            break;
          }
        }
        if (matchAll) {
          wordMatch = true;
          break;
        }
      }
      if (wordMatch) {
        match = undefined;
      } else {
        matchArgs = cmd;
      }
    }
  }

  return {
    command: match,
    args: matchArgs
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.pad"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>pad (str, width, delimiter)](#apidoc.element.cash.vorpal.util.pad)
- description and source-code
```javascript
function pad(str, width, delimiter) {
  width = Math.floor(width);
  delimiter = delimiter || ' ';
  var len = Math.max(0, width - strip(str).length);
  return str + Array(len + 1).join(delimiter);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.parseArgs"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>parseArgs (str, opts)](#apidoc.element.cash.vorpal.util.parseArgs)
- description and source-code
```javascript
function parseArgs(str, opts) {
  var reg = /"(.*?)"|'(.*?)'|'(.*?)'|([^\s"]+)/gi;
  var arr = [];
  var match = undefined;
  do {
    match = reg.exec(str);
    if (match !== null) {
      arr.push(match[1] || match[2] || match[3] || match[4]);
    }
  } while (match !== null);

  arr = minimist(arr, opts);
  arr._ = arr._ || [];
  return arr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.parseCommand"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>parseCommand (command, commands)](#apidoc.element.cash.vorpal.util.parseCommand)
- description and source-code
```javascript
function parseCommand(command, commands) {
  var self = this;
  var pipes = [];
  var match = undefined;
  var matchArgs = undefined;
  var matchParts = undefined;

  function parsePipes() {
    // First, split the command by pipes naively.
    // This will split command arguments in half when the argument contains a pipe character.
    // For example, say "(Vorpal|vorpal)" will be split into ['say "(Vorpal', 'vorpal)'] which isn't good.
    var naivePipes = String(command).trim().split('|');

    // Contruct empty array to place correctly split commands into.
    var newPipes = [];

    // We will look for pipe characters within these quotes to rejoin together.
    var quoteChars = ['"', '\'', '''];

    // This will expand to contain one boolean key for each type of quote.
    // The value keyed by the quote is toggled off and on as quote type is opened and closed.
    // Example { "'": true, "'": false } would mean that there is an open angle quote.
    var quoteTracker = {};

    // The current command piece before being rejoined with it's over half.
    // Since it's not common for pipes to occur in commands, this is usually the entire command pipe.
    var commandPart = '';

    // Loop through each naive pipe.
    for (var key in naivePipes) {
      // It's possible/likely that this naive pipe is the whole pipe if it doesn't contain an unfinished quote.
      var possiblePipe = naivePipes[key];
      commandPart += possiblePipe;

      // Loop through each individual character in the possible pipe tracking the opening and closing of quotes.
      for (var i = 0; i < possiblePipe.length; i++) {
        var char = possiblePipe[i];
        if (quoteChars.indexOf(char) !== -1) {
          quoteTracker[char] = !quoteTracker[char];
        }
      }

      // Does the pipe end on an unfinished quote?
      var inQuote = _.some(quoteChars, function (quoteChar) {
        return quoteTracker[quoteChar];
      });

      // If the quotes have all been closed or this is the last possible pipe in the array, add as pipe.
      if (!inQuote || key * 1 === naivePipes.length - 1) {
        newPipes.push(commandPart.trim());
        commandPart = '';
      } else {
        // Quote was left open. The pipe character was previously removed when the array was split.
        commandPart += '|';
      }
    }

    // Set the first pipe to command and the rest to pipes.
    command = newPipes.shift();
    pipes = pipes.concat(newPipes);
  }

  function parseMatch() {
    matchParts = self.matchCommand(command, commands);
    match = matchParts.command;
    matchArgs = matchParts.args;
  }

  parsePipes();
  parseMatch();

  if (match && _.isFunction(match._parse)) {
    command = match._parse(command, matchParts.args);
    parsePipes();
    parseMatch();
  }

  return {
    command: command,
    match: match,
    matchArgs: matchArgs,
    pipes: pipes
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cash.vorpal.util.prettifyArray"></a>[function <span class="apidocSignatureSpan">cash.vorpal.util.</span>prettifyArray (arr)](#apidoc.element.cash.vorpal.util.prettifyArray)
- description and source-code
```javascript
function prettifyArray(arr) {
  arr = arr || [];
  var arrClone = _.clone(arr);
  var width = process.stdout.columns;
  var longest = strip(arrClone.sort(function (a, b) {
    return strip(b).length - strip(a).length;
  })[0] || '').length + 2;
  var fullWidth = strip(String(arr.join(''))).length;
  var fitsOneLine = fullWidth + arr.length * 2 <= width;
  var cols = Math.floor(width / longest);
  cols = cols < 1 ? 1 : cols;
  if (fitsOneLine) {
    return arr.join('  ');
  }
  var col = 0;
  var lines = [];
  var line = '';
  for (var key in arr) {
    var arrEl = arr[key];
    if (col < cols) {
      col++;
    } else {
      lines.push(line);
      line = '';
      col = 1;
    }
    line += this.pad(arrEl, longest, ' ');
  }
  if (line !== '') {
    lines.push(line);
  }
  return lines.join('\n');
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
