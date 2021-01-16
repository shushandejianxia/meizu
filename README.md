# 01-vue_shop

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).

# 项目开始
## 全局安装vue脚手架并创建项目
>1、使用命令`npm install -g @vue/cli` 
>2、打开vue界面`vue ui`
>3、创建项目，配置路由
>4、配置Element-UI组件库
 ```
 1、在vue可视化界面中，添加插件`vue-cli-plugin-element`
 2、配置插件：选择按需导入
 ```
>5、配置axios库
 ```
 1、选择依赖
 2、添加依赖`axios`
 ```
 >6、初始化git远程仓库
 >7、将项目托管到码云


 ## 运行项目
 > `npm run serve` 或 `yarn serve`

 ## 项目优化
 ### 生成打包报告
 >1、可以运行  `vue-cli-service build --report`
 >2、也可以通过ui面板中的控制台和分析面板，可以方便的看到项目中存在的问题
 ### 修改webpack的默认配置
 > 在项目的根目录中，创建vue.config.js，对项目的打包发布过程做自定义的配置`https://cli.vuejs.org/zh/config/#vue-config-js`

 ## 上线
 ### 使用node创建服务器将dist目录开放

 ## 使用pm2管理应用 
 > 1、`npm i pm2 -g`
 > 2、启动项目:`pm2 start 脚本 --name 自定义名称` === ` pm2 start .\app.js --name web_vue_shop`
 > 3、查看运行的项目:`pm2 ls`
 > 4、重启项目:`pm2 restart 自定义名称`
 > 4、停止项目:`pm2 stop 自定义名称` || `pm2 stop id`
 > 5、删除项目:`pm2 delete 自定义名称`