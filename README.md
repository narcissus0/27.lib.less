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
