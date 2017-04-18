# WRITE
### Node.js

* ##### 1.Node.js的特点

* Node.js 是一个基于 Chrome V8 引擎的 JavaScript 运行环境。 

* Node.js 使用了一个事件驱动、非阻塞式 I/O 的模型，使其轻量又高效。 

* Node.js 的包管理器 npm，是全球最大的开源库生态系统。

* ##### 2.3m安装法

* nvm(Node Version Manager)

  * 解决多版本共存,切换问题

* npm(Node Package Manager)

  * 解决Node.js模块安装问题

* nrm(NPM Registry Manager)

  * 解决npm镜像访问慢,提供测试,切换

* ##### 3.NVM

* curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh|bash

* 下载nvm,并将路径配置到~/.bashrc中

* 注:如果终端是zsh,则需要配置到~/.zshrc中(课通过echo $0查询)

  * NVM常用命令
  * nvm — version 查看当前版本
  * nvm ls 查看当前已安装node的版本
  * nvm ls-remote 查看远程node的版本
  * nvm install 4.4.5 安装某版本 node
  * nvm use 4.4.5 使用某版本 node
  * nvm alias default 4.4.5把某版本node设置为默认值

* ##### 4.NPM

* 安装完Node后自带

* npm-v 查询当前npm版本

* npm install nam -g 通过 nam 更新 npm

* npm install 模块名

* ##### 5.NRM

* npm install -g nrm

* nrm test

* nrm ls

* nrm use taobao

* ##### 6.Node.js和CommonJS之间的关系

* CommonJS是一种规范,而Node.js是这种规范的实现

* Node.js只是实现了部分CommonJS的规范

## 如何有效的学习node.js

从刚接触Node.js到现在，自己也是一路摸滚打爬过来的，虽不说是什么高手，但对于如何学习Node.js，还是有一些个人见解，拿出来与大家共勉~

学习Node.js大致有 6 个步骤或者说 6 个层次

##### 第一步

- JavaScript 的特性和语法。假如你对 JavaScript 还不熟悉的话，推荐书籍及链接：	
  - JavaScript 推荐书籍列表
  - 深入理解JavaScript系列
- Node.js 是什么？Node.js与JavaScript的区别是什么？
- Node.js的优点？Node.js的缺点？
- Node.js适用场景？Node.js不适用的场景？
- Node.js的基本语法。Node.js的特性：
  - 单线程
  - 异步IO
  - 事件驱动
- npm 是什么？npm的基本使用
- REPL

其实上面的内容，大部分Node.js的书籍都有介绍。基本了解了Node.js后，我们可以写一些 hello world 的程序：

- 搭建一个 HTTP 服务器，返回 hello, world 。(使用 HTTP 模块)
- 读取一个 txt 文件，将内容显示到命令行中。（使用 fs 模块）
- 等等

##### 第二步

你也许想，Node.js 只有那些少得可怜的核心模块能做什么呢？别担心，npm 上目前有近 7W 的第三方模块，月下载量高达 2.1亿 （2014—4—20 数据）… 这才是 Node.js 的活力所在。当你对Node.js已经了解的差不多了，并且按耐不住跃跃欲试了。这个时候，我们不妨用 Node.js 的第三方模块做些好玩的事情：

- 搭建一个微博网站
- 搭建一个博客网站
- 搭建一个在线聊天室
- 写一个简单的爬虫
- 调用一些网站的API做一些好玩的东西

但是，并不是说 Node.js 只能做以上事情，几乎其他语言能做的事情 Node.js 都能做，而且有些情况下能做的更好。

##### 第三步

当然，就像学 js 也不能只会用框架一样，学习 Node.js 也不能只会用外部模块。这个时候，我们需要回头深入了解下 Node.js 核心模块的用法。说白了，就是好好看 Node.js 官方 API 文档。看文档是码农必备技能，英语不好的童鞋浏览器装个划词翻译的插件。

##### 第四步

- 多实践。不管是用核心模块还是外部模块，尝试用 Node.js 解决某个问题或者替换掉以前用其他语言写过的代码。
- 读源码。这里说的读源码并不是说上来就去读 Node 或者其他较大的框架的源码。这个时候，挑一些简单的只实现某个特定功能的工具模块的源码读，这种模块的代码通常在几百行，阅读起来并不是很困难，但是却能涨不少的姿势。比如：
  - underscore （学习 JavaScript 的语法和技巧）

##### 第五步

坚持第四步。在使用 Node.js 时发现没有合适的模块选择或者选择的模块功能不尽人意，这个时候你可以尝试去创建一个模块或者修改现有的模块，并且使用 npm 发布自己的模块或者去该模块的 GitHub  上提 PR 。

##### 第六步

- 多实践。这个就不用解释了
- 读 Node 源码及较大的框架的源码。提高必备
- 多关注下 GitHub 上的牛人
- 重复第1-6步

PS: 贯穿始终的是买几本 Node.js 的书读，推荐《深入浅出Node.js》。

