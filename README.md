less27 - a quick less code library
======

Coding quickens as in the rocket.

简介
---------------
这是一个基于less的代码库，所以希望你对less有一定的了解。[less简介](http://www.bootcss.com/p/lesscss/)。

27.lib.less目的在于进一步减少你的less代码量，并提供尽可能多的代码片段来提升你的代码效率。

27.lib.less可以这样来写less

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

#目录结构

```tree
.
|____ css
| |____ style.css            --目标文件
|____ less
| |____ _27
| | |____ _attr.less         --属性类
| | |____ _css3.less         --css3 相关
| | |____ _grid.less         --删格布局
| | |____ _reset.less        --css reset 相关
| | |____ _lib.less          --常用样式
| | |____ _oocss.less        --面向对象
| | |____ _init.less         --总入口（此处调用了以上所有的库）
| |____ style.less           --在此处引入_27._init.less，并进行其他代码编写

```
