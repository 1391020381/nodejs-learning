# cpu密集vs I/O密集
1. cpu密集:压缩、解压、加密、解密
2. I/O密集:文件操作、网络操作、数据库
# web常见场景
1. 静态资源的读取(css/js/image)
2. 数据库操作
3. 渲染页面
# 进程
是计算机中的程序关于某个数据集合上的一次运行活动,是系统进行资源分配和调度的基本单位(正在进行中的程序)
# 线程
进程内一个相对独立的、可调度的执行单元,与同属一个进程的线程共享进程的资源。
多线程:启动一个进程,在一个进程内启动多个线程,这样,多个线程也可以一块执行多个任务。

# NodeJS的单线程
1. 单线程只是针对主进程,I/O操作系统底层多线程调度
2. 单线程并不是单进程(node有集群的概念)

# 常用场景
1. Web Server
2. 本地代码构建
3. 实用工具开发

# 在node中尽量使用异步操作，如果使用通过操作,又可能一个用户就可以堵塞主进程,就发挥不了node的调度的优势。<类似服务员和大厨的关系。node的住进程就是服务员负责调度,I/O就是大厨。>

# 在github上创建项目是不要忘记,勾选 初始化项目时带有 README.md和.gitignore以及license
# github上项目clone时可以选择使用  Use HTTPS还是 Use SSH <点击图标可以切换>

# .gitignore
1. 匹配模式前 / 代表项目根目录
2. 匹配模式最后加 / 代表是目录
3. 匹配模式前加 ! 代表取反
4. * 代表任意字符
5.  ?匹配任意一个字符
6. ** 匹配多级目录

# [ESLint](http://eslint.cn/docs/user-guide/command-line-interface#init) 
eslint --init
#Accept-Encoding
* Accept-Encoding:gzip,deflate
# Content-Encoding
* Content-Encoding: gzip
[RisingStack](https://blog.risingstack.com/)
[Fiddler抓包](http://www.cnblogs.com/yoyoketang/tag/fiddler/)