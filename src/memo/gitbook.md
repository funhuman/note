# Gitbook

## 介绍

> Gitbook 是一个使用 Git 和 Markdown 构建书籍的工具。

## 环境

Gitbook 运行需要 Node.js 环境支持。

推荐使用版本管理工具 nvm（[文档](https://nvm.uihtm.com/)）管理Node.js。

下面介绍 nvm 的安装和用 nvm 管理 Node.js 的方法。

### 步骤0：确认本机环境

注意：在安装前请确保本机上没有安装过 Node.js，如有，需要卸载。

（此处略去了确认和卸载的操作方法，如有需要请去互联网寻找帮助）

### 步骤1：下载、安装 nvm

在 [nvm 文档](https://nvm.uihtm.com/) 文档页面，根据页面提示下载并安装 nvm。

![nvm 文档网页截图](/image/nvm-download-help-image.jpg)

### 步骤2：使用 nvm 安装 Node.js

使用管理员权限打开 CMD，依次运行下面的命令：

```
nvm install 10.23.0
nvm use 10.23.0
```

上面命令中第一行是安装指定版本的 nvm，第二行是让本机的 Node.js 切换到指定版本。

上面命令中的指定版本可以更改（但不宜过高，否则会无法运行 Gitbook）

##### 步骤3：使用 nvm 安装 Node.js

使用下面命令，安装 gitbook 包。

```
npm install gitbook-cli -g
```

那么，到这里，环境就算是配置完成了。

## 简单运行

下面尝试简单的运行一个 gitbook 项目，来测试环境配置是否成功。

### 步骤1：创建 gitbook 项目的目录

在电脑上一个合适位置创建一个文件夹。

### 步骤2：初始化 gitbook 目录

打开 CMD，切换到第一步创建的项目目录，运行下面的命令：

```
gitbook init
```

获得两个文件：
- REAMDE.md：项目简介
- SUMMARY.md：电子书的目录文档


### 步骤3：启动项目

打开 CMD，切换到项目目录，运行下面的命令，可以启动项目。

```
gitbook serve
```

运行成功的效果如下图所示：

![gitbook 运行成功示例图](/image/gitbook-success-example.jpg)

如果需要打包成静态网页，用于挂载在服务器，项目文件夹里的 `_book` 文件夹就是静态文件了。

## 总结

### 命令小结

安装 gitbook

```
npm install gitbook-cli -g
```

初始化项目（生成两个文件 `REAMDE.md` `SUMMARY.md`）

```
gitbook init
```

启动项目并生成静态文件
```
gitbook serve
```

## 参考

参考：
- [gitbook 教程 - 学习小集](https://myridge.gitee.io/pages/gitbooked/gitbook教程.html)
- [gitbook 教程 - W3C](https://www.w3cschool.cn/gitbook/)

更多链接：
- [Gitbook 官网（En）](https://www.gitbook.com/)
