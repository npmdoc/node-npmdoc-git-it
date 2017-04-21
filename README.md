# npmdoc-git-it

#### api documentation for  git-it (v1.6.9)  [![npm package](https://img.shields.io/npm/v/npmdoc-git-it.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-git-it) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-git-it.svg)](https://travis-ci.org/npmdoc/node-npmdoc-git-it)

#### Terminal app for learning Git and GitHub

[![NPM](https://nodei.co/npm/git-it.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/git-it)

- [https://npmdoc.github.io/node-npmdoc-git-it/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-git-it/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-git-it/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-git-it/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-git-it/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-git-it/build/screenCapture.npmPackageDependencyTree.svg)



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
