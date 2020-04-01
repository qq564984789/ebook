---
abbrlink: 354222414
cover: true
categories:  Gitbook
tags:  Gitbook
keywords:  Gitbook
---
### 什么是Gitbook?
[Gitbook](https://www.gitbook.com/)是2014年中期发布的一款面向开发者文档书写的开源工具。作为一个文档平台，公司团队可以基于Gitbook编写产品说明书或公司内部的知识库。Gitbook的目标是成为一个人性化的协同合作产品，保证每个人都可以通过文档来创建、编辑、分享知识。
### Gitbook能做什么？
- (团队)异步合作
- 分享你的知识：公开或私有
- 文档中加入小黄连（Emoji）
### 实验环境
- OS：Win10
- node.js：12.13.1
- npm：6.12.1
### 动手实验
1. 安装gitbook客户端

   ```bash
    npm install -g gitbook-cli@2.3.0
   
   ```
 上述语句执行结果如下图所示：
![](http://yangkai123.top/QQ截图20200401173745.png)
> 我们这里安装的是2.3.0版本，因为当前最新的2.3.2版本似乎有bug。
2. 新建一个文件目录，用于存放将来自制的电子书。我这里取名为`gitbook`。
3. 在新建目录`gitbook`下执行

  ```bash
  gitbook init
  ```
 上述语句执行结果如下图所示：
![](http://yangkai123.top/image-20200401174514992-1585734392811.png)
   最后显示内容为：<img src="http://yangkai123.top/20200401175146.png"  />
  不难发现，上述指令会在你新建的目录下创建`README.md`和`SUMMARY.md`两个文档。`SUMMARY.md`文档用于存放电子书的目录（章节标题）。
4. 启动`gitbook`服务

   ```bash
   gitbook serve
   ```
   上述语句执行结果如下图所示：
   ![](http://yangkai123.top/20200401175534.png)
   > 该命令其实首先会调用 gitbook build 编译书籍，然后打开一个 web 服务器，在本地的 4000 端口监听服务。
   > 
 5. 查看电子书：在浏览器中输入上述`http://localhost:4000/`网址即可查看。
