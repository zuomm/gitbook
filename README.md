# GitBook 使用教程

### 一、GitBook 准备工作

#### 安装node

GitBook 是一个基于 [Node.js](https://nodejs.org/en/) 的命令行工具，下载安装 Node.js，安装完成之后，你可以使用下面的命令来检验是否安装成功。

```
$ node -v
v7.7.1
```
#### 安装GitBook

输入下面的命令来安装 GitBook

```
$ npm install gitbook-cli -g
```
安装完成之后，你可以使用下面的命令来检验是否安装成功
```
$ gitbook -V
CLI version: 2.3.2
GitBook version: 3.2.3
```
更多详情请参照 [GitBook 安装文档](https://github.com/GitbookIO/gitbook/blob/master/docs/setup.md) 来安装


### 二、下载本项目到本地
```
$ git clone git@gitlab.0easy.com:aiotcloud/aiot-openAPI-document.git
```
### 进入项目
```
$ cd aiot-openAPI-document
```
### 安装依赖
```
$ gitbook install
```
### 运行
```
$ gitbook serve
```
注：执行gitbook serve时会自动进行build编译成html静态文件,直接在本地输入http://localhost:4000就可以查看网站了。

### 构建
```
$ gitbook build
```
注：打包后项目会多了一个_book目录，_book目录是我们需要的网站静态html文件，只需要部署_book静态文件。
![PNG](\images\build.png)

### 三、修改文件夹后需同步目录内容
SUMMARY.md
```
# Summary

* [前言](README.md)

### 基础问题

* [简介](Chapter1/1.md)
    * [使用GitBook命令行工具制作文档的步骤](Chapter1/2.md)
* [如何制作多级目录](Chapter1/3.md)

### 功能拓展

* [如何插入图片](Chapter2/1.md)
    * [如何在表格中使用竖线|](Chapter2/2.md)
* [如何在url中使用括号](Chapter2/3.md)
---
* [如何定制](Chapter3/README.md)

```

目录说明：

1. `* [目录标题1](xxx/xxx.md) ：对应一条目录，括号里面是目录对应的文件`；
2. 二级目录需要在一级目录缩进几个空格就行了；
3. gitbook最多只有三级目录；
4. 目录前面可以用 * - ；
5. ` ### 基础问题 、### 功能拓展 `这些表示目录分块展示，也可以不用，看个人需要。

### 四、友链
- [GitBook 学习笔记](https://yangjh.oschina.io/gitbook/faq/Contents.html)
- [GitBook 插件整理](https://www.jianshu.com/p/427b8bb066e6)