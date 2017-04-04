# api documentation for  [mockgoose (v7.1.1)](https://github.com/Mockgoose/Mockgoose)  [![npm package](https://img.shields.io/npm/v/npmdoc-mockgoose.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mockgoose) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mockgoose.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mockgoose)
#### Mockgoose is an in memory database mock to allow for testing of applications that rely on Mongoose.

[![NPM](https://nodei.co/npm/mockgoose.png?downloads=true)](https://www.npmjs.com/package/mockgoose)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mockgoose/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mockgoose_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mockgoose/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mockgoose/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mockgoose/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Anthony McCormick",
        "email": "anthony.mccormick@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/Mockgoose/Mockgoose/issues"
    },
    "dependencies": {
        "async": "2.1.5",
        "debug": "2.2.0",
        "fs-extra": "^2.0.0",
        "mongodb-prebuilt": "^6.0.2",
        "portfinder": "^1.0.13",
        "rimraf": "^2.6.1",
        "uuid": "^3.0.1"
    },
    "description": "Mockgoose is an in memory database mock to allow for testing of applications that rely on Mongoose.",
    "devDependencies": {
        "@types/async": "~2.0.39",
        "@types/fs-extra": "~0.0.37",
        "@types/mongoose": "^4.7.6",
        "@types/node": "^6.0.58",
        "@types/node-uuid": "0.0.28",
        "chai": "~2.2.0",
        "mocha": "~2.2.4",
        "mongoose": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "0959fe2928c7f2e09f8dcd3eca36b4a0a8b1d6c4",
        "tarball": "https://registry.npmjs.org/mockgoose/-/mockgoose-7.1.1.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "4de055ad2d791c5f4a309cb261f3e44f2769bcab",
    "homepage": "https://github.com/Mockgoose/Mockgoose",
    "keywords": [
        "mongodb",
        "mongoose",
        "datastore",
        "nosql",
        "sql",
        "db",
        "database",
        "mock",
        "stub",
        "in memory"
    ],
    "license": "MIT",
    "main": "built/mockgoose.js",
    "maintainers": [
        {
            "name": "mccormicka",
            "email": "anthony.mccormick@gmail.com"
        },
        {
            "name": "winfinit",
            "email": "winfinit@gmail.com"
        }
    ],
    "name": "mockgoose",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mockgoose/Mockgoose.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "types": "built/mockgoose.d.ts",
    "version": "7.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mockgoose](#apidoc.module.mockgoose)
1.  [function <span class="apidocSignatureSpan">mockgoose.</span>ConnectionWrapper (functionName, mongoose, connectionString)](#apidoc.element.mockgoose.ConnectionWrapper)
1.  [function <span class="apidocSignatureSpan">mockgoose.</span>Mockgoose (mongooseObj)](#apidoc.element.mockgoose.Mockgoose)
1.  object <span class="apidocSignatureSpan">mockgoose.</span>ConnectionWrapper.prototype
1.  object <span class="apidocSignatureSpan">mockgoose.</span>Mockgoose.prototype
1.  object <span class="apidocSignatureSpan">mockgoose.</span>mockgoose_helper

#### [module mockgoose.ConnectionWrapper](#apidoc.module.mockgoose.ConnectionWrapper)
1.  [function <span class="apidocSignatureSpan">mockgoose.</span>ConnectionWrapper (functionName, mongoose, connectionString)](#apidoc.element.mockgoose.ConnectionWrapper.ConnectionWrapper)

#### [module mockgoose.ConnectionWrapper.prototype](#apidoc.module.mockgoose.ConnectionWrapper.prototype)
1.  [function <span class="apidocSignatureSpan">mockgoose.ConnectionWrapper.prototype.</span>run (args)](#apidoc.element.mockgoose.ConnectionWrapper.prototype.run)

#### [module mockgoose.Mockgoose](#apidoc.module.mockgoose.Mockgoose)
1.  [function <span class="apidocSignatureSpan">mockgoose.</span>Mockgoose (mongooseObj)](#apidoc.element.mockgoose.Mockgoose.Mockgoose)

#### [module mockgoose.Mockgoose.prototype](#apidoc.module.mockgoose.Mockgoose.prototype)
1.  [function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getMemoryStorageName ()](#apidoc.element.mockgoose.Mockgoose.prototype.getMemoryStorageName)
1.  [function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getMockConnectionString (port)](#apidoc.element.mockgoose.Mockgoose.prototype.getMockConnectionString)
1.  [function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getOpenPort ()](#apidoc.element.mockgoose.Mockgoose.prototype.getOpenPort)
1.  [function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getTempDBPath ()](#apidoc.element.mockgoose.Mockgoose.prototype.getTempDBPath)
1.  [function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>mockConnectCalls (connection)](#apidoc.element.mockgoose.Mockgoose.prototype.mockConnectCalls)
1.  [function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>prepareStorage ()](#apidoc.element.mockgoose.Mockgoose.prototype.prepareStorage)

#### [module mockgoose.mockgoose_helper](#apidoc.module.mockgoose.mockgoose_helper)
1.  [function <span class="apidocSignatureSpan">mockgoose.mockgoose_helper.</span>MockgooseHelper (mongoose, mockgoose)](#apidoc.element.mockgoose.mockgoose_helper.MockgooseHelper)



# <a name="apidoc.module.mockgoose"></a>[module mockgoose](#apidoc.module.mockgoose)

#### <a name="apidoc.element.mockgoose.ConnectionWrapper"></a>[function <span class="apidocSignatureSpan">mockgoose.</span>ConnectionWrapper (functionName, mongoose, connectionString)](#apidoc.element.mockgoose.ConnectionWrapper)
- description and source-code
```javascript
function ConnectionWrapper(functionName, mongoose, connectionString) {
    this.functionName = functionName;
    this.mongoose = mongoose;
    this.functionCode = mongoose[functionName];
    this.connectionString = connectionString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mockgoose.Mockgoose"></a>[function <span class="apidocSignatureSpan">mockgoose.</span>Mockgoose (mongooseObj)](#apidoc.element.mockgoose.Mockgoose)
- description and source-code
```javascript
function Mockgoose(mongooseObj) {
    this.mongodHelper = new mongodb_prebuilt_1.MongodHelper();
    this.debug = Debug('Mockgoose');
    this.helper = new mockgoose_helper_1.MockgooseHelper(mongooseObj, this);
    this.mongooseObj = mongooseObj;
    this.mongooseObj.mocked = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mockgoose.ConnectionWrapper"></a>[module mockgoose.ConnectionWrapper](#apidoc.module.mockgoose.ConnectionWrapper)

#### <a name="apidoc.element.mockgoose.ConnectionWrapper.ConnectionWrapper"></a>[function <span class="apidocSignatureSpan">mockgoose.</span>ConnectionWrapper (functionName, mongoose, connectionString)](#apidoc.element.mockgoose.ConnectionWrapper.ConnectionWrapper)
- description and source-code
```javascript
function ConnectionWrapper(functionName, mongoose, connectionString) {
    this.functionName = functionName;
    this.mongoose = mongoose;
    this.functionCode = mongoose[functionName];
    this.connectionString = connectionString;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mockgoose.ConnectionWrapper.prototype"></a>[module mockgoose.ConnectionWrapper.prototype](#apidoc.module.mockgoose.ConnectionWrapper.prototype)

#### <a name="apidoc.element.mockgoose.ConnectionWrapper.prototype.run"></a>[function <span class="apidocSignatureSpan">mockgoose.ConnectionWrapper.prototype.</span>run (args)](#apidoc.element.mockgoose.ConnectionWrapper.prototype.run)
- description and source-code
```javascript
run = function (args) {
    this.originalArguments = args;
    var mockedArgs = args;
    mockedArgs[0] = this.connectionString;
    return this.functionCode.apply(this.mongoose, mockedArgs);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mockgoose.Mockgoose"></a>[module mockgoose.Mockgoose](#apidoc.module.mockgoose.Mockgoose)

#### <a name="apidoc.element.mockgoose.Mockgoose.Mockgoose"></a>[function <span class="apidocSignatureSpan">mockgoose.</span>Mockgoose (mongooseObj)](#apidoc.element.mockgoose.Mockgoose.Mockgoose)
- description and source-code
```javascript
function Mockgoose(mongooseObj) {
    this.mongodHelper = new mongodb_prebuilt_1.MongodHelper();
    this.debug = Debug('Mockgoose');
    this.helper = new mockgoose_helper_1.MockgooseHelper(mongooseObj, this);
    this.mongooseObj = mongooseObj;
    this.mongooseObj.mocked = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mockgoose.Mockgoose.prototype"></a>[module mockgoose.Mockgoose.prototype](#apidoc.module.mockgoose.Mockgoose.prototype)

#### <a name="apidoc.element.mockgoose.Mockgoose.prototype.getMemoryStorageName"></a>[function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getMemoryStorageName ()](#apidoc.element.mockgoose.Mockgoose.prototype.getMemoryStorageName)
- description and source-code
```javascript
getMemoryStorageName = function () {
    return "ephemeralForTest";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mockgoose.Mockgoose.prototype.getMockConnectionString"></a>[function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getMockConnectionString (port)](#apidoc.element.mockgoose.Mockgoose.prototype.getMockConnectionString)
- description and source-code
```javascript
getMockConnectionString = function (port) {
    var dbName = 'mockgoose-temp-db-' + uuidV4();
    var connectionString = "mongodb://localhost:" + port + "/" + dbName;
    return connectionString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mockgoose.Mockgoose.prototype.getOpenPort"></a>[function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getOpenPort ()](#apidoc.element.mockgoose.Mockgoose.prototype.getOpenPort)
- description and source-code
```javascript
getOpenPort = function () {
    return new Promise(function (resolve, reject) {
        portfinder.getPort({ port: 27017 }, function (err, port) {
            if (err) {
                reject(err);
            }
            else {
                resolve(port);
            }
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mockgoose.Mockgoose.prototype.getTempDBPath"></a>[function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>getTempDBPath ()](#apidoc.element.mockgoose.Mockgoose.prototype.getTempDBPath)
- description and source-code
```javascript
getTempDBPath = function () {
    return new Promise(function (resolve, reject) {
        var tempDir = path.resolve(os.tmpdir(), "mockgoose", Date.now().toString());
        fs.ensureDir(tempDir, function (err) {
            if (err)
                throw err;
            resolve(tempDir);
        });
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mockgoose.Mockgoose.prototype.mockConnectCalls"></a>[function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>mockConnectCalls (connection)](#apidoc.element.mockgoose.Mockgoose.prototype.mockConnectCalls)
- description and source-code
```javascript
mockConnectCalls = function (connection) {
    var createConnection = new ConnectionWrapper('createConnection', this.mongooseObj, connection);
    this.mongooseObj.createConnection = function () { return createConnection.run(arguments); };
    var connect = new ConnectionWrapper('connect', this.mongooseObj, connection);
    this.mongooseObj.connect = function () { return connect.run(arguments); };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mockgoose.Mockgoose.prototype.prepareStorage"></a>[function <span class="apidocSignatureSpan">mockgoose.Mockgoose.prototype.</span>prepareStorage ()](#apidoc.element.mockgoose.Mockgoose.prototype.prepareStorage)
- description and source-code
```javascript
prepareStorage = function () {
    var _this = this;
    return new Promise(function (resolve, reject) {
        var tempDBPathPromise = _this.getTempDBPath();
        var openPortPromise = _this.getOpenPort();
        Promise.all([tempDBPathPromise, openPortPromise]).then(function (promiseValues) {
            var dbPath = promiseValues[0];
            var openPort = promiseValues[1].toString();
            var storageEngine = _this.getMemoryStorageName();
            var mongodArgs = [
                '--port', openPort,
                '--storageEngine', storageEngine,
                '--dbpath', dbPath
            ];
            _this.debug("@prepareStorage mongod args, " + mongodArgs);
            _this.mongodHelper.mongoBin.commandArguments = mongodArgs;
            _this.mongodHelper.run().then(function () {
                var connectionString = _this.getMockConnectionString(openPort);
                _this.mockConnectCalls(connectionString);
                resolve();
            }, function (e) {
                throw e;
                // return this.prepareStorage();
            });
        });
    });
}
```
- example usage
```shell
...
You simply require Mongoose and Mockgoose and wrap Mongoose with Mockgoose.

'''javascript
var mongoose = require('mongoose');
var Mockgoose = require('mockgoose').Mockgoose;
var mockgoose = new Mockgoose(mongoose);

mockgoose.prepareStorage().then(function() {
	// mongoose connection		
});
'''

Once Mongoose has been wrapped by Mockgoose connect() will be intercepted by Mockgoose so that no MongoDB instance is created.

## Mocha
...
```



# <a name="apidoc.module.mockgoose.mockgoose_helper"></a>[module mockgoose.mockgoose_helper](#apidoc.module.mockgoose.mockgoose_helper)

#### <a name="apidoc.element.mockgoose.mockgoose_helper.MockgooseHelper"></a>[function <span class="apidocSignatureSpan">mockgoose.mockgoose_helper.</span>MockgooseHelper (mongoose, mockgoose)](#apidoc.element.mockgoose.mockgoose_helper.MockgooseHelper)
- description and source-code
```javascript
function MockgooseHelper(mongoose, mockgoose) {
    this.mongoose = mongoose;
    this.mockgoose = mockgoose;
    this.debug = Debug('MockgooseHelper');
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
