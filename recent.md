我在回忆自己前端的学习历程。

# 预备
介绍背景以及出发前的准备

## 前提知识储备

我在大学期间通过开设的课程学习到了 HTML，而对于 JavaScript 的掌握却是在工作之后才逐步了解的。

- [W3school](http://www.w3school.com.cn/) 去补充 HTML 章节、浏览器脚本下的 JavaScript、AJAX 两个章节。

-  [ECMAScript 6 入门](https://es6.ruanyifeng.com/) 补充 ES6 语法（JavaScript 书写方式的迭代）


##  前端背景了解

但我毕业后，前端已经告别了刀耕火种的Jquery时代，直至` 2019 年 7 月`，目前最流行的前端库分别是

-  [Vue](https://vuejs.org/) ，自动档，官方教程写得特别得体。
-  [React](https://reactjs.org/) ，手动挡，文档要差一些。

而国内有两个流行的开源 UI 库分别是

- 基于 Vue 的 [Element](https://element.eleme.cn/) 
- 基于 React 的 [Ant.Design](https://ant.design/)


# 出发

我通过[看、做、想](https://pjchender.blogspot.com/2016/08/blog-post.html)三个阶段来回想我的前端成长之路。

## 看 & 框架/库的掌握

我是从毕业后才开始代码的编写的，我很感谢我的师父给了我一个实习机会。而我接触的第一个前端框架是 Vue，项目中接触的第一个 UI 框架则是 Element UI。

但我会因为会关注到各种小细节而拖慢我对一个事物的理解。所以工作后的两个星期始终不得要领。我把 [Vue](<https://cn.vuejs.org/v2/guide/index.html>) 官方教程的基础从头到尾刷了一遍。

### 关键突破点
整个 View 库学习下来，最有感触的就是这句 `Events up, props down`，有个提纲挈领的作用。
- 把注意力集中到数据的处理上，把数据看做是溪流，在组件中，数据是永恒的，不可变的。
- 单项数据流，自组件不可以修改父组件传递来的值。

![eventsprops](/img/eventsprops.png)

每一个UI组件的关键用法，都会有详细的实例，拿 [Button](https://element.eleme.cn/#/zh-CN/component/button) 举例

## 做 & 模仿最佳实践
以及这些开源的项目只是模板，

[vue-element-admin](<https://github.com/PanJiaChen/vue-element-admin/blob/master/README.zh-CN.md>)

但，样板代码只是用mock来的数据来，通过看公司的项目

## 想 & 项目工程的维护

记得真正开始承担项目的维护，是我在结束两个月实习后的第一份工作，那时我已经离开了师父他们，真正的第一份工作，才让我快速的成长起来，我才有主动的意识去了解和把握整个项目。也才开始知道基于 `Node` 构建的工程化的前端项目。

### 关键突破点

一切围绕根目录的`package.json`展开，我只重点关注 `script`，`dependencies`两个 key.

### 构建

在 `script` 中查看，两个前端框架都用 `CLI` 脚手架构建工具

- Vue
  - [Vue CLI](https://cli.vuejs.org/zh/guide/#cli)

- React
  - [create-react-app](https://github.com/facebook/create-react-app)
  - [umi](https://umijs.org/zh/guide/)

### 发布

在 `script` 中查看，`npm run build`，去查看根目录下的 `dist` 目录

### 部署
只要搭建一个静态服务器就可以
- Nginx
- IIS
- public

### 维护

- 巨人的肩膀
  
在 `dependencies` 中， 如果需要添加一些插件，包管理工具 [npm](<https://www.npmjs.com/>) 就是我发现的巨人的肩膀，输入英文关键字查找你想到的插件，可以加 `Vue` 和 `React` 这两个前缀。

安装需要用到 `npm install`

- 自己封装
这是较为考验思考能力的，解耦为中心思想，当时直到目前我还没有很好的掌握这个度。


### 细节与常见问题

[v-on 绑定事件时，函数名加括号和不加括号有什么区别？](<https://www.zhihu.com/question/55753541>)




