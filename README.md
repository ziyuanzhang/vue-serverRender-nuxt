# vue-server-render-nuxt

> Nuxt.js project

## Build Setup

``` bash
# install dependencies
$ npm install # Or yarn install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build 
$ npm start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, checkout the [Nuxt.js docs](https://github.com/nuxt/nuxt.js).


支持scss：
1.安装一些loader
   npm i node-sass sass-loader scss-loader --save-dev
2.>在nuxt.config.js中配置(需要全局使用的scss)
module.exports = {
    css: [
         {
               src: '*.scss',
               lang: 'scss'
          }
    ]  
}
