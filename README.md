# api documentation for  [ember-cli-gravatar (v3.8.1)](https://github.com/johnotander/ember-cli-gravatar#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ember-cli-gravatar.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ember-cli-gravatar) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ember-cli-gravatar.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ember-cli-gravatar)
#### Component for gravatar image tags

[![NPM](https://nodei.co/npm/ember-cli-gravatar.png?downloads=true)](https://www.npmjs.com/package/ember-cli-gravatar)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ember-cli-gravatar/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ember-cli-gravatar_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ember-cli-gravatar/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ember-cli-gravatar/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ember-cli-gravatar/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "John Otander"
    },
    "bugs": {
        "url": "https://github.com/johnotander/ember-cli-gravatar/issues"
    },
    "dependencies": {
        "ember-cli-babel": "^5.1.6",
        "ember-cli-htmlbars": "^1.0.3"
    },
    "description": "Component for gravatar image tags",
    "devDependencies": {
        "broccoli-asset-rev": "^2.4.2",
        "ember-ajax": "0.7.1",
        "ember-cli": "2.4.3",
        "ember-cli-app-version": "^1.0.0",
        "ember-cli-dependency-checker": "^1.2.0",
        "ember-cli-htmlbars": "^1.0.3",
        "ember-cli-htmlbars-inline-precompile": "^0.3.1",
        "ember-cli-inject-live-reload": "^1.4.0",
        "ember-cli-qunit": "^1.4.0",
        "ember-cli-release": "0.2.8",
        "ember-cli-sri": "^2.1.0",
        "ember-cli-uglify": "^1.2.0",
        "ember-data": "^2.4.2",
        "ember-disable-prototype-extensions": "^1.1.0",
        "ember-export-application-global": "^1.0.5",
        "ember-load-initializers": "^0.5.1",
        "ember-resolver": "^2.0.3",
        "ember-try": "^0.2.2",
        "loader.js": "^4.0.1"
    },
    "directories": {
        "doc": "doc",
        "test": "tests"
    },
    "dist": {
        "shasum": "9efb6295b7f906984e31a25e166aca1d8eff653f",
        "tarball": "https://registry.npmjs.org/ember-cli-gravatar/-/ember-cli-gravatar-3.8.1.tgz"
    },
    "ember-addon": {
        "configPath": "tests/dummy/config"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "5eda531c72ab61ea2b50e200db4da6bc72a59ece",
    "homepage": "https://github.com/johnotander/ember-cli-gravatar#readme",
    "keywords": [
        "gravatar",
        "avatar",
        "component",
        "ember-addon"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "johno",
            "email": "johnotander@gmail.com"
        }
    ],
    "name": "ember-cli-gravatar",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/johnotander/ember-cli-gravatar.git"
    },
    "scripts": {
        "build": "ember build",
        "start": "ember server",
        "test": "ember try:testall"
    },
    "version": "3.8.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ember-cli-gravatar](#apidoc.module.ember-cli-gravatar)
1.  [function <span class="apidocSignatureSpan">ember-cli-gravatar.</span>included (app)](#apidoc.element.ember-cli-gravatar.included)
1.  string <span class="apidocSignatureSpan">ember-cli-gravatar.</span>name



# <a name="apidoc.module.ember-cli-gravatar"></a>[module ember-cli-gravatar](#apidoc.module.ember-cli-gravatar)

#### <a name="apidoc.element.ember-cli-gravatar.included"></a>[function <span class="apidocSignatureSpan">ember-cli-gravatar.</span>included (app)](#apidoc.element.ember-cli-gravatar.included)
- description and source-code
```javascript
function included(app) {
  // workaround for https://github.com/ember-cli/ember-cli/issues/3718
  if (typeof app.import !== 'function' && app.app) {
    app = app.app;
  }
  this.app = app;
  this._super.included(app);

  app.import(app.bowerDirectory + '/blueimp-md5/js/md5.js');
  app.import('vendor/ember-cli-gravatar/md5-shim.js', {
    type: 'vendor',
    exports: { 'md5': ['md5'] }
  });
}
```
- example usage
```shell
...

included: function included(app) {
  // workaround for https://github.com/ember-cli/ember-cli/issues/3718
  if (typeof app.import !== 'function' && app.app) {
    app = app.app;
  }
  this.app = app;
  this._super.included(app);

  app.import(app.bowerDirectory + '/blueimp-md5/js/md5.js');
  app.import('vendor/ember-cli-gravatar/md5-shim.js', {
    type: 'vendor',
    exports: { 'md5': ['md5'] }
  });
}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
