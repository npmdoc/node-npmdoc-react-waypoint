# npmdoc-react-waypoint

#### api documentation for  [react-waypoint (v6.0.0)](https://github.com/brigade/react-waypoint)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-waypoint.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-waypoint) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-waypoint.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-waypoint)

#### A React component to execute a function whenever you scroll to an element.

[![NPM](https://nodei.co/npm/react-waypoint.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-waypoint)

- [https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-waypoint",
    "version": "6.0.0",
    "description": "A React component to execute a function whenever you scroll to an element.",
    "main": "build/waypoint.js",
    "types": "index.d.ts",
    "repository": {
        "type": "git",
        "url": "https://github.com/brigade/react-waypoint.git"
    },
    "homepage": "https://github.com/brigade/react-waypoint",
    "bugs": "https://github.com/brigade/react-waypoint/issues",
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
    "author": "Brigade Engineering",
    "license": "MIT",
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0",
        "prop-types": "^15.0.0"
    },
    "devDependencies": {
        "@types/react": "^15.0.21",
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
        "karma-webpack": "^2.0.3",
        "prop-types": "^15.5.4",
        "react": "^15.5.3",
        "react-dom": "^15.5.3",
        "rimraf": "^2.6.1",
        "safe-publish-latest": "^1.1.1",
        "webpack": "^2.3.3"
    },
    "keywords": [
        "react",
        "component",
        "react-component",
        "scroll",
        "onscroll"
    ],
    "dependencies": {
        "consolidated-events": "^1.0.1"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
