---
title: 2020前端面试准备，拿不到offer算我输！
top: false
cover: false
toc: true
mathjax: true
date: 2019-12-31 14:34:01
password:
summary:
tags:
categories:
---

### <center>HTML</center>

#### 1.语义化

>Web语义化是指使用恰当语义的html标签、class类名等内容，让页面具有良好的结构与含义，从而让人和机器都能快速理解网页内容。

- 正确的标签做正确的事情
- 页面内容结构化
- 无CSS样子时也容易阅读，便于阅读维护和理解
- 便于浏览器、搜索引擎解析。 利于爬虫标记、利于SEO

###### 1. html 语义化

> HTML为网页文档内容提供上下文结构和含义。对于HTML体系而言，Web语义化是指使用语义恰当的标签，使页面有良好的结构，让页面元素有含义，便于被浏览器、搜索引擎解析、利于SEO

```html
<html>
    <body>
        <article>
            <header>
                <h1>h1 - WEB 语义化</h1>
            </header>
            <nav>
                <ul>
                    <li>nav1 - HTML语义化</li>
                    <li>nav2 - CSS语义化</li>
                </ul>
            </nav>
            <section>
                section1 - HTML语义化
            </section>
            <section>
                section2 - CSS语义化
            </section>
            <time datetime="2018-03-23" pubdate>time - 2018年03月23日</time>
            <footer> footer - by 小维</footer>
        </article>
    </body>
</html>
```

###### 2.css语义化

> CSS语义就是class和ID命名的语义,指用易于理解的名称对html标签附加的class或id命名,良好的CSS命名方式减少沟通调试成本，易于理解。    

例: 

```html
<!-- 以表现为中心 -->
<div class="ft margin10">
    <span>用户名：小维</span>
<div>

<!-- 以信息为中心 -->
<p class="user_info">
    <em>用户名:小维</em>
<p>
```

__问__：既然CSS class和ID命名的语义化可以便于阅读理解和减少沟通调试成本，那么我们是不是可以用div 结合class和ID语义化命名的方式来代替html的语义化？

从代码的层面上来看，使用CSS class语义化的命名也是能够便于阅读和维护的，但是这样子并不利于__SEO__和__屏幕阅读器识别__。

---

#### 2.新标签新特性

- __新特性__

1. 语意特性,添加 ``` <header><header/><nav><nav> ```等标签
2. 多媒体， 用于媒介回放的 video 和 audio 元素
3. 图像效果，用于绘画的 canvas 元素，svg元素等
4. 离线 & 存储,对本地离线存储的更好的支持,local Store,Cookies等
5. 设备兼容特性 ，HTML5提供了前所未有的数据与应用接入开放接口。使外部应用可以直接与浏览器内部的数据直接相连，
6. 连接特性，更有效的连接工作效率，使得基于页面的实时聊天，更快速的网页游戏体验，更优化的在线交流得到了实现。HTML5拥有更有效的服务器推送技术，Server-Sent Event和WebSockets就是其中的两个特性。
7. 性能与集成特性，HTML5会通过XMLHttpRequest2等技术，帮助您的Web应用和网站在多样化的环境中更快速的工作

- __新标签__

1. 多媒体：```<audio></audio>, <video><video>,<source></source>, <embed></embed>, <track></track>```
2. 新表单元素：```<datalist> ,<output> , <keygen>```
3. 新文档节段和纲要: ``` <header>页面头部、<section>章节、<aside>边栏、<article>文档内容、<footer>页面底部、<section>章节、<aside>边栏、<article>文档内容、<footer>页面底部等```

__注：__ 使用html5shiv可以解决ie低版本不兼容的问题，只需要在head中加上,当版本低于IE9时，浏览器会加载html5.js脚本，使得支持html5的新功能，也可以将脚本文件下载到本地。

```html
<head>
  <!--[if lt IE 9]>
  <script src='http://apps.bdimg.com/libs/html5shiv/3.7/html5shiv.min.js'>
  </script>
  <![endif]-->
</head>
```

# <center>（待更新）</center>

#### 3.input和textarea的区别

#### 4.用一个div模拟textarea的实现

#### 5.移动设备忽略将页面中的数字识别为电话号码的方法

### CSS

#### 1.盒模型

#### 2.flex

#### 3.css单位

#### 4.css选择器

#### 5.bfc 清除浮动

#### 6.层叠上下文

#### 7.常见页面布局

#### 8.响应式布局

#### 9.css预处理，后处理

#### 10.css3新特性

##### 1.animation和transiton的相关属性

##### 2.animate和translate

#### 11.display哪些取值

#### 12.相邻的两个inline-block节点为什么会出现间隔，该如何解决

#### 13.meta viewport 移动端适配

#### 14.CSS实现宽度自适应100%，宽高16:9的比例的矩形

#### 15.rem布局的优缺点

#### 16.画三角形

#### 17.1像素边框问题

## JS

- 1、原型/原型链/构造函数/实例/继承
- 2、有几种方式可以实现继承
- 3、用原型实现继承有什么缺点，怎么解决
- 4、arguments
- 5、数据类型判断
- 6、作用域链、闭包、作用域
- 7、Ajax的原生写法
- 8、对象深拷贝、浅拷贝
- 9、图片懒加载、预加载
- 10、实现页面加载进度条
- 11、this关键字
- 12、函数式编程
- 13、手动实现parseInt
- 14、为什么会有同源策略
- 15、怎么判断两个对象是否相等
- 16、事件模型
  - 事件委托、代理
  - 如何让事件先冒泡后捕获
- 17、window的onload事件和domcontentloaded
- 18、for...in迭代和for...of有什么区别
- 19、函数柯里化
- 20、call apply区别，原生实现bind
  - call，apply，bind 三者用法和区别：角度可为参数、绑定规则（显示绑定和强绑定），运行效率、运行情况。
- 21、async/await
- 22、立即执行函数和使用场景
- 23、设计模式(要求说出如何实现,应用,优缺点)/单例模式实现
- 24、iframe的缺点有哪些
- 25、数组问题
  - 数组去重
  - 数组常用方法
  - 查找数组重复项
  - 扁平化数组
  - 按数组中各项和特定值差值排序
- 26、BOM属性对象方法
- 27、服务端渲染
- 28、垃圾回收机制
- 29、eventloop
  - 进程和线程
  - 任务队列
- 30、如何快速让字符串变成已千为精度的数字

## ES6

- 1、声明 let、const
- 2、解构赋值
- 3、声明类与继承：class、extend
- 4、Promise的使用与实现
- 5、generator（异步编程、yield、next()、await 、async）
- 6、箭头函数this指向问题、拓展运算符
- 7、map和set有没有用过，如何实现一个数组去重，map数据结构有什么优点？
- 8、ES6怎么编译成ES5,css-loader原理,过程
- 9、ES6转成ES5的常见例子
  - 使用es5实现es6的class

## 浏览器

- 1、输入url到展示页面过程发生了什么？
- 2、重绘与回流
  - 重绘(repaint): 当元素样式的改变不影响布局时，浏览器将使用重绘对元素进行更新，此时由于只需要UI层面的重新像素绘制，因此 损耗较少
  - 回流(reflow): 当元素的尺寸、结构或触发某些属性时，浏览器会重新渲染页面，称为回流。此时，浏览器需要重新经过计算，计算后还需要重新页面布局，因此是较重的操作。会触发回流的操作:
     \* 页面初次渲染
     \* 浏览器窗口大小改变
     \* 元素尺寸、位置、内容发生改变
     \* 元素字体大小变化
     \* 添加或者删除可见的 dom 元素
     \* 激活 CSS 伪类（例如：:hover）
     \* 查询某些属性或调用某些方法
     \* clientWidth、clientHeight、clientTop、clientLeft
     \* offsetWidth、offsetHeight、offsetTop、offsetLeft
     \* scrollWidth、scrollHeight、scrollTop、scrollLeft
     \* getComputedStyle()
     \* getBoundingClientRect()
     \* scrollTo()
     **回流必定触发重绘，重绘不一定触发回流。重绘的开销较小，回流的代价较高。**
- 3、防抖与节流
- 4、cookies、session、sessionStorage、localStorage
- 5、浏览器内核

## 服务端与网络

- 1、常见状态码
- 2、缓存
  - 200 From cache和200 ok
  - 400,401,403状态码分别代表什么
  - 浏览器缓存
- 3、cookie, session, token
- 4、前端持久化的方式、区别
- 5、DNS是怎么解析的
- 6、cdn
- 7、计算机网络的相关协议
- 8、http/https/http2.0
- 9、get post区别
- 10、ajax、 axios库
- 11、tcp三次握手，四次挥手流程
- 12、跨域
- 13、前端安全XSS、CSRF
- 14、websocket
- 15、Http请求中的keep-alive有了解吗
- 16、网络分层
- 17、即时通信，除了Ajax和websocket
- 18、模块化，commonJS，es6，cmd，amd

## Vue

- 1、vue解决了什么问题
- 2、MVVM的理解
- 3、如何实现一个自定义组件，不同组件之间如何通信的？
- 4、nextTick
- 5、生命周期
- 6、虚拟dom的原理
- 7、双向绑定的原理？数据劫持？
- 8、组件通信
  - 父->子
  - 子->父
  - 非父子组件
- 9、Proxy 相比于 defineProperty 的优势
- 10、watch computed区别
- 11、virtual dom 原理实现
- 12、vue-router(hash， HTML5 新增的 pushState
  - 单页应用，如何实现其路由功能---路由原理
  - vue-router如何做用户登录权限等
  - 你在项目中怎么实现路由的嵌套
- 13、vuex的理解

## 前端性能优化

- 页面DOM节点太多，会出现什么问题？如何优化？
- 如何做性能监测

## SEO和语义化

这个没被问过

## 微信小程序

微信小程序和h5差异，如果有开发weex的经验，可能会加上weex

## git

一些基本命令

## 打包工具webpack

- 1、打包原理
- 2、打包插件
- 3、webpack热更新原理
- 4、优化构建速度

## 算法

- 1、排序算法
- 2、动态规划，参见背包问题
- 3、二叉树
- 4、加油站问题(贪心算法)
- 5、二分法
- 6、二叉树遍历
- 7、单链表反转
- 8、取1000个数字里面的质数
- 9、找出数组中和为给定值的两个元素，如：[1, 2, 3, 4, 5]中找出和为6的两个元素。
- 10、线性顺序存储结构和链式存储结构有什么区别？以及优缺点

## 移动端

- 1、自适应
- 2、pwa
- 3、移动端手势

## 附加题

- 1、无限滚动方案
- 2、如何处理兼容性问题
- 3、你遇到过最难的问题是什么
- 4、ES6 class与ES5 function区别及联系
- 5、vue怎么监听数组
- 6、写过webpack loader吗
- 7、微信网页版登录机制思考