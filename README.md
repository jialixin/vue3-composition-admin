<p align="center">
  <a href="https://github.com/rcyj-FED/vue3-composition-admin-docs" target="_blank">
    <img width="180" src="https://github.com/rcyj-FED/vue3-composition-admin-docs/blob/main/docs/.vuepress/public/icons/android-chrome-192x192.png" alt="logo">
  </a>
</p>

<p align="center">
  <a href="https://github.com/vuejs/vue">
    <img src="https://img.shields.io/badge/vue-3.0-brightgreen.svg" alt="vue">
  </a>
  <a href="https://github.com/element-plus/element-plus">
    <img src="https://img.shields.io/badge/element--plus-1.x-blue" alt="element-plus">
  </a>
  <a href="https://github.com/vuejs/vuex">
    <img src="https://img.shields.io/badge/vuex-4.0-brightgreen" alt="vuex">
  </a>
   <a href="https://github.com/intlify/vue-i18n-next">
    <img src="https://img.shields.io/badge/vue--i18n--next-9.0-brightgreen" alt="vue-i18n-next">
   </a>
   <a href="https://github.com/npm/npm">
    <img src="https://img.shields.io/badge/npm-6.1.8-blue" alt="npm">
   </a>
</p>

> vue3-composition-admin 是一个管理端模板解决方案，它是基于vue3,ts和element-plus，项目都是以composition api风格编写。

## 简介

项目的基础版本出自于源于花裤衩大佬的 vue-element-admin。

版本：

vue2+js版本：[vue-element-admin](https://github.com/PanJiaChen/vue-element-admin)

vue2+ts版本：[vue-typescript-admin-template](https://github.com/Armour/vue-typescript-admin-template) 

vue3 发布之后，性能增强，速度vue2的倍数，打包体积都在减小（treeshaking），composition api 增加了项目可读性。

项目目的：
  - 保持技术的先进性，跟上技术发展
  - 作为公司定制组件的代码demo集合
  - 解决方案集合
  - 统一技术标准


## HighLight

项目均已最新技术实现，Vue3配套升级全家桶和涉及的插件组件等

项目采用技术:
- vue3 + composition api
- typescript3.9
- sass (dart sass)
- [echats5](https://github.com/apache/echarts)

vue next 系列:
- [element-plus](https://github.com/element-plus/element-plus)
- [vue-router-next](https://github.com/vuejs/vue-router-next)
- [vuex-4.0](https://github.com/vuejs/vuex)
- [vue-vue-i18n-next](https://github.com/panter/vue-i18next)


## Document

- [文档地址](https://rcyj-fed.github.io/vue3-composition-admin-docs/)
- [文档项目git地址](https://github.com/rcyj-FED/vue3-composition-admin-docs)


## Setup

项目主要是前端和mock server（node）

### Mock

后台模拟服务器和其他版本不同，采用koa2+Faker进行模拟。

- [Koa2](https://github.com/koajs/koa)
- [Faker](https://github.com/Marak/faker.js)

启动mock server:

```shell
     "mock": "cd mock && ts-node-dev mock.ts"
```

### vue admin

多环境启动：

```shell
    "serve:dev": "cross-env NODE_ENV=development dotenv -e .env.dev.serve vue-cli-service serve",
    "build:dev": "cross-env NODE_ENV=production  dotenv -e .env.dev.build vue-cli-service build",
    "serve:test": "cross-env NODE_ENV=development dotenv -e .env.test.serve vue-cli-service serve",
    "build:test": "cross-env NODE_ENV=production  dotenv -e .env.test.build vue-cli-service build",
    "serve:prod": "cross-env NODE_ENV=development dotenv -e .env.prod.serve vue-cli-service serve",
    "build:prod": "cross-env NODE_ENV=production  dotenv -e .env.prod.build vue-cli-service build",
```


快捷启动(同时启动前后端)：

```shell
    "start": "concurrently \"npm run mock\" \"npm run serve:dev\"",
```




## Browsers support

Modern browsers and Internet Explorer 10+.

| [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/edge/edge_48x48.png" alt="IE / Edge" width="24px" height="24px" />](https://godban.github.io/browsers-support-badges/)</br>IE / Edge | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/firefox/firefox_48x48.png" alt="Firefox" width="24px" height="24px" />](https://godban.github.io/browsers-support-badges/)</br>Firefox | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/chrome/chrome_48x48.png" alt="Chrome" width="24px" height="24px" />](https://godban.github.io/browsers-support-badges/)</br>Chrome | [<img src="https://raw.githubusercontent.com/alrra/browser-logos/master/src/safari/safari_48x48.png" alt="Safari" width="24px" height="24px" />](https://godban.github.io/browsers-support-badges/)</br>Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge | last 2 versions | last 2 versions | last 2 versions |

## License

[MIT](https://github.com/rcyj-FED/vue3-composition-admin/blob/main/LICENSE)

Copyright (c) 2021-present 人才有价


