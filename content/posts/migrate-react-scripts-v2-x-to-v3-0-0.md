+++
title = "Migrate react-scripts v2.x to v3.0.0"
date = "2019-09-05"
draft = false
pinned = false
image = "/img/react-scripts.png"
+++
## npm run build fails to minify

Before **react-scripts@2.0.0**, this problem was caused by third party node_modules using modern JavaScript features because the minifier couldn't handle them during the build. This has been solved by compiling standard modern JavaScript features inside node_modules in **react-scripts@2.0.0** and higher.

If you're seeing this error, you're likely using an old version of react-scripts. You can either fix it by avoiding a dependency that uses modern syntax, or by upgrading to react-scripts@>=2.0.0 and following the migration instructions in the changelog.



## Update react-scripts

> In order to update react-scripts to the latest version, according to release notes, you should run the following command inside your project’s directory terminal:

` npm install --save --save-exact react-scripts@3.0.0`

during an update, you may see that react-scripts package depends on a different version of some of your dependencies (ex. eslint , or any other dependency). In that case, you can remove explicitly provided dependencies it clashes with from your package.json file (all except typescript ) and then — re-run installation command above. In case of a typescript, you’ll need to type and save its version inside package.json. This way step-by-step you’ll trust react-scripts to install and maintain dependencies it relies on (and will clean your package.json file as a slight bonus).

## Migrate rules from TSLint to ESLint

* Next big thing might be moving all of your Typescript linting rules from tslint.json into .eslintrc :
* if you’re starting from a scratch, create an empty .eslintrc file in the root of your project’s directory and add following basic configuration there.
