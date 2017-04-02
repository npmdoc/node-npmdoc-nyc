# api documentation for  [nyc (v10.2.0)](https://github.com/istanbuljs/nyc#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nyc.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nyc) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nyc.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nyc)
#### the Istanbul command line interface

[![NPM](https://nodei.co/npm/nyc.png?downloads=true)](https://www.npmjs.com/package/nyc)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nyc/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nyc_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nyc/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-nyc/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Ben Coe",
        "email": "ben@npmjs.com"
    },
    "bin": {
        "nyc": "./bin/nyc.js"
    },
    "bugs": {
        "url": "https://github.com/istanbuljs/nyc/issues"
    },
    "bundleDependencies": [
        "archy",
        "arrify",
        "caching-transform",
        "convert-source-map",
        "debug-log",
        "default-require-extensions",
        "find-cache-dir",
        "find-up",
        "foreground-child",
        "glob",
        "istanbul-lib-coverage",
        "istanbul-lib-hook",
        "istanbul-lib-instrument",
        "istanbul-lib-report",
        "istanbul-lib-source-maps",
        "istanbul-reports",
        "md5-hex",
        "merge-source-map",
        "micromatch",
        "mkdirp",
        "resolve-from",
        "rimraf",
        "signal-exit",
        "spawn-wrap",
        "test-exclude",
        "yargs",
        "yargs-parser"
    ],
    "contributors": [
        {
            "name": "Isaac Schlueter"
        },
        {
            "name": "Mark Wubben"
        },
        {
            "name": "James Talmage"
        },
        {
            "name": "Krishnan Anantheswaran"
        }
    ],
    "dependencies": {
        "archy": "^1.0.0",
        "arrify": "^1.0.1",
        "caching-transform": "^1.0.0",
        "convert-source-map": "^1.3.0",
        "debug-log": "^1.0.1",
        "default-require-extensions": "^1.0.0",
        "find-cache-dir": "^0.1.1",
        "find-up": "^1.1.2",
        "foreground-child": "^1.5.3",
        "glob": "^7.0.6",
        "istanbul-lib-coverage": "^1.0.2",
        "istanbul-lib-hook": "^1.0.5",
        "istanbul-lib-instrument": "^1.7.0",
        "istanbul-lib-report": "^1.0.0",
        "istanbul-lib-source-maps": "^1.1.1",
        "istanbul-reports": "^1.0.2",
        "md5-hex": "^1.2.0",
        "merge-source-map": "^1.0.2",
        "micromatch": "^2.3.11",
        "mkdirp": "^0.5.0",
        "resolve-from": "^2.0.0",
        "rimraf": "^2.5.4",
        "signal-exit": "^3.0.1",
        "spawn-wrap": "1.2.4",
        "test-exclude": "^4.0.0",
        "yargs": "^7.0.2",
        "yargs-parser": "^4.0.2"
    },
    "description": "the Istanbul command line interface",
    "devDependencies": {
        "any-path": "^1.3.0",
        "bundle-dependencies": "^1.0.2",
        "chai": "^3.0.0",
        "coveralls": "^2.11.11",
        "exists-sync": "0.0.4",
        "forking-tap": "^0.1.1",
        "is-windows": "^1.0.0",
        "lodash": "^4.12.0",
        "newline-regex": "^0.2.1",
        "requirejs": "^2.3.0",
        "sanitize-filename": "^1.5.3",
        "sinon": "^2.1.0",
        "source-map-support": "^0.4.6",
        "split-lines": "^1.0.0",
        "standard": "^9.0.2",
        "standard-version": "^4.0.0",
        "tap": "^10.0.0",
        "which": "^1.2.11",
        "zero-fill": "^2.2.3"
    },
    "directories": {},
    "dist": {
        "shasum": "facd90240600c9aa4dd81ea99c2fb6a85c53de0c",
        "tarball": "https://registry.npmjs.org/nyc/-/nyc-10.2.0.tgz"
    },
    "files": [
        "index.js",
        "bin/*.js",
        "lib/*.js",
        "lib/commands/*.js",
        "lib/instrumenters/*.js",
        "!**/*covered.js"
    ],
    "gitHead": "455619f9fdd0a1f4fa08b0621e030cceda969011",
    "greenkeeper": {
        "ignore": [
            "find-up"
        ]
    },
    "homepage": "https://github.com/istanbuljs/nyc#readme",
    "keywords": [
        "coverage",
        "reporter",
        "subprocess",
        "testing"
    ],
    "license": "ISC",
    "main": "index.js",
    "maintainers": [
        {
            "name": "bcoe",
            "email": "ben@npmjs.com"
        },
        {
            "name": "isaacs",
            "email": "isaacs@npmjs.com"
        }
    ],
    "name": "nyc",
    "nyc": {
        "exclude": [
            "node_modules",
            "bin",
            "coverage",
            "test/fixtures/coverage.js",
            "test/build/*",
            "test/nyc-test.js",
            "index.covered.js",
            "test/fixtures/_generateCoverage.js"
        ]
    },
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/istanbuljs/nyc.git"
    },
    "scripts": {
        "build": "node ./build-tests",
        "bundle": "bundle-dependencies update",
        "clean": "rimraf ./.nyc_output ./node_modules/.cache ./.self_coverage ./test/fixtures/.nyc_output ./test/fixtures/node_modules/.cache *covered.js ./lib/*covered.js",
        "cover": "npm run clean && npm run build && npm run instrument && npm run run-tests && npm run report",
        "dev": "npm run clean && npm run build && npm run run-tests",
        "instrument": "node ./build-self-coverage.js",
        "pretest": "standard",
        "release": "standard-version",
        "report": "node ./bin/nyc  --temp-directory ./.self_coverage/ -r text -r lcov report",
        "run-tests": "tap -t120 --no-cov -b ./test/build/*.js ./test/src/nyc-bin.js ./test/src/process-args.js",
        "test": "npm run cover"
    },
    "standard": {
        "ignore": [
            "**/fixtures/**",
            "**/test/build/*"
        ]
    },
    "version": "10.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nyc](#apidoc.module.nyc)
1.  [function <span class="apidocSignatureSpan">nyc.</span>process (defaults)](#apidoc.element.nyc.process)
1.  object <span class="apidocSignatureSpan">nyc.</span>config_util
1.  object <span class="apidocSignatureSpan">nyc.</span>process.prototype
1.  object <span class="apidocSignatureSpan">nyc.</span>process_args

#### [module nyc.config_util](#apidoc.module.nyc.config_util)
1.  [function <span class="apidocSignatureSpan">nyc.config_util.</span>buildYargs (cwd)](#apidoc.element.nyc.config_util.buildYargs)
1.  [function <span class="apidocSignatureSpan">nyc.config_util.</span>decorateYargs (yargs)](#apidoc.element.nyc.config_util.decorateYargs)
1.  [function <span class="apidocSignatureSpan">nyc.config_util.</span>loadConfig (argv, cwd)](#apidoc.element.nyc.config_util.loadConfig)

#### [module nyc.process](#apidoc.module.nyc.process)
1.  [function <span class="apidocSignatureSpan">nyc.</span>process (defaults)](#apidoc.element.nyc.process.process)
1.  [function <span class="apidocSignatureSpan">nyc.process.</span>buildProcessTree (infos)](#apidoc.element.nyc.process.buildProcessTree)

#### [module nyc.process.prototype](#apidoc.module.nyc.process.prototype)
1.  [function <span class="apidocSignatureSpan">nyc.process.prototype.</span>getCoverageMap (merger)](#apidoc.element.nyc.process.prototype.getCoverageMap)
1.  [function <span class="apidocSignatureSpan">nyc.process.prototype.</span>render (nyc)](#apidoc.element.nyc.process.prototype.render)

#### [module nyc.process_args](#apidoc.module.nyc.process_args)
1.  [function <span class="apidocSignatureSpan">nyc.process_args.</span>hideInstrumenteeArgs ()](#apidoc.element.nyc.process_args.hideInstrumenteeArgs)
1.  [function <span class="apidocSignatureSpan">nyc.process_args.</span>hideInstrumenterArgs (yargv)](#apidoc.element.nyc.process_args.hideInstrumenterArgs)



# <a name="apidoc.module.nyc"></a>[module nyc](#apidoc.module.nyc)

#### <a name="apidoc.element.nyc.process"></a>[function <span class="apidocSignatureSpan">nyc.</span>process (defaults)](#apidoc.element.nyc.process)
- description and source-code
```javascript
function ProcessInfo(defaults) {
  defaults = defaults || {}

  this.pid = String(process.pid)
  this.argv = process.argv
  this.execArgv = process.execArgv
  this.cwd = process.cwd()
  this.time = Date.now()
  this.ppid = null
  this.root = null
  this.coverageFilename = null
  this.nodes = [] // list of children, filled by buildProcessTree()

  this._coverageMap = null

  for (var key in defaults) {
    this[key] = defaults[key]
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nyc.config_util"></a>[module nyc.config_util](#apidoc.module.nyc.config_util)

#### <a name="apidoc.element.nyc.config_util.buildYargs"></a>[function <span class="apidocSignatureSpan">nyc.config_util.</span>buildYargs (cwd)](#apidoc.element.nyc.config_util.buildYargs)
- description and source-code
```javascript
buildYargs = function (cwd) {
  return Yargs([])
    .usage('$0 [command] [options]\n\nrun your tests with the nyc bin to instrument them with coverage')
    .command('report', 'run coverage report for .nyc_output', function (yargs) {
      return yargs
        .usage('$0 report [options]')
        .option('reporter', {
          alias: 'r',
          describe: 'coverage reporter(s) to use',
          default: 'text'
        })
        .option('report-dir', {
          describe: 'directory to output coverage reports in',
          default: 'coverage'
        })
        .option('temp-directory', {
          describe: 'directory from which coverage JSON files are read',
          default: './.nyc_output'
        })
        .option('show-process-tree', {
          describe: 'display the tree of spawned processes',
          default: false,
          type: 'boolean'
        })
        .example('$0 report --reporter=lcov', 'output an HTML lcov report to ./coverage')
    })
    .command('check-coverage', 'check whether coverage is within thresholds provided', function (yargs) {
      return yargs
        .usage('$0 check-coverage [options]')
        .option('branches', {
          default: 0,
          description: 'what % of branches must be covered?'
        })
        .option('functions', {
          default: 0,
          description: 'what % of functions must be covered?'
        })
        .option('lines', {
          default: 90,
          description: 'what % of lines must be covered?'
        })
        .option('statements', {
          default: 0,
          description: 'what % of statements must be covered?'
        })
        .example('$0 check-coverage --lines 95', "check whether the JSON in nyc's output folder meets the thresholds provided")
    })
    .option('reporter', {
      alias: 'r',
      describe: 'coverage reporter(s) to use',
      default: 'text',
      globa: false
    })
    .option('report-dir', {
      describe: 'directory to output coverage reports in',
      default: 'coverage',
      global: false
    })
    .option('silent', {
      alias: 's',
      default: false,
      type: 'boolean',
      describe: "don't output a report after tests finish running",
      global: false
    })
    .option('all', {
      alias: 'a',
      default: false,
      type: 'boolean',
      describe: 'whether or not to instrument all files of the project (not just the ones touched by your test suite)',
      global: false
    })
    .option('exclude', {
      alias: 'x',
      default: testExclude.defaultExclude,
      describe: 'a list of specific files and directories that should be excluded from coverage, glob patterns are supported, node_modules
 is always excluded',
      global: false
    })
    .option('include', {
      alias: 'n',
      default: [],
      describe: 'a list of specific files that should be covered, glob patterns are supported',
      global: false
    })
    .option('require', {
      alias: 'i',
      default: [],
      describe: 'a list of additional modules that nyc should attempt to require in its subprocess, e.g., babel-register, babel-
polyfill.',
      global: false
    })
    .option('eager', {
      default: false,
      type: 'boolean',
      describe: 'instantiate the instrumenter at startup (see https://git.io/vMKZ9)',
      global: false
    })
    .option('cache', {
      alias: 'c',
      default: true,
      type: 'boolean',
      describe: 'cache instrumentation results for improved performance',
      global: false
    })
    .option('babel-cache', {
      default: false,
      type: 'boolean',
      describe: 'cache babel transpilation results for improved performance',
      global: false
    })
    .option('extension', {
      alias: 'e',
      default: [],
      describe: 'a list of extensions that nyc should handle in addition to .js',
      global: false
    })
    .option('check-coverage', {
      type: 'boolean',
      default: false,
      describe: 'check whether coverage is within thresholds provided',
      global: false
    })
    .option('branches', {
      default: 0, ...
```
- example usage
```shell
...
  )
}

if (pkgPath) {
  cwd = path.dirname(pkgPath)
}

var config = Config.buildYargs(cwd)
  .default({
    cwd: cwd
  })
if (rcConfig) config.config(rcConfig)
config = config.parse(argv || [])

// post-hoc, we convert several of the
...
```

#### <a name="apidoc.element.nyc.config_util.decorateYargs"></a>[function <span class="apidocSignatureSpan">nyc.config_util.</span>decorateYargs (yargs)](#apidoc.element.nyc.config_util.decorateYargs)
- description and source-code
```javascript
decorateYargs = function (yargs) {
  return yargs
    .help('h')
    .alias('h', 'help')
    .version()
    .command(require('../lib/commands/instrument'))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nyc.config_util.loadConfig"></a>[function <span class="apidocSignatureSpan">nyc.config_util.</span>loadConfig (argv, cwd)](#apidoc.element.nyc.config_util.loadConfig)
- description and source-code
```javascript
loadConfig = function (argv, cwd) {
  cwd = cwd || process.env.NYC_CWD || process.cwd()
  var pkgPath = findUp.sync('package.json', {cwd: cwd})
  var rcPath = findUp.sync('.nycrc', {cwd: cwd})
  var rcConfig = null

  if (rcPath) {
    rcConfig = JSON.parse(
      fs.readFileSync(rcPath, 'utf-8')
    )
  }

  if (pkgPath) {
    cwd = path.dirname(pkgPath)
  }

  var config = Config.buildYargs(cwd)
    .default({
      cwd: cwd
    })
  if (rcConfig) config.config(rcConfig)
  config = config.parse(argv || [])

  // post-hoc, we convert several of the
  // configuration settings to arrays, providing
  // a consistent contract to index.js.
  config.require = arrify(config.require)
  config.extension = arrify(config.extension)
  config.exclude = arrify(config.exclude)
  config.include = arrify(config.include)
  config.cwd = cwd

  return config
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.nyc.process"></a>[module nyc.process](#apidoc.module.nyc.process)

#### <a name="apidoc.element.nyc.process.process"></a>[function <span class="apidocSignatureSpan">nyc.</span>process (defaults)](#apidoc.element.nyc.process.process)
- description and source-code
```javascript
function ProcessInfo(defaults) {
  defaults = defaults || {}

  this.pid = String(process.pid)
  this.argv = process.argv
  this.execArgv = process.execArgv
  this.cwd = process.cwd()
  this.time = Date.now()
  this.ppid = null
  this.root = null
  this.coverageFilename = null
  this.nodes = [] // list of children, filled by buildProcessTree()

  this._coverageMap = null

  for (var key in defaults) {
    this[key] = defaults[key]
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nyc.process.buildProcessTree"></a>[function <span class="apidocSignatureSpan">nyc.process.</span>buildProcessTree (infos)](#apidoc.element.nyc.process.buildProcessTree)
- description and source-code
```javascript
buildProcessTree = function (infos) {
  var treeRoot = new ProcessInfo({ _label: 'nyc' })
  var nodes = { }

  infos = infos.sort(function (a, b) {
    return a.time - b.time
  })

  infos.forEach(function (p) {
    nodes[p.root + ':' + p.pid] = p
  })

  infos.forEach(function (p) {
    if (!p.ppid) {
      return
    }

    var parent = nodes[p.root + ':' + p.ppid]
    if (!parent) {
      parent = treeRoot
    }

    parent.nodes.push(p)
  })

  return treeRoot
}
```
- example usage
```shell
...

if (this._showProcessTree) {
  this.showProcessTree()
}
}

NYC.prototype.showProcessTree = function () {
var processTree = ProcessInfo.buildProcessTree(this._loadProcessInfos())

console.log(processTree.render(this))
}

NYC.prototype.checkCoverage = function (thresholds) {
var map = this._getCoverageMapFromAllCoverageFiles()
var summary = map.getCoverageSummary()
...
```



# <a name="apidoc.module.nyc.process.prototype"></a>[module nyc.process.prototype](#apidoc.module.nyc.process.prototype)

#### <a name="apidoc.element.nyc.process.prototype.getCoverageMap"></a>[function <span class="apidocSignatureSpan">nyc.process.prototype.</span>getCoverageMap (merger)](#apidoc.element.nyc.process.prototype.getCoverageMap)
- description and source-code
```javascript
getCoverageMap = function (merger) {
  if (this._coverageMap) {
    return this._coverageMap
  }

  var childMaps = this.nodes.map(function (child) {
    return child.getCoverageMap(merger)
  })

  this._coverageMap = merger([this.coverageFilename], childMaps)

  return this._coverageMap
}
```
- example usage
```shell
...

ProcessInfo.prototype.getCoverageMap = function (merger) {
  if (this._coverageMap) {
    return this._coverageMap
  }

  var childMaps = this.nodes.map(function (child) {
    return child.getCoverageMap(merger)
  })

  this._coverageMap = merger([this.coverageFilename], childMaps)

  return this._coverageMap
}
...
```

#### <a name="apidoc.element.nyc.process.prototype.render"></a>[function <span class="apidocSignatureSpan">nyc.process.prototype.</span>render (nyc)](#apidoc.element.nyc.process.prototype.render)
- description and source-code
```javascript
render = function (nyc) {
  this.getCoverageMap(function (filenames, maps) {
    var map = libCoverage.createCoverageMap({})

    nyc.loadReports(filenames).forEach(function (report) {
      map.merge(report)
    })

    maps.forEach(function (otherMap) {
      map.merge(otherMap)
    })

    return map
  })

  return archy(this)
}
```
- example usage
```shell
...
  this.showProcessTree()
}
}

NYC.prototype.showProcessTree = function () {
var processTree = ProcessInfo.buildProcessTree(this._loadProcessInfos())

console.log(processTree.render(this))
}

NYC.prototype.checkCoverage = function (thresholds) {
var map = this._getCoverageMapFromAllCoverageFiles()
var summary = map.getCoverageSummary()

// ERROR: Coverage for lines (90.12%) does not meet global threshold (120%)
...
```



# <a name="apidoc.module.nyc.process_args"></a>[module nyc.process_args](#apidoc.module.nyc.process_args)

#### <a name="apidoc.element.nyc.process_args.hideInstrumenteeArgs"></a>[function <span class="apidocSignatureSpan">nyc.process_args.</span>hideInstrumenteeArgs ()](#apidoc.element.nyc.process_args.hideInstrumenteeArgs)
- description and source-code
```javascript
hideInstrumenteeArgs = function () {
  var argv = process.argv.slice(2)
  var yargv = parser(argv)
  if (!yargv._.length) return argv
  for (var i = 0, command; (command = yargv._[i]) !== undefined; i++) {
    if (~commands.indexOf(command)) return argv
  }

  // drop all the arguments after the bin being
  // instrumented by nyc.
  argv = argv.slice(0, argv.indexOf(yargv._[0]))
  argv.push(yargv._[0])

  return argv
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nyc.process_args.hideInstrumenterArgs"></a>[function <span class="apidocSignatureSpan">nyc.process_args.</span>hideInstrumenterArgs (yargv)](#apidoc.element.nyc.process_args.hideInstrumenterArgs)
- description and source-code
```javascript
hideInstrumenterArgs = function (yargv) {
  var argv = process.argv.slice(1)
  argv = argv.slice(argv.indexOf(yargv._[0]))
  if (argv[0][0] === '-') {
    argv.unshift(process.execPath)
  }
  return argv
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
