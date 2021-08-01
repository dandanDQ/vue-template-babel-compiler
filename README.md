# vue-template-babel-compiler
Enable `Optional Chaining(?.)`, `Nullish Coalescing(??)` and many new ES syntax for [Vue.js SFC](https://vuejs.org/v2/guide/single-file-components.html) based on [Babel](https://babeljs.io/).

<p align="center">
  <a href="https://www.npmjs.com/package/vue-template-babel-compiler">
    <img
    src="https://img.shields.io/npm/v/vue-template-babel-compiler.svg?sanitize=true"
    alt="Version">
  </a>
  <a href="https://github.com/JuniorTour/vue-template-babel-compiler">
    <img
    src="https://img.shields.io/github/last-commit/JuniorTour/vue-template-babel-compiler?sanitize=true"
    alt="last-commit">
  </a>
</p>

## DEMO
![DEMO](https://user-images.githubusercontent.com/14243906/127761300-076db45a-cdce-4fda-bd02-1f4fa96de6d8.png)

## Features
- All features of [vue-template-compiler](https://github.com/vuejs/vue/tree/dev/packages/vue-template-compiler#readme) && [vue-template-es2015-compiler](https://github.com/vuejs/vue-template-es2015-compiler)
- new ES syntax: `Optional Chaining`, `Bigint`, `Nullish Coalescing` and more
- Customization syntax, babel plugin...

## Usage
### 1. Install
``` bash
npm install --save-dev vue-template-babel-compiler
```

### 2. Config
#### 1. [vue-cli](https://cli.vuejs.org/guide/webpack.html#modifying-options-of-a-loader)
``` js
// vue.config.js
module.exports = {
    chainWebpack: config => {
        config.module
            .rule('vue')
            .use('vue-loader')
            .tap(options => {
                options.compiler = require('vue-template-babel-compiler')
                return options
            })
    }
}
```

#### 2. [nuxt.js](https://nuxtjs.org/docs/2.x/features/configuration#extend-webpack-to-load-audio-files)
``` js
// nuxt.config.js
```

#### 3. [webpack](https://cli.vuejs.org/guide/webpack.html#modifying-options-of-a-loader)
``` js
// your webpack.config.js which config vue-loader
```


### Welcome for Issues && PR.
