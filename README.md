# my-project

> Vue-TypeScript-electron Demo


[![forthebadge](https://forthebadge.com/images/badges/made-with-vue.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/powered-by-electricity.svg)](https://forthebadge.com)

[![TypeScript](https://badges.frapsoft.com/typescript/code/typescript.svg?v=101)](https://github.com/ellerbrock/typescript-badges/)

## 简介
这是Vue-Cli 3.0、TypeScript、electron初始化得到Demo。构建Typescript、electron和Vue项目是一件麻烦的事情，尝试过各种方案后发现使用[vue-cli-plugin-electron-builder](https://github.com/nklayman/vue-cli-plugin-electron-builder) 是目前最好的选择。
## 使用

### 方法一:克隆本仓库
```
git clone https://github.com/Robinsir/vue-electron-typescript.git
cd vue-electron-typescript
npm i
npm run electron:serve #或者npm run dev
```
### 方法二:使用Vue-Cli 3.0插件
使用Vue-Cli创建此项目有更加自由的选择。可以根据以下步骤创建：

#### 首先**必须安装Vue-Cli 3.0**
```
vue -V #查询当前Vue-cli 版本
npm uninstall vue-cli #如果版本低于3.0,则要删除并重新安装
npm i -g @vue/cli  #安装vue-cli 3.0
```
#### 初始化一个Vue-Cli 3.0项目
```
vue create my-project  #创建项目

? Please pick a preset: Manually select features
? Check the features needed for your project: Babel, TS, Router, Vuex, Linter
? Use class-style component syntax? No # 是否使用class风格的组件定义
? Use Babel alongside TypeScript for auto-detected polyfills? (Y/n)Yes
? Pick a linter / formatter config: TSLint
? Pick additional lint features: Lint on save
? Where do you prefer placing config for Babel, PostCSS, ESLint, etc.? In dedicated config files # 分离配置文件

cd my-project
vue add electron-builder #添加electron插件
npm run electron:serve #运行electron
```

## 脚本


### 编译以及热更新
```
npm run electron:serve
```

### 构建应用
```
npm run electron:build
```

### Run your tests
```
npm run test
```

### Lints and fixes files
```
npm run lint
```

### 更多
 [vue-cli-plugin-electron-builder](https://github.com/nklayman/vue-cli-plugin-electron-builder)