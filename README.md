> 本项目前后端分离，前端参考 [小米商城](www.mi.com) 实现。

> 这是本项目的前端，后端请移步到[项目后端](https://github.com/Miki-Hunter/-store-server-django)

> 此即[原博主项目-前端](https://github.com/hai-27/vue-store)，用作备份。后端使用 django + drf 进行重构，前后端结合使用。

> [原作者项目-后端](https://github.com/hai-27/store-server) node.js + Koa框架实现

> [重构后项目-后端](https://github.com/Miki-Hunter/-store-server-django) django + drf 实现

## 项目简介

本项目前后端分离，前端基于`Vue`+`Vue-router`+`Vuex`+`Element-ui`+`Axios`，参考小米商城实现。后端基于`Node.js(Koa框架)`+`Mysql`实现。

前端包含了11个页面：首页、登录、注册、全部商品、商品详情页、关于我们、我的收藏、购物车、订单结算页面、我的订单以及错误处理页面。

实现了商品的展示、商品分类查询、关键字搜索商品、商品详细信息展示、登录、注册、用户购物车、订单结算、用户订单、用户收藏列表以及错误处理功能。

## 技术栈

- **前端：**`Vue`+`Vue-router`+`Vuex`+`Element-ui`+`Axios`

## 功能模块

### 登录

页面使用了element-ui的`Dialog`实现弹出蒙版对话框的效果，`登录`按钮设置在App.vue根组件，通过`vuex`中的`showLogin`状态控制登录框是否显示。

这样设计是为了既可以通过点击页面中的按钮登录，也可以是用户访问需要登录验证的页面或后端返回需要验证登录的提示后自动弹出登录框，减少了页面的跳转，简化用户操作。

用户输入的数据往往是不可靠的，所以本项目前后端都对登录信息进行了校验，前端基于element-ui的表单校验方式，自定义了校验规则进行校验。

### 注册

页面同样使用了element-ui的`Dialog`实现弹出蒙版对话框的效果，`注册`按钮设置在App.vue根组件，通过父子组件传值控制注册框是否显示。

用户输入的数据往往是不可靠的，所以本项目前后端同样都对注册信息进行了校验，前端基于element-ui的表单校验方式，自定义了校验规则进行校验。

### 购物车
购物车采用vuex实现，页面效果参考了小米商城的购物车。

详细实现过程请看：[基于Vuex实现小米商城购物车](https://juejin.im/post/5e660ef9518825490276748a)

### 运行项目
```
1. Clone project

git clone https://github.com/Miki-Hunter/vue-store-1.0.git

2. Project setup

cd vue-store-1.0
npm install

3. Compiles and hot-reloads for development

npm run serve

4. Compiles and minifies for production

npm run build
```
