27.lib.less
======

> **27.lib.less**一个加快css编写的less库

因为基于[less](http://www.bootcss.com/p/lesscss/)，所以希望你对less有一定的了解。如果你懒，你也是可以不用了解的。因为本库只是借用了的less的语言特性，其用法是可以完全独立的。

27.lib.less目的在于减少你的css代码量，并提供尽可能多的代码片段来提升你的代码效率。

27.lib.less可以这样来写css

```less
/* 输入 */
.box{
	#wHlh(100px,40px);
	#paTl(50%);
	#mtL(-15px,25px);
	#bcC(#000,#fff);
	border:1px solid #ddd;
}

/* 编译输出 */
.box {
  height: 40px;
  width: 100px;
  line-height: 40px;
  position: absolute;
  top: 50%;
  left: 50%;
  margin-top: -15px;
  margin-left: 25px;
  background-color: #000000;
  color: #ffffff;
  border: 1px solid #ddd;
}
```
代码量减少了有没有？效率提高了有没有？是不是很神奇？

我知道你现在一脸懵B，粗看这个写法确实很难懂！没有关系，其实知道真相的你眼泪会掉下来，因为真的很简单，请听我慢慢道来。

## 目录结构

```tree
.
|____ _27
| |____ _core.less         --核心库，属性类
| |____ _grid.less         --删格布局
| |____ _reset.less        --css reset 相关
| |____ _lib.less          --常用样式
| |____ _oocss.less        --面向对象
| |____ _init.less         --总入口（此处调用了以上所有的库）
|***
|____ style.less           --在此处引入_27/_init.less，并进行其他代码编写

```
***27.lib.less*** 一共有1个核心文件`_core`，4个拓展文件，以及一个入口文件`_init`组成。除了入口文件有调用所有库文件以外，其它5个库文件相互独立。并且里面的方法都只是声明，直接引入项目只要不调用就不会生成任何代码，无污染，无残留。你也可以根据你实际的项目，添加自定义拓展库，只要遵循命名规则即可。

## 使用方法

1. 将_27文件夹放到你的项目目录中
2. 在需要使用这个库的less文件顶部采用相对路径`@import`引入。  
例：` @import "_27/_init.less"; `
3. 用less编译工具编译即可

## 编译工具
1. [koala](http://koala-app.com/index-zh.html)是一个前端预处理器语言图形编译工具，支持Less、Sass、Compass、CoffeeScript，帮助web开发者更高效地使用它们进行开发。跨平台运行，完美兼容windows、linux、mac。
2. [gulp-less](https://www.npmjs.com/package/gulp-less)命令行工具glup的less插件。

## wiki

- [Home](https://github.com/ziven27/27.lib.less/wiki)
- [1.快速开始](https://github.com/ziven27/27.lib.less/wiki/1.%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B)
- [2._core.less](https://github.com/ziven27/27.lib.less/wiki/2._core.less)
- [3._lib.less](https://github.com/ziven27/27.lib.less/wiki/3._lib.less)
- [4._reset.less](https://github.com/ziven27/27.lib.less/wiki/4._reset.less)
- [5._grid.less](https://github.com/ziven27/27.lib.less/wiki/5._grid.less)
- [6._oocss.less](https://github.com/ziven27/27.lib.less/wiki/6._oocss.less)

