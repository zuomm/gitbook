# GitBook 使用教程

## GitBook 准备工作

### 1、安装node
GitBook 是一个基于 [Node.js](https://nodejs.org/en/) 的命令行工具，下载安装 Node.js，安装完成之后，你可以使用下面的命令来检验是否安装成功。
```
$ node -v
v7.7.1
```
### 2、安装GitBook
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


## 下载本项目到本地
```
$ git clone git@gitlab.0easy.com:aiotcloud/aiot-openAPI-document.git
```
## 进入项目
```
cd aiot-openAPI-document
```
## 安装依赖
```
$ gitbook install
```
## 运行
```
$ gitbook serve
```