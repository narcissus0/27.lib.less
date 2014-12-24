less27
======

A less tool, 
Speed up coding.

###第一步
![image](https://github.com/ziven27/less27/blob/master/guide/step1.png)

打开koala<a href="http://koala-app.com" target="_blank">下载地址</a>，把doc的文件拖入。

###第二步
![image](https://github.com/ziven27/less27/blob/master/guide/step2.png)

点击执行编译，就会在style.less所在目录生成编译后的style.css文件。使用的时候直接使用style.css即可。

###第三步
![image](https://github.com/ziven27/less27/blob/master/guide/step3.png)

这是编译后的内容。


###目录结构

```tree
.
└── less27
    ├── doc
    │   ├── 27less
    │   │   ├── _27.attribute.less              --属性类
    │   │   ├── _27.css3.less                   --CSS3相关
    │   │   ├── _27.frame.less                  --布局框架
    │   │   ├── _27.library.less                --通用框架
    │   │   ├── _27.oocss.less                  --面向对象
    │   │   ├── _27.reset.less                  --CSS Reset 相关
    │   │   └── _27.style.less                  --调用其它文件
    │   └── style.less                          --27less 目录的style.less 文件
    ├── guide                                   --使用教程截图
    │   ├── step1.png
    │   ├── step2.png
    │   └── step3.png
    ├── LICENSE
    └── README.md
```