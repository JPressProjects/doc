# JPress文档



## 开始
演示站点：[http://www.yangfuhai.com](http://www.yangfuhai.com) （也是作者博客）

JPress官网：[http://jpress.io](http://jpress.io) 

### 简介
JPress，一个wordpress的java代替版本，使用JFinal开发。支持类似wordpress的几乎所有功能，比如：模板，插件等。同时在模板上，JPress提出了“模板即模型”的概念，方便模板制作人灵活制作业务模型，移除了widget等繁杂功能，同时在模板和插件制作上比wordpress更加灵活简洁。

但是，JPress又不是wordpress的java版本，它天生融合了微信公众平台，整合了国内众多云平台、短信发送、邮件发送平台，独创的“模板即模型”概念是wordpress所不具备的，只有资深的wordpress玩家才能体会里面的微妙关系。同时后续会添加微信文章同步，QQ公众平台，今日头条，一点资讯等新媒体的文章同步功能，更加国产和本地化。


### 下载
目前JPress托管在github和git.oschina.net上，网址分别是：

* [https://github.com/JpressProjects/jpress](https://github.com/JpressProjects/jpress)
* [http://git.oschina.net/fuhai/jpress](http://git.oschina.net/fuhai/jpress)

可以通过以上网址查看JPress的更新情况。

目前下载可以进入以上两个网站直接通过浏览器下载ZIP压缩包，也可以通过以下git命令下载到本地。

<center> `git clone https://github.com/JpressProjects/jpress.git` </center>
或
<center> `git clone https://git.oschina.net/fuhai/jpress.git` </center>


## 部署
### 环境配置

#### JAVA环境配置
目前假定您已经配置好了JAVA环境，若不会配置JAVA环境，请自行通过搜索引擎搜索相关知识。

#### Maven环境配置
暂略...

### JPress安装

#### tomcat安装
暂略...

#### JPress安装
如果您已经在您的服务器配置好了相关应用，比如tomcat，nginx等，就可以进行JPress安装了。

主要有一下三个步骤：

##### 第1步：生成war包
下载到本地后，进入jpress-web目录，执行`mvn package`命令，稍等片刻，命令执行完毕后会在jpress-web目录生成一个jpress-web-1.0.war的war包（可能今后jpress升级后，版本可能不是1.0了），拷贝war包放到tomcat的webapp目录下即可运行。

##### 第2步：拷贝war到tomcat并运行
拷贝第一个生成的war包到tomcat的webapp目录，启动tomcat。

##### 第3步：浏览器访问tomcat，进行配置
当jpress第一次运行的时候，jpress会去检测`class path`目录下是否有db.properties数据库配置文件，如果没有该文件，证明jpress是第一次运行。当浏览器访问jpress时，jpress会自动跳转到安装页面，让用户进行安装。


#### JPress安装注意事项
1. JPress要求数据库 ***必须*** 在5.5以上，建议最好是`5.6`或`5.6以上`。
2. JPress在安装的过程中，需要用用户自己创建好数据库，JPress在安装的过程中只做建表工作。


## 后台管理

### 进入后台
当JPress安装完毕后，访问http://yoursite.com/admin（本地：`http://127.0.0.1/admin`），输入安装配置的账号密码，即可进入管理后台。

### 内容发布
### 网站配置
#### 常规
#### 评论
#### 通知
#### SEO
#### 水印
#### 连接形式

### 微信相关

#### 自动回复
#### 默认回复
#### 菜单设置
#### 微信配置



## 模板开发
###模板结构
###模板标签
###模板设置

## 插件开发
### helloworld
### 规范
### 钩子

## 高级
### 二次开发
### 数据库操作

## 关于
### 开发者
### JPress