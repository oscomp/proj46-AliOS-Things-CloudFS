# proj46-AliOS-Things-CloudFS
### 项目名称
基于AliOS Things操作系统提供云文件系统

### 项目描述

文件系统是操作系统的重要组成部分，用来管理和存储大量的文件信息，负责对文件的存储空间进行分配和管理，并对存入其中的文件进行保护和检索，同时为用户提供包括文件创建、删除、命名、读写、访问控制等一系列功能。此外，文件系统还可以根据存取权限及访问操作类型来指定用户对文件的存取。
云存储伴随着云计算产生，作为云计算的先驱，它很早就进入了广大研究人员的视野，众多企业都将其作为进军云计算的第一步，目前也有很多企业面向大众提供云盘服务的企业。阿里云也面向公众提供云存储服务。
云盘功能在移动端操作系统中大多以独立应用程序的形式存在，和本地操作系统没有很好的融。
AliOS Things是阿里云智能IoT开发的物联网操作系统，在物联网领域有大量广泛的应用。
本实验的目标是在AliOS Things上面，打通云文件系统的功能。主要目的主要有三点：

1. 帮助学生掌握操作系统提供的文件系统接口的功能及需求
2. 帮助学生掌握常用云存储接口
3. 帮助学生掌握端云一体开发方式的一般流程

### 所属赛道

2021全国大学生操作系统比赛的“OS功能设计”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生（2021年春季学期或之后本科毕业的大一~大四的学生）
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2021全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

童武胜

* github
* email wusheng.tws@alibaba-inc.com

梁超众

* github
* email ethan.lcz@alibaba-inc.com



### 难度

中等



### 特征

* 文件信息更新的实时性
* 轻量级实现，避免太大性能损失
* 合适的缓存功能，避免产生过大的网络负载



### 文档

* 硬件平台：阿里云IoT官方推出的HaaS EDU K1或HaaS100
* 软件平台：AliOS Things物联网操作系统
* 云存储服务：阿里云OSS服务
* HaaS EDU K1技术文档：https://blog.csdn.net/haastech/category_10825080.html
* HaaS100快速开始文档：https://help.aliyun.com/document_detail/184184.html
* AliOS Things物联网操作系统说明文档：
* 1. (推荐使用) AliOS Things 3.3版本:https://gitee.com/alios-things/AliOS-Things/tree/rel_3.3.0/
* 1.1 OSS 组件说明文档: https://gitee.com/alios-things/AliOS-Things/tree/rel_3.3.0/components/oss
* 2. AliOS Things 3.1版本: https://github.com/alibaba/AliOS-Things/tree/dev_3.1.0_haas
* 阿里云OSS SDK说明：https://help.aliyun.com/product/31815.html?spm=a2c4g.11186623.6.540.4dc426fdq0ZNv5
* 注意，阿里云提供多种语言的OSS SDK，选择C++或C语言版SDK即可。

### License

* [Apache-2.0](https://opensource.org/licenses/Apache-2.0)



## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标

在AliOS Things操作系统及阿里云OSS SDK的基础上分步骤完成如下功能：

### 第一题

* 与导师协商，确认完成实验题目的思路及步骤
* 书写OSS功能移植及设计文档
* 先将OSS功能在AliOS Things上面运行起来，能本地文件上传、下载云端文件、获取云端文件信息

### 第二题

* 书写云文件系统设计文档
* 将OSS功能对接到AliOS Things VFS模块，将云文件系统挂在在/cloud目录下

### 第三题

* 开放题目，云文件系统的目录缓存，云文件本地缓存，端云状态同步，断点恢复等功能

### 提交内容要求

所提交的作品需要包含：

* 云文件系统设计文档：需要对本赛题的整体设计及完成功能模块的设计思想进行清楚的描述
* 云文件系统实现代码：提交的代码中需要包含云文件系统实现的所有实现代码（包含功能代码及测试代码）
