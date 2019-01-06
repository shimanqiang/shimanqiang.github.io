title: Hexo搭建博客-01
categories:
  - 杂七杂八
tags:
  - Hexo
  - 博客
date: 2019-01-06 16:47:29
---
# Hexo搭建博客系列-01

## 配置环境

### 安装
#### 安装前提
- Git
- Node.js
    
如果您的电脑中已经安装上述必备程序，那么恭喜您！接下来只需要使用 npm 即可完成 Hexo 的安装。

```
$ npm install -g hexo-cli
```
#### 安装Git
- Windows：下载并安装 git.
- Mac：使用 Homebrew, MacPorts ：brew install git;或下载 安装程序 安装。
- Linux (Ubuntu, Debian)：sudo apt-get install git-core
- Linux (Fedora, Red Hat, CentOS)：sudo yum install git-core

#### 安装Node.js
安装 Node.js 的最佳方式是使用 nvm。

cURL:

```
$ curl https://raw.github.com/creationix/nvm/v0.33.11/install.sh | sh
```
Wget:

```
$ wget -qO- https://raw.github.com/creationix/nvm/v0.33.11/install.sh | sh
```
安装完成后，重启终端并执行下列命令即可安装 Node.js。

```
$ nvm install stable
```

或者您也可以下载 安装程序 来安装。

#### 安装Hexo

```
$ npm install -g hexo-cli

```

## 建立博客
### 初始化博客
首先，进入到你的工作目录，执行以下命令

```
$ hexo init myblog

$ cd myblog && npm install

$ tree -L 1
.
├── _config.yml
├── node_modules
├── package-lock.json
├── package.json
├── scaffolds
├── source
└── themes
```

此时，基本一个博客站点就建立好了，来看看效果吧

### 部署博客
#### 命令
- 生成静态文件

  ```
  $ hexo generate
  $ hexo g   ## 该命令简写方式
  
  选项	描述
  -d, --deploy	文件生成后立即部署网站
  -w, --watch	监视文件变动
  
  ```

- 启动本地Hexo服务

  ```
  $ hexo server
  $ hexo s ##该命令可以简写
  启动服务器。默认情况下，访问网址为： http://localhost:4000/。

  选项	描述
  -p, --port	重设端口
  -s, --static	只使用静态文件
  -l, --log	启动日记记录，使用覆盖记录格式
  
  eg. hexo -p 9000 server
  ```

- 部署网站（比如：github pages）

  ```
  $ hexo deploy
  $ hexo d  ##该命令可以简写

  参数	描述
  -g, --generate	部署之前预先生成静态文件
  ```

#### 演示
  ```
  http://localhost:4000
  ```
  - hexo初始化时，默认有一篇文章的，关于如何创建文章。

## 参考资料
- 官方文档：https://hexo.io/zh-cn/docs/
    
    
    
    
    