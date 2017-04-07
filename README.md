# api documentation for  [react-waypoint (v5.2.1)](https://github.com/brigade/react-waypoint)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-waypoint.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-waypoint) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-waypoint.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-waypoint)
#### A React component to execute a function whenever you scroll to an element.

[![NPM](https://nodei.co/npm/react-waypoint.png?downloads=true)](https://www.npmjs.com/package/react-waypoint)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-react-waypoint%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brigade Engineering"
    },
    "bugs": {
        "url": "https://github.com/brigade/react-waypoint/issues"
    },
    "dependencies": {
        "consolidated-events": "^1.0.1"
    },
    "description": "A React component to execute a function whenever you scroll to an element.",
    "devDependencies": {
        "@types/react": "^0.14.55",
        "babel": "^6.23.0",
        "babel-cli": "^6.23.0",
        "babel-core": "^6.23.1",
        "babel-loader": "^6.4.0",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-react-jsx": "^6.23.0",
        "babel-preset-es2015": "^6.22.0",
        "eslint": "^3.17.1",
        "eslint-config-brigade": "^3.2.1",
        "eslint-plugin-react": "^6.10.0",
        "in-publish": "^2.0.0",
        "jasmine-core": "^2.1.3",
        "karma": "^1.5.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-cli": "^1.0.1",
        "karma-firefox-launcher": "^1.0.1",
        "karma-jasmine": "^1.1.0",
        "karma-webpack": "^1.8.1",
        "react": "^15.0.0",
        "react-dom": "^15.0.0",
        "rimraf": "^2.6.1",
        "safe-publish-latest": "^1.1.1",
        "webpack": "^1.14.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0c5e13600df5e59c0e1abc29a527054ce3db6909",
        "tarball": "https://registry.npmjs.org/react-waypoint/-/react-waypoint-5.2.1.tgz"
    },
    "gitHead": "f00df845cdb1d96d21a015bca246ab51e1ec39f1",
    "homepage": "https://github.com/brigade/react-waypoint",
    "keywords": [
        "react",
        "component",
        "react-component",
        "scroll",
        "onscroll"
    ],
    "license": "MIT",
    "main": "build/waypoint.js",
    "maintainers": [
        {
            "name": "bigsley",
            "email": "bigsley@gmail.com"
        },
        {
            "name": "brigade",
            "email": "services+npm@brigade.com"
        },
        {
            "name": "janpaul123",
            "email": "me@janpaulposma.nl"
        },
        {
            "name": "lencioni",
            "email": "joe.lencioni@gmail.com"
        },
        {
            "name": "trotzig",
            "email": "henric.trotzig@gmail.com"
        }
    ],
    "name": "react-waypoint",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/brigade/react-waypoint.git"
    },
    "scripts": {
        "build": "npm run clean && babel src/ -d build/",
        "check-changelog": "expr $(git status --porcelain 2>/dev/null| grep \"^\\s*M.*CHANGELOG.md\" | wc -l) >/dev/null || (echo 'Please edit CHANGELOG.md' && exit 1)",
        "check-only-changelog-changed": "(expr $(git status --porcelain 2>/dev/null| grep -v \"CHANGELOG.md\" | wc -l) >/dev/null && echo 'Only CHANGELOG.md may have uncommitted changes' && exit 1) || exit 0",
        "clean": "rimraf build",
        "lint": "eslint . --ext .js,.jsx",
        "postversion": "git commit package.json CHANGELOG.md -m \"Version $npm_package_version\" && npm run tag && git push && git push --tags && npm publish",
        "prepublish": "in-publish && safe-publish-latest && npm run build || not-in-publish",
        "pretest": "npm run --silent lint",
        "preversion": "npm run test && npm run check-changelog && npm run check-only-changelog-changed",
        "tag": "git tag v$npm_package_version",
        "test": "npm run testonly",
        "testonly": "karma start --single-run",
        "testonly:watch": "karma start --no-single-run"
    },
    "types": "index.d.ts",
    "version": "5.2.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-waypoint](#apidoc.module.react-waypoint)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>getWindow ()](#apidoc.element.react-waypoint.getWindow)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.bottomOffset ()](#apidoc.element.react-waypoint.propTypes.bottomOffset)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.children ()](#apidoc.element.react-waypoint.propTypes.children)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.debug ()](#apidoc.element.react-waypoint.propTypes.debug)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.onEnter ()](#apidoc.element.react-waypoint.propTypes.onEnter)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.scrollableAncestor ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor)
1.  [function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.topOffset ()](#apidoc.element.react-waypoint.propTypes.topOffset)
1.  object <span class="apidocSignatureSpan">react-waypoint.</span>defaultProps
1.  object <span class="apidocSignatureSpan">react-waypoint.</span>propTypes
1.  string <span class="apidocSignatureSpan">react-waypoint.</span>above
1.  string <span class="apidocSignatureSpan">react-waypoint.</span>below
1.  string <span class="apidocSignatureSpan">react-waypoint.</span>displayName
1.  string <span class="apidocSignatureSpan">react-waypoint.</span>inside
1.  string <span class="apidocSignatureSpan">react-waypoint.</span>invisible

#### [module react-waypoint.defaultProps](#apidoc.module.react-waypoint.defaultProps)
1.  boolean <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>fireOnRapidScroll
1.  boolean <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>horizontal
1.  [function <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>onEnter ()](#apidoc.element.react-waypoint.defaultProps.onEnter)
1.  [function <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>onLeave ()](#apidoc.element.react-waypoint.defaultProps.onLeave)
1.  [function <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>onPositionChange ()](#apidoc.element.react-waypoint.defaultProps.onPositionChange)
1.  string <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>bottomOffset
1.  string <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>topOffset

#### [module react-waypoint.propTypes](#apidoc.module.react-waypoint.propTypes)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>bottomOffset ()](#apidoc.element.react-waypoint.propTypes.bottomOffset)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>children ()](#apidoc.element.react-waypoint.propTypes.children)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>debug ()](#apidoc.element.react-waypoint.propTypes.debug)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>fireOnRapidScroll ()](#apidoc.element.react-waypoint.propTypes.fireOnRapidScroll)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>horizontal ()](#apidoc.element.react-waypoint.propTypes.horizontal)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onEnter ()](#apidoc.element.react-waypoint.propTypes.onEnter)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onLeave ()](#apidoc.element.react-waypoint.propTypes.onLeave)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onPositionChange ()](#apidoc.element.react-waypoint.propTypes.onPositionChange)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>scrollableAncestor ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>topOffset ()](#apidoc.element.react-waypoint.propTypes.topOffset)

#### [module react-waypoint.propTypes.bottomOffset](#apidoc.module.react-waypoint.propTypes.bottomOffset)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>bottomOffset ()](#apidoc.element.react-waypoint.propTypes.bottomOffset.bottomOffset)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.bottomOffset.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.bottomOffset.isRequired)

#### [module react-waypoint.propTypes.children](#apidoc.module.react-waypoint.propTypes.children)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>children ()](#apidoc.element.react-waypoint.propTypes.children.children)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.children.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.children.isRequired)

#### [module react-waypoint.propTypes.debug](#apidoc.module.react-waypoint.propTypes.debug)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>debug ()](#apidoc.element.react-waypoint.propTypes.debug.debug)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.debug.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.debug.isRequired)

#### [module react-waypoint.propTypes.onEnter](#apidoc.module.react-waypoint.propTypes.onEnter)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onEnter ()](#apidoc.element.react-waypoint.propTypes.onEnter.onEnter)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.onEnter.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.onEnter.isRequired)

#### [module react-waypoint.propTypes.scrollableAncestor](#apidoc.module.react-waypoint.propTypes.scrollableAncestor)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>scrollableAncestor ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor.scrollableAncestor)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.scrollableAncestor.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor.isRequired)

#### [module react-waypoint.propTypes.topOffset](#apidoc.module.react-waypoint.propTypes.topOffset)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>topOffset ()](#apidoc.element.react-waypoint.propTypes.topOffset.topOffset)
1.  [function <span class="apidocSignatureSpan">react-waypoint.propTypes.topOffset.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.topOffset.isRequired)



# <a name="apidoc.module.react-waypoint"></a>[module react-waypoint](#apidoc.module.react-waypoint)

#### <a name="apidoc.element.react-waypoint.getWindow"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>getWindow ()](#apidoc.element.react-waypoint.getWindow)
- description and source-code
```javascript
getWindow = function () {
  if (typeof window !== 'undefined') {
    return window;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.bottomOffset"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.bottomOffset ()](#apidoc.element.react-waypoint.propTypes.bottomOffset)
- description and source-code
```javascript
propTypes.bottomOffset = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.children"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.children ()](#apidoc.element.react-waypoint.propTypes.children)
- description and source-code
```javascript
propTypes.children = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.debug"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.debug ()](#apidoc.element.react-waypoint.propTypes.debug)
- description and source-code
```javascript
propTypes.debug = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.onEnter"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.onEnter ()](#apidoc.element.react-waypoint.propTypes.onEnter)
- description and source-code
```javascript
propTypes.onEnter = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.scrollableAncestor"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.scrollableAncestor ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor)
- description and source-code
```javascript
propTypes.scrollableAncestor = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.topOffset"></a>[function <span class="apidocSignatureSpan">react-waypoint.</span>propTypes.topOffset ()](#apidoc.element.react-waypoint.propTypes.topOffset)
- description and source-code
```javascript
propTypes.topOffset = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.defaultProps"></a>[module react-waypoint.defaultProps](#apidoc.module.react-waypoint.defaultProps)

#### <a name="apidoc.element.react-waypoint.defaultProps.onEnter"></a>[function <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>onEnter ()](#apidoc.element.react-waypoint.defaultProps.onEnter)
- description and source-code
```javascript
function onEnter() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.defaultProps.onLeave"></a>[function <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>onLeave ()](#apidoc.element.react-waypoint.defaultProps.onLeave)
- description and source-code
```javascript
function onLeave() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.defaultProps.onPositionChange"></a>[function <span class="apidocSignatureSpan">react-waypoint.defaultProps.</span>onPositionChange ()](#apidoc.element.react-waypoint.defaultProps.onPositionChange)
- description and source-code
```javascript
function onPositionChange() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes"></a>[module react-waypoint.propTypes](#apidoc.module.react-waypoint.propTypes)

#### <a name="apidoc.element.react-waypoint.propTypes.bottomOffset"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>bottomOffset ()](#apidoc.element.react-waypoint.propTypes.bottomOffset)
- description and source-code
```javascript
bottomOffset = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.children"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>children ()](#apidoc.element.react-waypoint.propTypes.children)
- description and source-code
```javascript
children = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.debug"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>debug ()](#apidoc.element.react-waypoint.propTypes.debug)
- description and source-code
```javascript
debug = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.fireOnRapidScroll"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>fireOnRapidScroll ()](#apidoc.element.react-waypoint.propTypes.fireOnRapidScroll)
- description and source-code
```javascript
fireOnRapidScroll = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.horizontal"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>horizontal ()](#apidoc.element.react-waypoint.propTypes.horizontal)
- description and source-code
```javascript
horizontal = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.onEnter"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onEnter ()](#apidoc.element.react-waypoint.propTypes.onEnter)
- description and source-code
```javascript
onEnter = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.onLeave"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onLeave ()](#apidoc.element.react-waypoint.propTypes.onLeave)
- description and source-code
```javascript
onLeave = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.onPositionChange"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onPositionChange ()](#apidoc.element.react-waypoint.propTypes.onPositionChange)
- description and source-code
```javascript
onPositionChange = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.scrollableAncestor"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>scrollableAncestor ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor)
- description and source-code
```javascript
scrollableAncestor = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.topOffset"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>topOffset ()](#apidoc.element.react-waypoint.propTypes.topOffset)
- description and source-code
```javascript
topOffset = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes.bottomOffset"></a>[module react-waypoint.propTypes.bottomOffset](#apidoc.module.react-waypoint.propTypes.bottomOffset)

#### <a name="apidoc.element.react-waypoint.propTypes.bottomOffset.bottomOffset"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>bottomOffset ()](#apidoc.element.react-waypoint.propTypes.bottomOffset.bottomOffset)
- description and source-code
```javascript
bottomOffset = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.bottomOffset.isRequired"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.bottomOffset.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.bottomOffset.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes.children"></a>[module react-waypoint.propTypes.children](#apidoc.module.react-waypoint.propTypes.children)

#### <a name="apidoc.element.react-waypoint.propTypes.children.children"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>children ()](#apidoc.element.react-waypoint.propTypes.children.children)
- description and source-code
```javascript
children = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.children.isRequired"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.children.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.children.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes.debug"></a>[module react-waypoint.propTypes.debug](#apidoc.module.react-waypoint.propTypes.debug)

#### <a name="apidoc.element.react-waypoint.propTypes.debug.debug"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>debug ()](#apidoc.element.react-waypoint.propTypes.debug.debug)
- description and source-code
```javascript
debug = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.debug.isRequired"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.debug.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.debug.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes.onEnter"></a>[module react-waypoint.propTypes.onEnter](#apidoc.module.react-waypoint.propTypes.onEnter)

#### <a name="apidoc.element.react-waypoint.propTypes.onEnter.onEnter"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>onEnter ()](#apidoc.element.react-waypoint.propTypes.onEnter.onEnter)
- description and source-code
```javascript
onEnter = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.onEnter.isRequired"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.onEnter.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.onEnter.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes.scrollableAncestor"></a>[module react-waypoint.propTypes.scrollableAncestor](#apidoc.module.react-waypoint.propTypes.scrollableAncestor)

#### <a name="apidoc.element.react-waypoint.propTypes.scrollableAncestor.scrollableAncestor"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>scrollableAncestor ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor.scrollableAncestor)
- description and source-code
```javascript
scrollableAncestor = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.scrollableAncestor.isRequired"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.scrollableAncestor.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.scrollableAncestor.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-waypoint.propTypes.topOffset"></a>[module react-waypoint.propTypes.topOffset](#apidoc.module.react-waypoint.propTypes.topOffset)

#### <a name="apidoc.element.react-waypoint.propTypes.topOffset.topOffset"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.</span>topOffset ()](#apidoc.element.react-waypoint.propTypes.topOffset.topOffset)
- description and source-code
```javascript
topOffset = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-waypoint.propTypes.topOffset.isRequired"></a>[function <span class="apidocSignatureSpan">react-waypoint.propTypes.topOffset.</span>isRequired ()](#apidoc.element.react-waypoint.propTypes.topOffset.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
