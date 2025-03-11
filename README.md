![logo](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/log.png)


<p align="center">
  <a href="https://gitee.com/Runner-Go-Team/RunnerGo/releases/tag/v1.1.3">
    <img src="https://img.shields.io/badge/releases-v1.1.3-brightgreen.svg" alt="vue">
   <a href="https://gitee.com/Runner-Go-Team/RunnerGo/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-Apache License 2.0-brightgreen.svg" alt="vue">
 <a href="https://gitee.com/Runner-Go-Team/RunnerGo/releases/tag/v1.0.4">
    <img src="https://img.shields.io/badge/download-18.3KB-brightgreen.svg" alt="vue">
   <a href="https://wiki.runnergo.cn/docs/">
    <img src="https://img.shields.io/badge/document-RunnerGo-brightgreen.svg" alt="vue">


## 源码清单：

### runnerGo-management-websocket-open

https://gitee.com/Runner-Go-Team/Runner-go-management-websocket-open

### runnergo-management-open
https://gitee.com/Runner-Go-Team/runnergo-management-open

### runnergo-collector-open
https://gitee.com/Runner-Go-Team/runnergo-collector-open

### runnergo-engine-open
https://gitee.com/Runner-Go-Team/runnergo-engine-open

### file-server
https://gitee.com/Runner-Go-Team/file-server

### runnergo-fe-open
https://gitee.com/Runner-Go-Team/runnergo-fe-open

### runnergo-fe-admin-open
https://github.com/Runner-Go-Team/runnergo-fe-admin-open

### runnergo-permission-open
https://github.com/Runner-Go-Team/RunnerGo-permission-open



## 基于go语言的一体化性能压测工具

RunnerGo致力于打造成一款全栈式测试平台，采用了较为宽松的Apache-2.0 license开源协议，方便志同道合的朋友一起为开源贡献力量，目前实现了接口测试、场景自动化测试、性能测试等测试能力。随着不断的迭代，我们将会推出更多的测试功能。我们的目的是为研发赋能，让测试更简单。

## 工具特性：
- go语言运行：基于go语言开发，运行速度快、更节省资源
- 智能调度算法：自研的调度算法，合理利用服务器资源，降低资源消耗
- 实时生成测试报告：运行任务后，可实时查看执行结果，快速诊断服务病症
- 丰富的报告图表： 全方位展示各个指标运行曲线图
- 实时修改： 可根据压测模式实时修改并发数、持续时长等
- 实时日志： 可在压测过程中开启日志模式，查看请求响应信息
- 可编辑报告：可在任务运行结束后，针对测试结果进行测试分析，实时编写报告
- Flow场景流：可视化的业务流，通过连线就可快速搭建起来自己的业务流，还可直接调试运行场景，电流般的业务流转
- 多种压测模式：支持并发模式、阶梯模式、错误率模式、响应时间模式、每秒应答数模式、轮次模式等多种压测模式，支持根据机器自定义分布配置，满足所有业务需求
- 自持接口自动化，采用用例集概念，生成丰富的自动化报告
- Mock服务：支持自定义请求校验与响应期望
- 企业管理后台：支持多团队管理，通过权限设置来管理员工，保护公司数据安全和流量资源

### 首页展示
![interface](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/home.jpg)

### 性能测试报告
![report](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/stress_report.jpg)

### 性能测试报告对比
![报告对比.jpg](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/contrast.jpg)

### 自动化测试报告
![report](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/auto_report.jpg)

### Mock服务

![report](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/mock.png)

### 企业管理后台

![report](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/2.3.0-9.png)

### 官网地址
[http://www.runnergo.com/](http://www.runnergo.com/)

## 快速开始

开源版安装教程请见： https://wiki.runnergo.cn/docs/42

默认超管账号**runnergo**  密码**runnergo**

里面有非常详细的图文教程，如需远程指导，也可划到当前页面最下方添加我们的微信，我们会为您提供安装帮助。


## 技术栈
- 后端: GoLang
- 前端: React.js
- 中间件: MySQL, MongoDB, Kafka, ZooKeeper, Redis
- 基础设施: Docker
- 测试引擎: GoLang

## 技术架构
![struct](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/struct.png)

## 业务流转图
![flow](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/images/flow.png)

## 联系我们
![qrcode](https://apipost.oss-cn-beijing.aliyuncs.com/kunpeng/lianxi.png)

环境要求
docker版在线安装
一、环境要求
1.1 部署服务器要求
操作系统：任何支持 Docker 的 Linux x86
CPU内存：最低要求 4C8G，推荐 8C16G
网络要求：可访问互联网
​ ❗ 并发量较大时，请关注您的带宽、服务器的cpu及内存使用率等，以免影响测试结果和业务运行。

1.2 网络端口要求
为保证RunnerGo正常运行，需要网络环境提供如下的网络端口配置要求，管理员可根据实际环境，在网络侧和主机侧开放相关端口：

组件	默认端口	说明
collector	30000	测试数据处理（报告）服务
admin-fe	9998	企业后台-ui 服务
web-ui	9999	web-ui服务
file-server	80	存储测试文件及头像服务
engine	30000	发压机
manage	58889	管理服务，包括增删改查以及压力机调度
manage-ws	58887	management-ws服务是用于把一些轮询接口，改成websocket互通消息的方式
permission	58890	企业后台及权限服务
mock	30003	http mock 服务
Mongo	27017	默认安装的Mongo数据库 对外提供的端口
MySQL	3306	默认安装的数据库对外提供的端口
Redis	6379	默认安装的 Redis 对外提供的端口
Kafka	9092	默认安装的Kafka 对外提供的端口
zookeeper	2181	默认安装的zk 对外提供的端口
Linux离线安装版本相关端口：

组件	默认端口	说明
Runnergo-ui	8181	企业后台-ui 服务
Zookeeper	2181	默认安装的zk 对外提供的端口
Kafka	9092	默认安装的Kafka 对外提供的端口
MySQL	3306	默认安装的数据库对外提供的端口
Redis	6379	默认安装的 Redis 对外提供的端口
Mongo	27017	默认安装的Mongo数据库 对外提供的端口
Windows安装
以windows 10系统为例

1、设置手动进入系统BIOS启用虚拟化技术
（展示型号是HUAWEI MateBook13），重启电脑按F2进入BIOS，然后启用虚拟化

(Inter启动虚拟化)将Virtualization Technology 设置为 <Enable>

[image.png](https://wiki.runnergo.cn/assets/images/install1-48122723997ae5fa6bd5fe8c37150cd5.jpg)

（AMD启动虚拟化）将SVM Mode 设置为 <Enabled>

[image.png](https://wiki.runnergo.cn/assets/images/install2-68d10be321b6e4aa226382330997ec12.png)

2、启动Hyper-V服务
进入控制面板-程序-启动或关闭Windows功能

[image.png](https://wiki.runnergo.cn/assets/images/install3-8afb1bde2c91a1a54c05b4311d4e8015.png)

3、下载docker并安装
下载地址：https://docker.p2hp.com/

下载后安装



4、下载git
下载地址：https://git-scm.com/

下载后安装

image.png

5、以管理员身份运行powershell，选择部署RunnerGo目录路径
（示例为安装D盘）

d:

[image.png](https://wiki.runnergo.cn/assets/images/78805a221a988e79ef3f42d7c5bfd4186589237a27a88-6195de44b877cb899a416f7538adf64a.png)

6、准备 docker 和 docker-compose 环境
git clone https://github.com/Runner-Go-Team/RunnerGo.git

或

git clone https://gitee.com/Runner-Go-Team/RunnerGo.git

[image.png](https://wiki.runnergo.cn/assets/images/78805a221a988e79ef3f42d7c5bfd4186589238cf3ef8-0e33feed070902f0d9c27b385823fba5.png)

7、进入RunnerGo目录
cd RunnerGo

[image.png](https://wiki.runnergo.cn/assets/images/78805a221a988e79ef3f42d7c5bfd418658923a185c12-0d5735e6b11641e6284cce5c5f84b966.png)

cd runnergo

[image.png](https://wiki.runnergo.cn/assets/images/78805a221a988e79ef3f42d7c5bfd418658923bb32127-164ff768adfdd3d3e34dea7c0cb7a382.png)

8、启动RunnerGo
docker compose up -d

由于启动的中间件多，请耐心等待下载完成后，使用下面命令查看是否都启动成功

docker compose ps

9、使用RunnerGo
安装成功后，在浏览器打开以下地址页面，即可登录使用

默认超管账号runnergo 密码runnergo

地址：http://本机外网地址:9998

image.png

查看本机外网地址

ipconfig

image.png

9、其他事项
如果功能中没有Hyper-V
需要运行（windows+R）打开 PowerShell，输入指令systeminfo显示

Hyper-V要求： 已检测到虚拟机监控程序。将不显示Hyper-V 所需的功能

image.png

然后我们新建文本，输入下面代码

pushd "%~dp0"
dir /b %SystemRoot%\servicing\Packages\
*Hyper-V*
.mum >hyper-v.txt
for /f %%i in ('findstr /i . hyper-v.txt 2^>nul') do dism /online /norestart /add-package:"%SystemRoot%\servicing\Packages\%%i"
del hyper-v.txt
Dism /online /enable-feature /featurename:Microsoft-Hyper-V-All /LimitAccess /ALL


保存为bat或cmd格式，然后以管理员方式运行，再重启电脑，即可。

安装docker后打开，如果一直在Starting the Docker Engine...
image.png

首先要更新WSL的版本，直接在PowerShell中执行（确保在管理员权限下打开）

wsl --update

确保WSL安装更新正确

wsl -l #list wsl installed
wsl --update

更新网络配置重启电脑

如何管理员权限运行PowerShell
通过 “运行”程序并使用快捷键提升权限：按下 Win + R 调出 “运行”对话框，再输入 “PowerShell”,输入后 按下 “CTRL + Shift + Enter”，即可以管理员运行。

[image.png](https://wiki.runnergo.cn/assets/images/install13-b4da174684124b9cd8e8cff8f0c73199.png)

通过搜索 “PowerShell”并右键选择 “以管理员权限运行”：按下“Win”并搜索“PowerShell”，并右键选择 “以管理员权限运行”

[image.png](https://wiki.runnergo.cn/assets/images/install14-333378f06b0e69b7fb6c882f065bc0a2.png)

源码部署

安装golang环境
💡
源码部署需具有Debug能力

RunnerGo项目的后端接口部分，基于Gin框架设计实现

Linux安装教程

Mac安装教程

Windowns安装教程

三、下载源码地址
四、本地使用
1、克隆代码 git clone https://github.com/Runner-Go-Team/RunnerGo-management-open.git

2、进入项目跟目录 cd RunnerGo-management-open

3、下载或更新依赖 go mod tidy

4、启动项目 go run main.go

五、配置文件相关
1、进入配置文件目录 cd RunnerGo-management-open/configs/*.yaml文件
（dev.yaml:开发环境，test.yaml:测试环境，prd.yaml：生产环境）

2、配置详情，请参考RunnerGo-management-open根目录下的README.md文件

3、关键配置解释

# clients下面的配置，主要是management请求压力机相关接口的配置，压力机服务为RunnerGo-engine-open，其中domain对应的就是RunnerGo-engine-open服务对应的IP或域名。
clients:
  runner:
    run_api: "https://domain/runner/run_api"
    run_scene: "https://domain/runner/run_scene"
    stop_scene: "https://domain/runner/stop_scene"
    run_plan: "https://domain/runner/run_plan"
    stop_plan: "https://domain/runner/stop"
    
# 下面两个redis，第一个主要是用来做日常缓存使用，第二个redis主要用来做报告数据的缓存，因为报告数据数据量比较到，所以才分开两个redis服务，个人使用的话，可以把两个redis配置成一样的值，使用一个redis服务即可。
redis:
  address: "1234.redis.rds.aliyuncs.com:6379"
  password: "******"
  db: 0

redisReport:
  address: "abcd.redis.rds.aliyuncs.com:6379"
  password: "******"
  db: 0
 
# 邮箱服务配置，主要用来发送邀请链接，运行计划报告等功能，如需使用，配置上自己的对应邮箱配置即可。       
smtp:
  host: "smtpdm.aliyun.com"
  port: 465
  email: "****@qq.com"
  password: "******"
  
# 短信服务，主要用来注册的时候给用户发短信验证码使用，若需要次服务，填写对应的账号密码即可。
sms:
  id: "your ID"
  secret: "your secret"
  
#邀请链接加密密钥,主要用来对邀请链接里面包含的参数进行加密，该字符串可任意填写一个密钥字符串即可，需要注意的是，改密钥的长度必须为，16，24，32这三种长度中的一种。   
inviteData:
  AesSecretKey:  "****************"


六、创建mysql数据库表
1、安装mysql，Mac安装、Linux安装、Windows安装

2、安装完以后，创建一个runnergo数据库，然后把根目录 RunnerGo-management-open/cmd/runnergo_database.sql拿出来，进入到你创建的数据库，然后执行这个sql文件，就会把对应的数据库创建好。
