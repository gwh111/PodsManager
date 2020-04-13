# PodsManager

[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://opensource.org/licenses/MIT "Feel free to contribute.")

Pods Manager beta版  
视频教程[https://www.bilibili.com/video/BV1pE411x7mJ](https://www.bilibili.com/video/BV1pE411x7mJ)  
PodsManager Tutorials[https://youtu.be/l9wxOOsLaLM](https://youtu.be/l9wxOOsLaLM)

<img width=800px src="https://github.com/gwh111/PodsManager/blob/master/PMVideo.002.jpeg?raw=true" >  
<img width=800px src="https://github.com/gwh111/PodsManager/blob/master/PMVideo.003.jpeg?raw=true" >  
<img width=800px src="https://github.com/gwh111/PodsManager/blob/master/PMVideo.004.jpeg?raw=true" >

如无法打开，解决步骤  
1、系统偏好设置-安全-允许任何来源。  
2、[Mac应用程序“XXX”不能打开？一条命令就搞定！](https://cloud.tencent.com/developer/article/1508073)


Pods Manager  
不需要一个很小的组件就建一个仓库了  
新建一个自己的仓库存放组件，可以是私有也可以是公开    
使用GitHub，新建一个repository作为组件安放的仓库，将仓库地址填到git栏里。

## 一、安装组件
1. 使用Cornerstone/GitHub客户端 checkout项目
2. 在右测+项目/组件 工程到项目/组件 列表，选择整个项目外面的文件夹
3. 在左侧更新组件列表，从组件看板选择组件+-到列表
4. 点击添加更新podfile
5. 安装

## 二、更新组件
1. 用Cornerstone/GitHub客户端  checkout组件代码
2. 用Xcode编写组件新版代码，用Cornerstone/GitHub客户端 提交代码！
3. 在右侧+组件工程到组件列表
4. 修改版本号，回车
5. 添加示例code
6. 提交
更新组件看板即可查看提交版本

## 三、新建xxx组件
1. 新建xxx文件夹
2. Xcode新建项目到xxx文件夹内，目录如下，目的是为了使用时可以从ccs.xxx 获取实例
```
├── xxx.xcodeproj
├── ...
├── xxx
│   ├── AppDelegate.h
│   ├── ...
│   ├── xxx
│   │   ├── ccs+xxx.h
│   │   ├── ccs+xxx.m
│   │   ├── xxxLib 或 xxxC
│   │   ├── ...
```
3. 使用Cornerstone/GitHub客户端  提交代码，Pod文件夹不要提交！
4. 添加示例code
5. 提交
更新组件看板即可查看提交版本

## 注意：手动编写podfile和podspec时严格按照默认格式
Error：*fatal: could not read Username for 'https://github.com': Device not configured*  
使用GitHub作为仓库时出现该错误可以打开终端手动推送一次 'git push origin master'，然后输入用户名密码。  
或百度该错误找到.git配置文件配置账户

Error：*/bin/bash: /usr/local/bin/pod: No such file or directory*
sudo gem install -n /usr/local/bin cocoapods

