# npmtest-git-it

#### basic test coverage for  git-it (v1.6.9)  [![npm package](https://img.shields.io/npm/v/npmtest-git-it.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-git-it) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-git-it.svg)](https://travis-ci.org/npmtest/node-npmtest-git-it)

#### Terminal app for learning Git and GitHub

[![NPM](https://nodei.co/npm/git-it.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/git-it)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-git-it/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-git-it/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-git-it/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-git-it/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-git-it/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-git-it/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-git-it/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-git-it/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-git-it/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-git-it/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-git-it/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-git-it/build/test-report.html](https://npmtest.github.io/node-npmtest-git-it/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-git-it/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-git-it/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-git-it/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-git-it/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-git-it/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-git-it/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-git-it/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-git-it/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "git-it",
    "version": "1.6.9",
    "description": "Terminal app for learning Git and GitHub",
    "main": "index.js",
    "bin": "./git-it.js",
    "scripts": {
        "build": "node guide/buildpages.js && node guide/buildpages.js zhtw",
        "build-english": "node guide/buildpages.js",
        "build-zhtw": "node guide/buildpages.js zhtw",
        "copy-guide": "cp -r ./guide ./.guide",
        "git-co": "git checkout gh-pages && git reset --hard origin/gh-pages",
        "paste-guide": "cp -r ./.guide/* .. && rm -rf ./.guide",
        "git-stage": "npm run copy-guide && npm run git-co && npm run paste-guide",
        "git-commit": "git add -A . && git commit -a -m 'gh-pages update'",
        "git-push": "git push origin gh-pages --force && git checkout master",
        "deploy": "npm run git-stage && npm run git-commit && npm run git-push"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/jlord/git-it.git"
    },
    "author": "Jessica Lord",
    "license": "BSD-2-Clause",
    "bugs": {
        "url": "https://github.com/jlord/git-it/issues"
    },
    "dependencies": {
        "concat-stream": "~1.2.1",
        "ecstatic": "^0.5.4",
        "github-oauth": "0.0.4",
        "glob": "^3.2.11",
        "handlebars": "^2.0.0-alpha.4",
        "marked": "^0.3.2",
        "request": "~2.30.0",
        "workshopper-jlord": "^0.0.6",
        "cheerio": "~0.17.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
